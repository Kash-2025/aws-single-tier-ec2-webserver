WS Single-Tier Architecture Deployment
📌 Overview

This project demonstrates the deployment of a single-tier web architecture using AWS.

The solution hosts a static restaurant website on an Amazon EC2 instance running Apache within a public subnet.

🏗 Architecture Flow

User → Internet → Internet Gateway → Public Subnet → EC2 (Apache Web Server)

🛠 Services Used

Amazon EC2 (t2.micro)

Amazon VPC (default)

Internet Gateway

Route Tables

Security Groups

Apache (httpd)

Amazon Linux 2

🔐 Security Configuration

HTTP (Port 80) open to public

SSH (Port 22) restricted to my IP

Principle of least privilege applied

🚀 Deployment Steps

Launched EC2 instance in default VPC

Configured security group rules

Installed and started Apache

Deployed custom HTML webpage

Verified connectivity and routing

📚 Key Learnings

What makes a subnet public

Route table role in internet connectivity

Difference between security groups and routing

Troubleshooting SSH connectivity

⚠ Limitations

Single point of failure

No auto-scaling

No load balancing

🔄 Future Improvements

Add Elastic IP

Add CloudWatch monitoring

Upgrade to multi-tier architecture

Convert deployment to Infrastructure as Code (Terraform)
