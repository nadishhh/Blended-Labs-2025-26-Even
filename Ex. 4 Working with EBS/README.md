# Lab 4 – Working with Amazon Elastic Block Store (EBS)

## Author

* **Name**: NADISH S
* **Register Number**: 212224050023
* **Date of Submission**:17/09/26

# Lab 4 – Working with Amazon Elastic Block Store (EBS)

## Objective

The objective of this experiment is to understand how Amazon Elastic Block Store (EBS) provides persistent block-level storage for EC2 instances. This lab focuses on creating and attaching an EBS volume, formatting and mounting it on an EC2 instance, storing data, and verifying data persistence after instance reboot.


## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* An existing EC2 instance (Amazon Linux 2 preferred)
* Basic knowledge of Linux commands

## Tools Used

* AWS Management Console
* Amazon EC2
* Amazon EBS
* SSH Client (Terminal / PuTTY)


## Tasks Performed

### Task 1: Explore Amazon EBS

Explore the Amazon EBS service through the EC2 dashboard. Observe different volume types such as General Purpose SSD (gp2/gp3), Provisioned IOPS SSD, Throughput Optimized HDD, and Cold HDD.

### Task 2: Create an EBS Volume

Create a new EBS volume in the same Availability Zone as the EC2 instance. Choose an appropriate size and volume type.

### Task 3: Attach EBS Volume to EC2 Instance

Attach the created EBS volume to the running EC2 instance as an additional block device.

### Task 4: Format the EBS Volume

Connect to the EC2 instance using SSH and format the attached volume with a file system (for example, ext4).

### Task 5: Mount the EBS Volume

Mount the formatted volume to a directory in the EC2 instance (for example, /data or /mnt/ebs).

### Task 6: Store Data in EBS Volume

Create files and directories inside the mounted EBS volume and store sample data.


### Task 7: Verify Data Persistence

Reboot the EC2 instance and verify that the data stored in the EBS volume is still available after reboot.


## Workflow (Student Explanation)

1. Explore Amazon EBS (Elastic Block Store) in the EC2 dashboard and understand different volume types such as General Purpose SSD (gp2/gp3), Provisioned IOPS SSD, and HDD-based volumes. These are used for persistent block-level storage.
2. Create a new EBS volume by selecting the required size and type. Ensure the volume is created in the same Availability Zone as the EC2 instance for successful attachment.
3. Attach the created EBS volume to the running EC2 instance as an additional block storage device. This makes the volume accessible to the instance.
4. Connect to the EC2 instance using SSH, format the volume with a file system (e.g., ext4), and mount it to a directory such as /mnt/ebs or /data for usage.
5. Store files in the mounted volume and verify persistence by rebooting the instance. The data remains intact, showing that EBS provides durable and persistent storage.



## Output Screenshots (Attach 3)

### Screenshot 1: EBS Volume Created

<img width="1919" height="909" alt="Screenshot 2026-03-11 154251" src="https://github.com/user-attachments/assets/e1d729d8-f2f4-4b1f-bbf9-f2b02abe99cb" />

### Screenshot 2: EBS Volume Attached to EC2

<img width="1918" height="898" alt="Screenshot 2026-03-11 154356" src="https://github.com/user-attachments/assets/74f459e3-3661-4039-84da-51db92dbbbb9" />

### Screenshot 3: Mounted Volume with Data

<img width="1918" height="902" alt="Screenshot 2026-03-11 155250" src="https://github.com/user-attachments/assets/c3727fec-1eb9-4443-b975-1d442cf26086" />


## Result / Conclusion

This experiment demonstrated how Amazon EBS provides persistent storage for EC2 instances. By creating, attaching, formatting, and mounting an EBS volume, and by verifying data after reboot, the concept of durable block storage in the cloud was clearly understood.
