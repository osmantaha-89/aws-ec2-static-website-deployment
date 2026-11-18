# AWS EC2 Static Website Deployment

## Project Overview
A hands-on Cloud Engineering learning project based on a Clarusway static website exercise. The project demonstrates local website testing, working with an existing Amazon EC2 Linux instance, basic network security configuration, GitHub version control, and public static website hosting.

## Live Demo
[View the redesigned website](https://osmantaha-89.github.io/aws-ec2-static-website-deployment/)

**Current deployment:** GitHub Pages  
**AWS EC2 deployment:** The original Clarusway carousel was verified running on EC2. The redesigned version has not yet been deployed to EC2.

## Technologies
- Amazon EC2 (t2.micro)
- Amazon Linux 2023
- AWS Security Groups
- HTTP and SSH
- HTML, CSS and JavaScript
- GitHub and GitHub Pages
- Visual Studio Code

## Architecture

Visitor → GitHub Pages → Responsive Static Website

Original AWS exercise:

Visitor → Public IPv4 → EC2 Security Group (HTTP port 80) → Linux Web Server → Original Carousel Website

## Work Completed
1. Inspected and tested the original static website project.
2. Created a backup of the original HTML file.
3. Integrated and locally tested a redesigned static website.
4. Checked an existing Amazon Linux EC2 instance.
5. Reviewed inbound security group rules.
6. Restricted SSH port 22 to the current client public IP while retaining HTTP access on port 80.
7. Started EC2 and verified that the original carousel website was accessible using its public IPv4 address.
8. Investigated SSH connectivity and Session Manager access limitations.
9. Stopped the EC2 instance to reduce ongoing compute charges.
10. Created a public GitHub repository and deployed the redesigned website using GitHub Pages.

## Security and Cost Considerations
- SSH access was restricted to a single client IP.
- HTTP access was retained for public website access.
- No private SSH key or AWS credentials are included in this repository.
- The EC2 instance was stopped after verification. Storage charges may still apply.
- The public GitHub Pages deployment is separate from AWS EC2 hosting.

## Current Limitations
- The redesigned website is not yet deployed on EC2.
- SSH access to the existing instance requires further troubleshooting.
- The demonstration currently uses GitHub Pages for public hosting.

## Planned Improvements
- Restore secure administration access to EC2.
- Deploy the redesigned website to the Linux server.
- Add repeatable infrastructure configuration using Terraform.
- Add automated validation and deployment with CI/CD.
- Add monitoring, documentation and deployment verification.

## Learning Approach
This project is part of a practical Cloud and DevOps portfolio development plan. The goal is to progressively build the ability to configure infrastructure, deploy applications, troubleshoot issues and independently reproduce implementations.

## Credits
Based on an original Clarusway training project. The redesigned website template was generated with AI assistance and integrated and tested as part of hands-on learning. AWS configuration review, deployment testing and GitHub publishing were performed through guided practice.
