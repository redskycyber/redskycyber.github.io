---
title: Hacktricks ARTE Course Review
date: 2024-07-22
categories: [AWS, COURSE_REVIEW]
tags: [aws, pentesting, cert, arte]
---

# My Experience with the AWS Red Team Expert (ARTE)

## Overview

![Course Image](assets/img/ARTE_course_image.png)

The ARTE certification is an AWS-focused penetration testing course and training that starts at the very basics and deepens your expertise in AWS security with a comprehensive exploration of advanced concepts. It covers the AWS pentesting methodology, dives into more than 20 common AWS services, and guides you through enumeration techniques/tools, privilege escalation, and playbooks to enhance your skill set.

## Prerequisites

- **Workstation:** Runs AWS CLI.
- **Skills:** Bash and Python are helpful for some enumeration scripts.
- **AWS Account:** Not required but can be handy for troubleshooting and when needing an external account.
- **Mindset:** A willingness to learn, explore, and fully immerse in the technical labs is a MUST.
- **Community:** Join the Hacktricks Discord server for questions and course/exam tickets (you should definitely get over there).

![Discord](assets/img/hacktricks_discord.png)

## Course Material

![Course Content](assets/img/ARTE_course_content.png)

- **Video Lessons:** 20+ Hours
- **Hands-on Labs:** 50+ including blackbox labs (these were my favorites)
- **Exam:** 12 Hours to prove your skills
- **Lab Time:** 60 days

## Services Covered

- IAM - Identity Access Management
- STS - Security Token Service
- KMS - Key Management Service
- Secrets Manager
- S3 - Simple Storage Service
- EC2 - Elastic Cloud Computing
- ELB - Elastic Load Balancer
- SSM - Simple Systems Manager
- Lightsail
- Lambda
- API Gateway
- EFS - Elastic File System
- RDS - Relational Database Services
- DynamoDB
- ECR - Elastic Container Registry
- ECS - Elastic Container Service
- Elastic Beanstalk
- CodeBuild
- SQS - Simple Queue Service
- SNS - Simple Notification Service
- Cognito

These are the top services you’ll find in most enterprise environments of AWS, chosen to give you a solid base with the most popular services in AWS. Understanding the methodology to perform similar activities with other services you may encounter is crucial. Hacktricks even rewards you with 1 free flag on the final exam if you commit a new privilege escalation technique to the course book, which is pretty cool.

## About the Instructor

![Carlos Polop Martin](assets/img/carlos.png)

Carlos Polop Martin is a wizard in pentesting and red teaming. You may know him from tools like PEASS-ng (Privilege Escalation Awesome Scripts SUITE), including linpeas and winpeas, which are incredible scripts for privilege escalation techniques. He is also known for Hacktricks, an amazing open-source repository and playbook for all things pentesting and offensive security. Their cloud.hacktricks.xyz site is filled with tons of cloud pentesting methodology, enumeration techniques, privilege escalation, and playbooks that act as the backbone for this course and training.

## Training Style

![Training](assets/img/arte_course_includes.png)

![Slides](assets/img/ARTE_Slides_example.png)

- **Video Recording:** Carlos walks through slides covering background, enumeration techniques, privilege escalation techniques, and persistence mechanisms for each main service.
- **Physical Copy of Slides:** Includes easy copy/paste of basic commands.
- **Reference Links:** To Cloud.hacktricks.xyz for additional key areas for each service.
- **Labs:** One to several labs for each course section, where you can practice and implement the techniques covered. Labs vary from introductory and simple (under 15 minutes) to complex challenges that may take a couple of hours.
- **Hints:** For completing each lab, linking to relevant sections of the cloud.hacktricks.xyz site. It’s recommended to search for the correct sections yourself based on the permissions discovered in the labs before relying on the hints.

I highly recommend going through ALL the labs over the 60 days you have access, tackling as many as you can from the start to ensure you have enough time to become fully familiar with the course content. Revisit any labs that challenged you, and ask questions either to the Hacktricks community or through their course ticketing on Discord to make sure all the labs are completed.

## Exam Coverage

Everything on the exam is covered in the course, but there are some areas where you’ll need to dive a little deeper on your own. The methodology is cemented in your process: discover or use provided credentials, enumerate current permissions, enumerate the service where you have permissions, search for privilege escalation vectors of the services, execute. This same methodology is needed to tackle the black box labs and final exam.

![Exam](assets/img/arte_exam.png)

