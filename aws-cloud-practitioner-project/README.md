#  AWS Cloud Practitioner Lab Project

This project demonstrates hands-on foundational experience using Amazon Web Services (AWS), focusing on two key services: *Amazon S3* and *EC2 (Elastic Compute Cloud)*. The goal is to simulate basic cloud service operations — creating, configuring, accessing, and managing resources — all through the AWS Console and EC2 Linux instance.


##  Step-by-Step Execution

### 1️⃣ AWS Account Creation and Console Access

Created a free-tier AWS account and logged in to the AWS Console successfully.

Screenshot:  
![Account Created](./screenshots/step-01-account-created.png)


### 2️⃣ Navigating the AWS Console

Explored the AWS Console to identify available services such as S3, EC2, IAM, and more.

Screenshot:  
![AWS Console Dashboard](./screenshots/step-02-console-dashboard.png)


### 3️⃣ S3 Bucket Creation

Created an Amazon S3 bucket with default settings (block public access, SSE encryption). This was done in preparation for storing cloud data securely.

 Screenshot of the configuration page:  
![S3 Bucket Setup](./screenshots/step-03-s3-create-start.png)

 Screenshot of successful bucket creation:  
![S3 Bucket Created](./screenshots/step-04-s3-created-successfully.png)


### 4️⃣ EC2 Instance Launch

Launched a free-tier Amazon EC2 instance using *Amazon Linux 2 AMI*, with:
- t2.micro instance type
- Default VPC and subnet
- Auto-generated key pair
- Security group allowing SSH (port 22)

Screenshot:  
![EC2 Launch Settings](./screenshots/step-05-ec2-launch-settings.png)

 Screenshot of running instance:  
![EC2 Running](./screenshots/step-06-ec2-instance-running.png)



### 5️⃣ Connecting to EC2 via Web Terminal

Used the EC2 *Connect* feature (browser terminal) to access the Linux terminal.

Screenshot:  
![EC2 Web CLI](./screenshots/step-07-ec2-connect-cli.png)



### 6️⃣ Running Linux Commands

Executed basic Linux diagnostic commands to understand the EC2 environment:

| Command | Purpose |
|--------|---------|
| whoami | Shows current user |
| hostname | Displays machine name |
| uname | Kernel/system details |
| uptime | Shows system running time |
| df | Disk space usage |

 Screenshots:
- whoami: ![whoami](./screenshots/step-08-whoami.png)
- hostname: ![hostname](./screenshots/step-09-hostname.png)
- uname: ![uname](./screenshots/step-10-uname.png)
- uptime: ![uptime](./screenshots/step-11-uptime.png)
- df: ![df](./screenshots/step-12-df.png)


### 7️⃣ EC2 Termination

After usage, the EC2 instance was *terminated* to avoid AWS charges.

Screenshot:  
![EC2 Terminated](./screenshots/step-13-ec2-terminated.png)



##  What I Learned

- ✅ Creating and configuring cloud resources on AWS
- ✅ Understanding how S3 and EC2 work at a beginner level
- ✅ Navigating cloud service dashboards
- ✅ Running basic terminal commands in a real Linux environment
- ✅ Practicing cost-saving cleanup (terminating instances)

---

##  Author

- *Project Execution*: [Anukwelu Amamachukwu Godson]

## Acknowledgment

This project was carried out through the AWS Skill Builder training platform as part of my foundational cloud computing journey. Special thanks to the AWS Cloud Practitioner Lab for providing a hands-on, practical learning experience.


##  Note

> Always remember to *terminate your EC2 instances and delete unused resources* to avoid unnecessary AWS billing.

