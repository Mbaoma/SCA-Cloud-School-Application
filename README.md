# SCA-Cloud-School-Application
Technical Assessment for SCA Cloud School Bootcamp

## Steps
1.  Change directory into the 'docker' folder, then run the flask app
    ```
    python main.py
    ```

2.  Create the Docker image
    ```
    docker build -t your-username/cloud-school-image .
    ```

3.  Run the following command
    ```
    docker run -p 8888:5000 --name cloud-school-image mbaoma/cloud-school-image 
    ```

4.  To confirm if your container was built, run:
    ```
    docker ps -a
    ```

5.  Check if the container runs in your localhost port 8888 by typing ```localhost:8888``` in your browser

![image](https://user-images.githubusercontent.com/49791498/104234555-e2431d00-5453-11eb-870e-fe029cff8b48.png)
*Docker Image*

6.  Push the image to docker hub