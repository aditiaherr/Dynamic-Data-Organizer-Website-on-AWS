# Dynamic Data Organizer Website on AWS

A dynamic data organizer web application deployed on **AWS Cloud Infrastructure**, offering scalable, reliable, and secure solutions for data management. Users can register, upload files, and manage data through an interactive website, leveraging AWS services like EC2, S3, and RDS.

---

## 1. Introduction

### Purpose of the Project
The goal of this project is to deploy a web application on AWS to allow users to register, upload files, and organize data dynamically. Utilizing AWS services, this project ensures **scalability**, **reliability**, and **cost-efficiency** for hosting modern web applications.

### Importance of Cloud Hosting
Cloud hosting revolutionizes application deployment by offering scalability, flexibility, and reduced infrastructure costs. AWS provides services that automatically scale with demand, ensuring secure and efficient operation of web applications.

### Project Scope
The project involves deploying a website on AWS with:
- **EC2 (Elastic Compute Cloud)**: Hosting the website.
- **RDS (Relational Database Service)**: Managing structured user data.
- **S3 (Simple Storage Service)**: Storing uploaded files securely.

---

## 2. Problem Statement

This project addresses common challenges in hosting dynamic websites:
- **Cost Efficiency**: Leverages AWS Free Tier to minimize hosting costs, ideal for startups and small-scale deployments.
- **Data Management**: Uses **MySQL on RDS** for structured data storage and management.
- **Scalability**: AWS's architecture supports seamless scaling as user demand grows.
- **Security**: Implements AWS **security groups** and controlled permissions for secure user data handling.

---

## 3. Architecture

The architecture combines several AWS services to create a cohesive and secure platform:

1. **EC2 Instance**:
   - Hosts the website.
   - Handles user requests and connects to S3 and RDS.

2. **S3 Bucket**:
   - Stores uploaded files securely.
   - Ensures efficient data retrieval and organization.

3. **RDS (MySQL)**:
   - Stores structured user and operations data.
   - Provides reliable and scalable database management.

4. **Security Groups**:
   - Protect HTTP, HTTPS, and SSH access to the EC2 instance.
   - Restrict database access to authorized connections.

---

## 4. AWS Services Used

### 1. Amazon EC2 (Elastic Compute Cloud)
- **Instance Type**: T2.micro (Free Tier eligible).
- **Purpose**: Hosts the website backend and frontend.
- **Features**: Start/stop control, scalable resources.

### 2. Amazon S3 (Simple Storage Service)
- **Purpose**: Stores files uploaded by users.
- **Security**: Controlled access using bucket permissions.

### 3. Amazon RDS (Relational Database Service)
- **Instance Type**: db.t4g.micro (Free Tier eligible).
- **Purpose**: Hosts a MySQL database to manage user and operations data.

### 4. AWS Security Groups
- **Purpose**: Protect incoming/outgoing traffic to EC2 and RDS.
- **Features**: Restrict database access to the EC2 instance.

---

## 5. Configuration of AWS Services

### 1. Setting Up EC2 Instance
- Launch a new EC2 instance using Amazon Linux AMI.
- Configure security groups to allow **HTTP**, **HTTPS**, and **SSH**.
- Assign a public IP for website access.

### 2. Setting Up S3 Bucket
- Create a new S3 bucket.
- Configure permissions for secure file upload/download.

### 3. Setting Up RDS (MySQL)
- Launch an RDS instance with MySQL.
- Configure security groups to restrict access to EC2.
- Create tables for:
  - **Users**: Stores registration data (name, email, password).
  - **Operations**: Logs user actions.

---

## 6. Deployment of Web Application on Cloud

### Website Deployment on EC2
- Host the website using **Apache** or **NGINX**.
- Deploy code to the EC2 instance.

### Connecting EC2 with RDS
- Use MySQL to interact with the database for user registrations and data operations.

### Integrating S3 with EC2
- Use AWS SDK to upload/retrieve files to/from S3.

### Public IP Access
- Users access the website via the **EC2 public IP**.

---

## 7. Results

- **Successful Deployment**: Application deployed effectively on AWS Free Tier.
- **Data Management**: Structured storage using MySQL on RDS.
- **Dynamic Features**: Interactive file operations and data management.
- **Resource Control**: Flexible start/stop options for the EC2 instance.
- **Security**: AWS security groups protect user data and access.

---

## How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/aditiaherr/Dynamic-Data-Organizer.git
   cd Dynamic-Data-Organizer

