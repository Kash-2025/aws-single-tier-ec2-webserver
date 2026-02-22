Built and Deployed a Single-Tier Architecture on AWS
As part of developing my cloud engineering foundations, I designed and deployed a working single-tier architecture on AWS.
Hypothetical Real-Life Scenario
A small local restaurant needs a simple public website to display opening hours and a daily menu — no database, no complex backend, just a lightweight and cost-effective solution.
🔹 Architecture Flow
User → Internet → Internet Gateway → Public Subnet → EC2 (Apache Web Server)
🔹 What I Implemented
Launched an Amazon Linux EC2 instance (t2.micro)
Used a public subnet within the default VPC
Verified route table configuration (0.0.0.0/0 → Internet Gateway)
Configured security groups:
HTTP (80) open to the public
SSH (22) restricted to my IP
Installed and configured Apache on Linux
Deployed a custom static HTML “restaurant menu” page
🔹 What This Strengthened
This project helped solidify my understanding of:
What makes a subnet truly “public”
The role of route tables vs security groups
How traffic flows from the internet to an EC2 instance
🔹 Key Takeaway
Single-tier architecture is simple and cost-effective, but introduces a single point of failure — if the EC2 instance fails, the entire site becomes unavailable.

This task really helped me visualise how the different components within a VPC work together — from route tables directing traffic, to security groups controlling access, and how an Internet Gateway enables public connectivity.
Building it hands-on made the flow of traffic much clearer than just reading about it.
