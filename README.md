# Netflix Submission
### Clone the following repository   https://github.com/exit-zero-academy/NetflixMovieCatalog.git
### Clone the following repository   https://github.com/exit-zero-academy/NetflixFrontend.git
## Create EC2 instances
![image](https://github.com/user-attachments/assets/e6fc99f9-4007-4ae0-94ee-437b8fbf5fc7)
## Edit inbound rules and open ports
![image](https://github.com/user-attachments/assets/44f096a3-9535-4367-a09c-f444c4e7bf9c)

## Create DNS using route 53
![image](https://github.com/user-attachments/assets/1c634161-ab34-43ac-bbb4-97cc02143b28)
1. Build a Docker image of the following app: https://github.com/exit-zero-academy/NetflixFrontend.  and   https://github.com/exit-zero-academy/NetflixMovieCatalog.git 

   This is a Node.js app. In the README you'll find instructions to build and run the app. 
   Use it as a baseline for you Dockerfile instructions. 

2. Push the images to container registry (either DockerHub or ECR). 
3. Deploy your image in a fresh new `*.nano` Ubuntu EC2 instance (pull the image and run it). 
4. In your Nginx instance, create a new `server` which routes traffic to your Netflix Frontend app. The app should be accessible from your domain, e.g.: http://netflix.devops-days-upes.com.



![image](https://github.com/user-attachments/assets/c303069e-7967-4909-be2c-ec435cb8b68b)

## Objectives

- **Deploy a microservices architecture** using **EC2 instances**, consisting of:
  - **Nginx**: Acts as the HTTP engine and reverse proxy.
  - **NetflixFrontend**: A **Node.js** web application serving as the frontend.
  - **NetflixMovieCatalog**: A **Flask-based API** for handling the movie catalog.

## Deployment Requirements

- **Use Docker containers** for all services** to ensure consistency and portability.
- **Access the service** via a domain name that is registered and managed using **AWS Route 53**.
- **Deploy a highly available architecture** by:
  - Running multiple instances of the **NetflixFrontend** service.
  - Configuring **Nginx** to function as a load balancer, distributing traffic across multiple frontend instances.
