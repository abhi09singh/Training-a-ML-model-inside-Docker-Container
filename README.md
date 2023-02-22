# Training-a-ML-model-inside-Docker-Container

LINK for detailed article of task : https://www.linkedin.com/pulse/training-ml-model-inside-docker-container-abhinav-singh

🌐  This article is based on TASK-01 of Machine Learning program running under  Linux World MLOps Summer Internship 2021 🌐

Task Description :-
👉 Pull the Docker container image of CentOS image from DockerHub and create a new container

👉 Install the Python software on the top of docker container

👉 In Container copy the date-set file from host to docker container.

👉 Install required libraries required to load ML model

👉 Create and Run the python code for prediction.

=================================================================

STEP : 1

Installing Docker on RHEL8
👉Install docker using “yum install docker-ce” . To check detail about this step check the google Doc link given below:


Checking status of docker whether it is running or not:-
👉“systemctl status docker” command shows the status of docker.

No alt text provided for this image
Pull the Docker container image of CentOS image from DockerHub and create a new container
👉“docker pull centos:8” is used for pulling image.

No alt text provided for this image
👉“docker run -it __name CONTAINERNAME centos:latest” for launching container.

No alt text provided for this image
STEP : 2

Install the Python software on the top of docker container
👉python can be installed using “yum install python3” command.

No alt text provided for this image
STEP : 3

Copying the data set (.csv file) from local host to docker container using which we train our ML model.
👉“docker cp <src> <container_name>:<dest>” is used for copying from local host to container.

No alt text provided for this image
No alt text provided for this image
STEP : 4

Install required libraries required to load ML model :-
👉All required libraries can be installed from the following command: pip3 install <name of library>



No alt text provided for this image
No alt text provided for this image
STEP : 5

Finally create python code for prediction.
👉Below is the python code for our ML model :-

No alt text provided for this image
🔰The Output of our Machine Learning Model :

No alt text provided for this image
Getting above output is the main task of our ML model. (Y=c+wX)

I hope this article helps you in learning something new . I tried my level best to justify each and every point of task .

Thanks For your time for reading 💌
