# ***Welcome to the PacMail Deployment Guide!***

Hi there! Welcome to my project. In this guide, I will walk you through deploying the PacMail web application, making it accessible to the public with a domain name. Think of this as a fun journey we'll take together. Let's get started!

---

### Project Overview

PacMail is a web application that allows users to send and receive emails. As a DevOps Engineer, your objective is to deploy this web app so it can be accessed publicly via a domain name. Here's what we'll cover:

- Server Preparation
- Server Setup
- Compose the App
- Create CI/CD Pipeline
- Create Domain Name
- Configure Web Server using Nginx
- Obtain SSL Certificate using Certbot

---

### 1. Server Preparation

First, you need a server that can be accessed publicly. You can use services like Amazon Web Service (AWS) or any other cloud provider. Make sure your server is up and running!

### 2. Server Setup

- Install Docker & Docker Compose to run and manage your application. You'll need to install both on your server.

- Install Nginx as your web server and to help manage web traffic with a reverse proxy.

- Firewall Configuration: To ensure the application is accessible, you'll need to configure your firewall to allow traffic on necessary ports (HTTP, HTTPS, and SSH) on your server.

### 3. Compose the App

You can use Docker Compose to deploy PacMail. This tool simplifies managing the different parts of your application (frontend, backend, and database) easily. Check out my code walkthrough:
[Click Here](https://github.com/Rico-febrian/PacMail-project/blob/main/docker-compose.yaml)

### 4. Create CI/CD Pipeline

Setting up a CI/CD pipeline ensures your code is always tested, built, and deployed automatically. This involves:

- Continuous Integration: Building, testing, and merging code changes.

- Continuous Delivery: Pushing our Docker images to your Docker Hub.

- Continuous Deployment: Deploying and running the app on your server.

You can use GitHub Actions or any other tools for automating these steps. Check out my code walkthrough:
[Click Here](https://github.com/Rico-febrian/PacMail-project/tree/main/.github/workflows)

### 5. Create Domain Name

To make the app accessible via the internet, you'll need to register a domain name. Services like Hostinger or any other domain registrar can help you with this. Point your new domain to your server's public IP address.

### 6. Configure Web Server using Nginx

Once you have your DNS set up, you need to configure Nginx to act as a reverse proxy. This will forward traffic from your domain to the correct parts of your application (frontend and backend).

### 7. Obtain SSL Certificate using Certbot

Finally, you need to secure the application using SSL. Certbot is a great tool to obtain and install SSL certificates for your domain easily.

---

## Conclusion

And that's it! You've successfully deployed the PacMail web application and made it publicly accessible via a domain name. This project has helped you practice web app deployment, Docker containerization, CI/CD pipeline setup, and Nginx configuration.

If you have any questions or need further assistance, feel free to reach out. Happy deploying!