## Black Box Labs

![Black Box Labs](assets/img/black_box_labs.png)

The black box labs are covered in their own section of the course 3.2, including Black Box (I), Black Box (II), and Black Box (III). Completing this section is highly recommended as it’s the most real-world and sets you up for success in the exam. For example, you may be given a URL to web infrastructure hosted on AWS and told to “pivot and escalate privileges,” and that’s it—no hints. These labs require general pentesting skills but revolve around cloud-hosted infrastructure, reflecting real-world experience.

If you get stuck, submit a lab ticket! The community is very supportive in giving subtle nudges and helping you reach the end solution on your own. Instructor ticket support is also very helpful. Sometimes just typing out a question and rewriting the steps you’ve taken can make the real path clear. Several tickets I submitted were followed up with “Never mind, I figured it out” only minutes after asking.

## Price

![Course Price](assets/img/course_price.png)

- **Cost:** 1099 Euro or close to 1200 USD depending on the conversion rate.
- **Value:** Although this course is pricier compared to others, it’s extremely well worth it. Especially if you can use it as part of your employer's training budget or wait for a promotional discount. The high-quality content and comprehensive coverage make it a valuable investment for becoming proficient in AWS pen testing.

## My Experience Overall

I started the AWS Hacktricks course with a deep interest in AWS pen testing and some prior experience, which made the course very intriguing. With several years of traditional pen testing under my belt, I was familiar with standard methodology and the “try harder” mentality. However, many aspects of cloud services were new to me. Interacting with these services on a technical level made a significant difference in my understanding. I firmly believe in hands-on practical certifications for this reason, and this course provided just that.

There are no knowledge prerequisites, but having a general understanding of AWS services, familiarity with the AWS CLI, and experience with tools like Scout Suite and Prowler for identifying security misconfigurations was helpful. The repetition of methodology throughout the labs solidified the process, boosting my confidence in enumerating and exploiting common AWS services, and tackling the challenges of the black box labs and final exam.

## My Exam Experience

The exam for this course was an excellent black box challenge that brought everything together in a fun and real-world experience. I kept good notes throughout the course, prepared by organizing them by section, and created a cheat sheet of the most common enumeration commands that I ran throughout the labs. You can schedule your exam for up to a year after you purchase the voucher, so there is plenty of time to get prepared. I found it best to schedule a week after my lab time ran out to give myself a little break, but not so much that I would forget all that I'd learned. The exam deployment was smooth, and the objectives appeared once the lab spun up, just a few minutes after my scheduled lab time. I was given 12 hours, with a countdown timer, and three fields to submit the flags for the environment. The flags are generically named but give you just enough info to infer what steps you should be taking next. I got the first flag within the first hour but struggled heavily with the second and third until the final couple of hours. A combination of nerves and not taking proper breaks limited some of my view in the exam, but I was happy to pull off a photo finish and submit all the flags in time. The exam felt very real-world and tested a few concepts from the course that strung together nicely. It was a great challenge, and I really enjoyed the experience. If you follow the methodology of the course, enumerate thoroughly, and complete all of the labs while taking good notes, you should do just fine with the final exam.

## Tips and Tricks for Success
> - Do these!
  - [x] Dive into the labs early and complete ALL of them, especially the Black Box labs
  - [x] Join the Hacktricks Discord for hints and support
  - [x] Take good lab notes and create an organized cheat sheet for the exam
  - [x] Enumerate thoroughly during the exam, and take breaks throughout
{: .prompt-tip }

## Conclusion

I genuinely loved this course. It solidified my confidence in AWS, and I can now discuss methodologies and attack vectors with ease. This path of taking the ARTE certification has significantly enhanced my AWS pen testing journey, and I plan to explore other certification paths for GCP and Azure as well. In my opinion, this is the gold standard for AWS pen testing certifications, but I'm always looking for more training opportunities in the near future.

If you have any questions about my experience with this course or my cloud pen testing journey, feel free to reach out to me on [LinkedIn](https://www.linkedin.com/in/mike-dame/).

![Course Completion](assets/img/Course progress.png)

![Cert Image](assets/img/arte_certificate_of_completion.png)

## Course Link
Start your own ARTE training experience here:
[ARTE Training](https://training.hacktricks.xyz/courses/arte)

## Disclaimer
This is not a sponsored post. All thoughts and opinions here are my own. I strive to provide genuine and impactful feedback for the cyber community to guide you toward the best resources for your career growth.

