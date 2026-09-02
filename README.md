# CLOUD-STORAGE-CREATION-S3-AND-LAUNCHING-AN-EC2-INSTANCE-IN-AWS-

# Aim

To create an Amazon S3 bucket for cloud storage and launch a virtual machine using
Amazon EC2 in the AWS Management Console.

# Procedure

# Part A – Creating an Amazon S3 Bucket

## Step 1
Open the AWS console.

URL: https://aws.amazon.com/console/

## Step 2
Log in using the following method:
 Click Sign in using root user email.
 Enter the registered email address.
 Enter the AWS password.
 Complete the verification process.
Output

## Step 3
Type S3 in the search box.

## Step 4
Click Amazon S3.

## Step 5
Click Create bucket.

## Step 6
Enter the following details.
Parameter Value
Bucket type General purpose
Bucket name student-cloud-storage-001
AWS Region Asia Pacific (Mumbai)

## Step 7
Leave the remaining settings unchanged.

## Step 8
Click Create bucket.

## Step 9
Click Upload.

## Step 10
Upload the following files:
 PDF file
 Word document
 Image file
Example
student-cloud-storage-001
│
├── Cloud.pdf
├── Assignment.docx
├── Image.jpg
└── Notes.pdf

# Part B – Launching an Amazon EC2
Instance

## Step 1
Type EC2 in the AWS search bar.

## Step 2
Open the EC2 Dashboard.

## Step 3
Click Launch instance.

## Step 4
Enter the instance name.
CloudLabVM

## Step 5
Select the operating system.
 Amazon Linux 2023
 Ubuntu Server

## Step 6
Select the instance type.
t3.micro

## Step 7
Create a key pair.
Parameter Value
Key pair name CloudLabKey
Key pair type RSA
Parameter Value
File format .pem

## Step 8
Download the CloudLabKey.pem file.

## Step 9
Configure the network settings.
✅ Allow SSH traffic (Port 22)
✅ Allow HTTP traffic (Port 80)
✅ Allow HTTPS traffic (Port 443)

## Step 10
Set the storage size.
8 GiB

## Step 11
Click Launch instance.

## Step 12
Wait until the status changes.
Pending
 ↓
Running

# Connecting to the EC2 Instance

## Step 1
Open EC2.

## Step 2
Select the instance.

## Step 3
Click Connect.

## Step 4
Select EC2 Instance Connect.

## Step 5
Click Connect.

## Step 6
Execute the following command:
echo "Hello AWS"

## Output
Hello AWS

# Stopping the EC2 Instance

## Step 1
Open EC2.

## Step 2
Select Instances.

## Step 3
Select the running instance.

## Step 4
Click Instance state.

## Step 5
Click Stop instance.
Status
Running
 ↓
Stopping
 ↓
Stopped
# Output

<img width="1513" height="688" alt="Screenshot 2026-09-02 102542" src="https://github.com/user-attachments/assets/2dbffe56-f582-486a-8288-37672b24ebe6" />

<img width="1520" height="691" alt="Screenshot 2026-09-02 102557" src="https://github.com/user-attachments/assets/254eab67-d83b-4c39-b844-e7b476aed6d6" />

<img width="1536" height="721" alt="Screenshot 2026-09-02 102953" src="https://github.com/user-attachments/assets/367446c6-dcf0-4702-8b3f-c9024b5ca794" />

<img width="1533" height="725" alt="Screenshot 2026-09-02 103310" src="https://github.com/user-attachments/assets/03f7e912-f847-46eb-8283-6dd5525eb348" />

<img width="1536" height="723" alt="Screenshot 2026-09-02 103356" src="https://github.com/user-attachments/assets/a67e15e2-d57c-4fb6-8a2a-f79c0aee28e6" />

# Result
The Amazon S3 bucket was created successfully, files were uploaded, an EC2 instance was
launched, and the virtual machine was connected successfully.
