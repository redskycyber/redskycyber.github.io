---
title: Hack The Box Blacksy Cloud Labs - Hailstorm (AWS) Review  
date: 2024-11-13 
categories: [AWS, COURSE_REVIEW]
tags: [aws, pentesting, lab, cert]  
---

# My Review of the BlackSky Hailstorm AWS Lab from Hack The Box

![Hailstorm Lab](assets/img/HTB/hailstormlogo.png)

**Hailstorm** is one of three advanced Cloud Labs from **Hack The Box**, offering hands-on hacking experience in a simulated AWS enterprise environment. This lab focuses on real-world AWS attack paths, common misconfigurations, and privilege escalation techniques, providing valuable practice for those pursuing AWS pentesting expertise. You'll engage in a progressive exploitation journey, where situational awareness in AWS is key. Flags guide you through each stage, but the responsibility of compromising the environment and reaching the objective is entirely on you.

![Hailstorm Lab](assets/img/HTB/1_hailstorm_overview.png)

## Overview
Hailstorm is exclusively available to users within the HTB Enterprise Platform. Each user receives their own private instance, along with VPN access and a Pwnbox click-and-play virtual machine, preloaded with essential tools and accessible directly from your browser.  

You'll begin with a brief scenario outlining a company's AWS infrastructure, where your task is to conduct a cloud security assessment, starting with an external IP address.

Within your lab, you can input discovered flags, tracking your progress through a list of sequential flags with subtle hints in their titles pointing to the next area of compromise.

![Introduction](assets/img/HTB/2_hailstorm_introduction.png)

## Prerequisites

- An HTB Enterprise account with a Cloud Labs subscription or Ultimate pricing plan.
- VPN or Pwnbox connection. This comes with unlimited instances within the HTB Enterprise Platform and makes it convenient to connect to the target environment and work on a lab on the go.
- An AWS account (free tier sufficient for one exploit).
- Intermediate familiarity with AWS pentesting and exploitation methods (This is a CTF-style lab focused on self-guided exploration rather than step-by-step instructions, so a problem-solving mindset and persistence are essential.)
- Familiarity with network discovery (nmap), network traversal (SSH), and some web exploitation techniques relevant to AWS exploitation.

![Pwnedbox](assets/img/HTB/3_pwnedbox.png)

![Pwnedbox2](assets/img/HTB/4_pwnedbox.png)

## Lab Objectives

The Hailstorm scenario comprises 15 progressively challenging flags within the AWS environment, each earning points that hint at difficulty levels. A progress bar at the top of the lab page fills in as you capture each flag, which follows the naming convention `BLACKSKY{flag_is_here}`.

As you work through the environment, expect to traverse multiple VMs, gather credentials, escalate privileges, and exploit various AWS services to capture all 15 flags.

![Progress bar](assets/img/HTB/5_progressbar.png)

Upon completing all of the flags, you will have earned the following learning outcomes:
- AWS enumeration
- Exploitation of serverless applications
- Exploiting misconfigurations
- Lateral movement
- Local privilege escalation
- Mitigations and best practices
- Situational awareness
- Web application and API exploitation

![Flags](assets/img/HTB/6_flags.png)

## Services Covered

Expect to encounter many services typical of an AWS environment, including:
- AWS Services: S3, Instance Metadata Service (IMDS), EC2, API Gateway, IAM, ECR, Secrets Manager, DynamoDB, SSM, Lambda, Elastic Beanstalk, SageMaker
- Additional Technologies: Git, Docker, Jenkins

## Lab Style

This lab is a self-guided experience, making it similar to a black-box penetration test. If needed, labs include write-ups as guided solutions to help understand the attack paths and help users get unstuck when completing the scenario. These can be enabled by the administrator within settings. Hack The Box Enterprise Lab support is also available for questions and troubleshooting. Their responsive assistance can be valuable if you get stuck.

## Access

Access to BlackSky Cloud Labs requires an Enterprise account, and Hack The Box pricing varies based on enterprise enrollment. For a full demo and to get in touch with the Hack The Box team, you can fill out a contact form located here: [Contact HTB Form](https://hacktheboxltd.sjv.io/e14gE1) 

Or sign up for a 14-day free trial of the platform here: [14-day Free Trial](https://enterprise.hackthebox.com/create-company)   

For other training on the Hack The Box platform, visit: [Hack The Box Training](https://hacktheboxltd.sjv.io/QjO4na)

![Sales](assets/img/HTB/7_talk_to_sales.png)

## My Overall Experience

I thoroughly enjoyed my time with Hailstorm. For those with AWS pentesting experience, it’s an excellent test of skills and methodologies in a black-box environment. The challenge of working across multiple VMs and AWS services, and the need to demonstrate proficiency in a range of skillsets, makes it a rewarding experience. This lab might be challenging for beginners, who may benefit from additional training before attempting Hailstorm, but it’s a strong addition to any AWS pentester’s journey. For me, it introduced new nuanced techniques, reinforced previous ones, and provided a well-rounded experience that I highly recommend.

## Tips for Success
> - Do these!
- [x] Prepare for a black-box challenge by mastering AWS enumeration, exploitation, and privilege escalation techniques beforehand.
- [x] Practice enumerating IAM permissions and researching service-specific attacks.
- [x] Don’t hesitate to ask for guidance from Enterprise Support if you’re stuck.
- [x] Approach Hailstorm as a robust test of your AWS pentesting skills rather than a guided learning module.
{: .prompt-tip }

![Cert](assets/img/HTB/8_certificate.png)