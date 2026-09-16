# Lab 3 – Introduction to Amazon Elastic Compute Cloud (EC2)

## Author

* **Name**: NADISH S
* **Register Number**: 212224050023

---

## Objective

The objective of this experiment is to understand the fundamentals of Amazon Elastic Compute Cloud (EC2). This lab focuses on launching and managing a virtual server, understanding instance types and AMIs, connecting to an EC2 instance, monitoring its status, and performing basic instance operations such as start, stop, and terminate.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* Web browser with internet connectivity
* Basic knowledge of Linux commands (optional)

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Key Pair
* Security Group
* SSH Client (PuTTY / Terminal)

---

## Tasks Performed

### Task 1: Explore Amazon EC2 Dashboard

Explore the EC2 service dashboard in the AWS Management Console. Observe the different sections such as Instances, AMIs, Instance Types, Key Pairs, Security Groups, and Elastic IPs.

---

### Task 2: Launch an EC2 Instance

Launch a new EC2 instance using Amazon Linux 2 AMI. Select an appropriate instance type (t2.micro) under the free tier. Configure basic settings such as instance name, key pair, and security group.

---

### Task 3: Configure Security Group

Configure a security group to allow inbound access:

* SSH (Port 22) from your IP address
* HTTP (Port 80) from anywhere (0.0.0.0/0)

This security group acts as a firewall for the instance.

---

### Task 4: Connect to EC2 Instance

Connect to the running EC2 instance using SSH. Use the downloaded key pair and connect via terminal or PuTTY.

For Amazon Linux:

```
ssh -i "keyname.pem" ec2-user@<Public-IP>
```

---

### Task 5: Perform Basic Instance Operations

Perform the following operations from the EC2 console:

* Stop the instance
* Start the instance
* Reboot the instance

Observe the state changes of the instance.

---

### Task 6: Monitor EC2 Instance

Monitor the EC2 instance using the Monitoring tab. Observe metrics such as CPU utilization, network in/out, and instance status checks.

---

### Task 7: Terminate EC2 Instance

Terminate the EC2 instance after completing the experiment to avoid unnecessary AWS charges.

---

## Workflow (Student Explanation)

(Write the steps you followed in your own words)

1. Logged in to the AWS Management Console and opened the **Amazon EC2 Dashboard**.

2. Launched an **EC2 instance** using the Amazon Linux 2 AMI, selected the **t2.micro** instance type, and configured the key pair and security group.

3. Connected to the running instance using **SSH** and performed basic operations such as **stop, start, and reboot** while monitoring its status.

4. After completing the experiment, checked the instance monitoring details and **terminated the EC2 instance** to avoid unnecessary charges.


---

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Dashboard / Instance List

<img width="1913" height="982" alt="ex3 1 clo" src="https://github.com/user-attachments/assets/161d0470-3dfb-4ff0-9a1e-12336db94201" />



---

### Screenshot 2: SSH Connection to Instance

<img width="1186" height="747" alt="ex3 2 clo" src="https://github.com/user-attachments/assets/74fbea1e-7497-421e-9501-b881969f02c9" />


---

### Screenshot 3: Instance Monitoring / Status

<img width="1918" height="983" alt="ex3 3 clo" src="https://github.com/user-attachments/assets/7edbb9f5-a1bb-48c7-922c-812eb613d037" />
<img width="1918" height="983" alt="ex3 4 clo" src="https://github.com/user-attachments/assets/b91cb591-3a94-45e3-8def-7db885eba989" />



---

## Result 

This experiment provided hands-on experience with Amazon EC2 by demonstrating how to launch, connect, manage, and monitor a virtual server in AWS. It helped in understanding the concept of Infrastructure as a Service (IaaS) and how compute resources can be provisioned and controlled on demand in the cloud.
