# Devops - Learning Docker:

## What are Containers?

Containers are lightweight, portable units that are used to run applications. They bond one applications with all its dependencies, ensuring it runs consistently across diferent environments. It provides isolation and improves resource efficiency. Using containers can streamline the deployment processes, ensuring the applications are reliable and portable. 

## What is Docker? 

Docker is an open platform for developing, shipping and running applications in containers. It simplifies the process of managing containers, making it easier to build, deploy and run applications. Docker is a game changer in modern development and operations. It simplifies deployment by ensuring consistent environments, improves efficiency with lightweight and fast starting containers. It enhances collaboration by making it easy to share environments and it streamlines workflows by integrating seamlessly with CI/CD pipelines. By adopting Docker, teams can increase their productivity, reduce errors, and ensure smoother development and deployment process

## Images & Containers

Images are templates for creating containers. An image is a "snapshot of an application at a certain point in time". Images are immutable, meaning they do not change once created. The only way to change an image is to recreate it as new. The immutability ensure that the application runs consistently no matter where it is deployed. Images are created in a docker file. It contains a series of instruction that Docker uses to create an image from. 

Contianers are the running instances of an image and the image which are napshots of an application. Containers are what you intereact with. They run the application and you can start, stop & modify them as needed

## FAMOUS Interview Q: VMs vs Containers

Both containers and virtual machines offer ways to run applications in isolated environments but they do so in fundementally different ways. 

Containers - are lightweight, thye share the host operating system and they start up quickly, which makes them ideal for modern cloud native applications. 

Virtual Machines - Provide strong isolation and include a full operating system which makes them suitable for applications requiring a full isolation or running different OS types on the same host. 

## Understanding Dockerfile

`FROM` : Specifies the base image to use for the Docker image. The base image serves as the foundation for the application. 

`RUN` : Executes commands in the container. This instruction is used to install packages, update dependencies etc. 

`COPY` : Copies files from the host machine into the container.

`WORKDIR` : Sets the working directory for subsequent instructions. This ensures that the command runs in the correct                    directory within the container.

`CMD` : Specifies the command to run when the container starts.

## Docker Compose

Docker Compose helps you run multiple docker containers together. Docker Compose is a critical tool in Devops for several reasons. It simplifies the development and testing process. It ensures consistency across different environments and enhances teamwork by making it easier to share and manage infrastructure setups. With Docker Compose, you can significantly stream on your workflow, reduce errors and foster better collaboration with the team.
