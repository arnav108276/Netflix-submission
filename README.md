# Netflix Submission
### Clone the following repository   https://github.com/exit-zero-academy/NetflixMovieCatalog.git
### Clone the following repository   https://github.com/exit-zero-academy/NetflixFrontend.git
## Create EC2 instances
![image](https://github.com/user-attachments/assets/e6fc99f9-4007-4ae0-94ee-437b8fbf5fc7)

## Create DNS using route 53
![image](https://github.com/user-attachments/assets/1c634161-ab34-43ac-bbb4-97cc02143b28)

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
