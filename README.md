# AWS-Disaster-Recovery-Setup-for-a-Multi-Tier-Web-App
# Automated AWS Disaster Recovery for a 3-Tier Web Application

### Project Summary
This project demonstrates a resilient, automated disaster recovery (DR) solution for a 3-tier web application built on AWS. The primary goal was to ensure business continuity by deploying a fully functional secondary site in a separate AWS region using Infrastructure as Code. The project concluded with a successful live failover test, proving the DR strategy was effective.

---
### Key Features
* **Automation:** The entire DR environment is deployed automatically using a **CloudFormation** template (`template.yaml`).
* **High Availability:** The architecture in each region uses an **Application Load Balancer** and an **Auto Scaling Group** to ensure the application is self-healing.
* **Multi-Region DR:** A "Warm Standby" strategy was implemented with a primary site in `ap-south-1` and a DR site in `us-east-1`.
* **Managed Database:** **Amazon RDS** was used to provide a reliable and secure database service.

---
### Architecture Diagram
This diagram shows the complete multi-region architecture.

<img width="1024" height="1024" alt="AWS Architecture diagram-DR" src="https://github.com/user-attachments/assets/60fe633f-fc83-4599-9a41-989d42726b99" />


---
### Core Technologies Used
* **AWS CloudFormation (Infrastructure as Code)**
* **Amazon EC2 & Auto Scaling**
* **Application Load Balancer (ALB)**
* **Amazon RDS**
* **AWS CLI**
* **AWS Secrets Manager**

---
### Project Deliverables
* [Disaster Recovery Runbook.docx](Disaster%20Recovery%20Runbook.docx): A step-by-step guide for the failover procedure.
* [RPO&RTO Analysis.docx](RPO&RTO%20Analysis.docx): A full report on the project's test results, challenges, and success criteria.
