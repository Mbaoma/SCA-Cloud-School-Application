# SCA-Cloud-School-Application
Technical Assessment for SCA Cloud School Bootcamp

## Steps
1.  Change directory into the 'docker' folder, then run the flask app
    ```
    python main.py
    ```

2.  Create the Docker image
    ```
    docker build -t your-username/cloud-school-image:v1 .
    ```
    Example
    ```
    docker build -t mbaoma/cloud-school-image:v1 .
    ```

3.  Run the docker file
    ```
    docker run -p 8888:5000 --name cloud-school-image: YOURNAME/cloud-school-image:v1
    ```
    Example
    ```
    docker run -p 8888:5000 --name cloud-school-image mbaoma/cloud-school-image:v1
    ```

4.  To confirm if your container was built, run:
    ```
    docker ps -a
    ```

5.  View the image in your localhost port 8888 by typing ```localhost:8888``` in your browser

![image](https://user-images.githubusercontent.com/49791498/104234555-e2431d00-5453-11eb-870e-fe029cff8b48.png)
*Docker Image*

6.  Push the image to docker hub
    ```
    docker login
    docker push YOUR_USERNAME/cloud-school-image:v1
    ```
    The image is published on [dockerhub](https://hub.docker.com/repository/docker/mbaoma/cloud-school-image)


7.  Make your changes

8.  Remove the previous docker container by running:
    ```
    docker rm -f container-id
    ```
    
9.  Create the updated image, assign it a tag, 'latest'
    ```
    docker build -t your-username/cloud-school-image:latest .
    ```
    Example
    ```
    docker build -t mbaoma/cloud-school-image:latest .
    ```

10. Run the docker file
    ```
    docker run -p 8888:5000 --name cloud-school-image: YOURNAME/cloud-school-image:latest
    ```
    Example
    ```
    docker run -p 8888:5000 --name cloud-school-image mbaoma/cloud-school-image:latest
    ```

11. Push the updated image to DockerHub
    ```
    docker push YOUR_USERNAME/cloud-school-image:latest
    ```

12. View the update image in your local browser by typing ```localhost:8888```
    ![image](https://user-images.githubusercontent.com/49791498/104238202-8380a200-5459-11eb-9294-317a884f6186.png)
    *Updated docker image*

    The updated image is published on [dockerhub](https://hub.docker.com/repository/docker/mbaoma/cloud-school-image)
