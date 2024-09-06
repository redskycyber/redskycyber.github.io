---
title: CloudBreach - Breaching AWS (CAWSP) Review
date: 2024-09-05
categories: [AWS, COURSE_REVIEW]
tags: [aws, pentesting, cert, CAWSP]
---

# My Experience with Breaching AWS

![Breaching AWS](assets/img/CAWSP_LOGO.png)

## Overview

The "Breaching AWS" course by CloudBreach offers an immersive dive into AWS security within a simulated environment. Designed for penetration testers, cloud architects, and security engineers, this hands-on course equips you with the tools to uncover and exploit AWS-specific vulnerabilities.

Covering AWS reconnaissance, phishing tactics, exploiting vulnerable services, and security audits, the course provides a comprehensive skill set. Successful completion earns the Offensive AWS Security Professional (OAWSP) badge, demonstrating AWS security expertise.

## Prerequisites

**Knowledge:** A basic understanding of AWS and cloud security fundamentals is expected.  
**Tools:** None required! CloudBreach provides an in-browser VM with all necessary cloud penetration testing tools and lab connectivity. A stable internet connection is the only requirement.

![In Browser VM](assets/img/CAWSP_In_Browser.png)

## Course Material

The course spans 22 attack paths, 17 attack paths, and 26 flags across a variety of lab challenges.

![Course Content](assets/img/CAWSP_Course_Content.png)

Key objectives include:
- AWS Reconnaissance
- AWS Phishing (Device Code)
- Secret Extraction from Secrets Manager, Storage, and Databases
- SNS Data Interception
- Kubernetes Misconfiguration Exploits
- Abusing Container Registry Permissions
- Lateral Movement across AWS Services
- Using Rancher to Gain EKS Pod Access
- Exploiting Misconfigured IAM Permissions
- Enumerating AWS Identity Center Directories
- Lambda Function Exploits
- EC2 Instance Misconfigurations

### AWS Services Covered

- S3
- SSM
- SNS
- Lambda
- DynamoDB
- ECR
- AWS SSO
- IAM
- Secrets Manager
- EBS
- RDS
- EC2
- IMDS
- EKS

## Training Style

The course is broken into self-paced sections, allowing flexibility in speed. Content is accessible on the page, so you can progress as needed.

**Lesson Content:** Introduces background information, definitions, enumeration techniques, and commands, guiding you through each AWS service and exploitation technique.

![Course Lesson](assets/img/CAWSP_BAWS01_Lesson.png)

**Lab:** Provides hands-on objectives that build upon each other, demonstrating real-world exploitation scenarios.

![Course Lab](assets/img/CAWSP_BAWS01_lab.png)

**Lab Solutions:** Offers a step-by-step guide to exploiting the lab environment, including expected commands and output. While solutions are available, it’s recommended to attempt the labs independently first to simulate real-world scenarios and prepare for the exam.

![Course Lab Solution](assets/img/CAWSP_BAWS_Lab_solution.png)

For extended content, the **Breaching AWS+** version includes PDFs and video recordings.

The course structure allows for personalized pacing. I found it easy to move through familiar areas while slowing down for new material. Lab solutions were helpful but only necessary as a fallback. The continuous, evolving scenario with a fictitious company added a layer of realism, as the labs felt connected rather than isolated.

Take a look at the first two unlocked sections to get a sense of the course before purchasing:

- [BAWS 01 – Enumerating S3 Buckets](https://cloudbreach.io/courses/breaching-aws/lessons/step1/)  
- [BAWS 02 – Dumping EBS Secrets](https://cloudbreach.io/courses/breaching-aws/lessons/baws-02-dumping-ebs-secrets/)

## Exam Experience

The exam is an engaging, objective-based challenge that tests everything learned in the course and labs. You have 24 hours to complete it, followed by 24 more hours to submit a report detailing how you compromised the target company.

Exam instructions, including the target company and success objective, are provided 15 minutes before your start time. The exam mirrored the labs, requiring a combination of enumeration, exploitation, pivoting, and escalation.

In my case, I completed the exam in about 6.5 hours, with the report taking another hour and a half. The report is only five pages, so it’s concise yet sufficient to demonstrate your work. You’ll have plenty of time to complete the exam and write the report, though if AWS is new to you, you might take longer.

![Course Exam](assets/img/CAWSP_Exam_info.png)

## Pricing

The course offers three pricing tiers based on the number of lab days and additional content. For most, 30 days of lab time should be enough to complete the objectives and prepare for the exam. Depending on how much study time you have and whether you want the extended "AWS+" material (which includes videos), the tier options are flexible.

[Pricing Information](https://cloudbreach.io/breachingaws/#pricing)

![Course Pricing](assets/img/CAWSP_Pricing.png)

## Overall Experience

I thoroughly enjoyed the "Breaching AWS" course. The content was well-organized, with exploitation techniques building on each other in a realistic environment. The ready-to-go in-browser VM saved setup time, and I picked up valuable techniques to enhance my AWS penetration testing skills. I’d recommend this course for anyone interested in AWS pentesting, whether you’re just starting or looking to advance.

## Tips and Tricks for Success

> - [x] Complete all the labs.  
> - [x] Try the labs on your own before relying on the solutions.  
> - [x] Take detailed notes and screenshots as course access expires after your time window.

{: .prompt-tip }

## Course Link

[CloudBreach - Breaching AWS](https://cloudbreach.io/courses/breaching-aws/)

![Course Completion](assets/img/CAWSP_Completion.png)

## Disclaimer

All opinions are my own. I aim to provide honest and insightful feedback to help guide fellow professionals in choosing valuable resources for career development.
