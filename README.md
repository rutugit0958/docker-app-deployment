
# Dockerized Application (Project 2)

This project demonstrates how to containerize an application using Docker.  
It includes creating Docker files, running the app inside containers, exposing required ports, and ensuring containers auto-start on system reboot.

---

##  Features

- Create Dockerfile to build application image
- Run application using Docker containers
- Expose required ports to access the app
- Configure container to auto-start on reboot
- Simple and beginner-friendly Docker setup

---

##  Tech Stack

- Docker
- Linux
- Application:# Dockerized Application (Project 2)

This project demonstrates how to containerize an application using Docker.  
It includes creating Docker files, running the app inside containers, exposing required ports, and ensuring containers auto-start on system reboot.

---
## 📂 Project Structure

bash

├── Dockerfile
├── app/
│   └── application files
├── README.md


##Dockerfile##

The Dockerfile is used to create a Docker image for the application.
# Example
FROM nginx:latest
COPY . /usr/share/nginx/html
EXPOSE 80
'''


 ##Build Docker Image##

Run the following command to build the Docker image:

docker build -t myapp .
Run Docker Container

Run the container and expose the required port:

docker run -d -p 8080:80 --name myapp_container myapp

 Verify Running Container

Check if the container is running:

docker ps

Access Application

Open your browser and visit:

http://localhost:8080

 Auto-start Container on Reboot

To ensure the container restarts automatically after system reboot:

docker update --restart=always myapp_container


##Verify restart policy:##

docker inspect myapp_container | grep RestartPolicy
'''
 Screenshots

Screenshots added in the screenshots/ folder:

Project structure

Docker image build

Running container

Application output

##Conclusion##

This project demonstrates practical Docker usage including image creation, container management, port exposure, and auto-restart configuration.
It is suitable for DevOps beginners and Docker practice.

##Author##

Rutuja Patil








- 
