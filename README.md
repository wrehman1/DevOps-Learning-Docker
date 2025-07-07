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

## Docker Registries

A Docker Registry is a storage and distribution hub for docker images. It is where images live and not running as containers. It is like an online library for docker images, making them accessible whenever and whereever you need them. Public registry, e.g. Docker Hub is open to everyone. Private registry, e.g. AWS ECR (Elastic Container Registry) is the AWS version of the registry where images are stored. 

## Making Images Lighter: MultiStage Builds

Large images can slow down your deployments. It consumes more bandwidth and requires more storage. Multistage builds in Docker allows you to use multiple from statements in your Dockerfile. The idea for this is to use one stage to build your application and another much lighter stage to create the final stage that will be deployed. This approach allowsyou to discard unnecessary files and dependencies resulting in a much smaller optimised image. By reducing the size of the docker image, you make your deployments faster and more efficient. Smaller images are quicker to pull from a registry, faster to deploy and take up less disc space. 

![image](https://github.com/user-attachments/assets/3855a772-0b67-43a7-9328-ec3e2137f7f5)

![image](https://github.com/user-attachments/assets/f20250b4-f8a9-4252-9552-aff4ef039da9)

## Kubernetes 

Kubernetes is an open source platform designed to automate teh depolyment, scaling and operations of application containers. It takes container management to the next level by providing advance features like container orchestration, automatic scaling and self-healing. These features ensure your application runs smoothly, efficiently, no matter the scale. 

Understanding Kubernetes is essential for modern Devops professionals as organisations increasingly adopt microservices architecture and cloud native technologies.

## Docker Swarm vs Kubernetes

Docker Swarm is easier to use and integrates esamlessly with Docker, making it a great option for smaller, less complex deployments. However, Kubernetes offers more power, flexibility and scalability, making it the preferred choice for large scale enterprise level applications. 

![image](https://github.com/user-attachments/assets/56c896bc-453c-44db-841a-45cdac701c63)

## Why Use Orchestration Tools?

![image](https://github.com/user-attachments/assets/a01413ec-b903-4aed-8772-cc9845c9e6fc)

