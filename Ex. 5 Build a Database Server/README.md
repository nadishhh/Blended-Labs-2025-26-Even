# Lab 5 – Build a Database Server (AWS)

## Author

* **Name**: NADISH S
* **Register Number**: 212224050023

---

## Objective

The objective of this experiment is to understand how to deploy and configure a database server in AWS. This lab focuses on launching an EC2 instance, installing a database management system (DBMS), configuring basic database settings, creating a sample database, and validating connectivity to the database server.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* An existing VPC and EC2 knowledge (from previous labs)
* Basic knowledge of Linux commands and SQL

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Security Groups
* SSH Client (Terminal / PuTTY)
* MySQL / MariaDB / PostgreSQL (any one)

---

## Tasks Performed

### Task 1: Launch EC2 Instance for Database Server

Launch a new EC2 instance using Amazon Linux 2 AMI. Select an appropriate instance type and configure key pair and security group.

---

### Task 2: Configure Security Group for Database Access

Modify the security group to allow:

* SSH (Port 22) for remote access
* Database port (e.g., MySQL – 3306 or PostgreSQL – 5432)

---

### Task 3: Connect to EC2 Instance

Connect to the EC2 instance using SSH from your local machine.

---

### Task 4: Install Database Server

Install a database server software such as MySQL, MariaDB, or PostgreSQL on the EC2 instance using package manager commands.

---

### Task 5: Start and Configure Database Service

Start the database service and configure basic settings such as root password and user privileges.

---

### Task 6: Create a Sample Database

Create a sample database and a table inside it. Insert a few records into the table.

---

### Task 7: Test Database Connectivity

Test the database server by connecting to it locally or remotely and performing basic SQL queries.

---

## Workflow (Student Explanation)

1. First, a security group named DB Security Group was created to allow the web server to connect to the database using port 3306 (MySQL).
2. A DB Subnet Group was created with subnets from two Availability Zones to allow the database to run in a Multi-AZ environment for high availability.
3. A MySQL RDS instance named lab-db was created with the database name lab, username main, and password lab-password.
4. The database was associated with the DB Security Group and the Lab VPC so that the web server can securely connect to the database.
5. The web application running on the EC2 server was opened using its IP address, and the RDS endpoint, database name, username, and password were entered to interact with the database.
---

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Instance for Database Server

<img width="1271" height="581" alt="image" src="https://github.com/user-attachments/assets/25587a1e-cf9a-4bb6-82bb-19e7852d1c86" />

---

### Screenshot 2: Database Service Running


<img width="1258" height="576" alt="image" src="https://github.com/user-attachments/assets/37530d42-f186-457d-af27-9d9a6e250d06" />


---

### Screenshot 3: Sample Database and Table

<img width="1283" height="727" alt="image" src="https://github.com/user-attachments/assets/86fbd58c-f4c8-408f-9654-14dac60374ef" />


---

## Result

This experiment demonstrated how to build a database server in AWS using an EC2 instance. By installing and configuring a DBMS, creating a sample database, and testing connectivity, the fundamentals of hosting and managing a cloud-based database server were underst
