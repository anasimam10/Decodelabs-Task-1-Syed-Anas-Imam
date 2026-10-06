# Cloud Portfolio — AWS S3 Static Website Hosting

> **Project 1 | Decode Labs Internship**  
> Created as my first project for the Decode Labs Internship to demonstrate static web hosting and serverless cloud deployment using Amazon Simple Storage Service (Amazon S3).

---

## 🔗 Live Website

**Live URL:** [Syed Anas Imam | CS Undergraduate & Systems/AI Trainee](http://anascv1.s3-website-us-east-1.amazonaws.com/)

---

## 📌 Project Overview

* **Objective:** Deploy a modern, responsive personal developer portfolio using Amazon S3 Static Website Hosting without provisioning traditional web servers (like EC2 or Apache/Nginx).
* **Tech Stack:** Amazon S3, HTML5, CSS3, JavaScript (vanilla).
* **Highlights:**
  * Clean, responsive dark-themed UI showcasing engineering projects, skills, and experience.
  * Direct PDF resume download hosted on S3.
  * Custom 404 error routing via `error.html`.

---

## ⚙️ S3 Configuration & Evidence

The bucket `anascv1` was configured in the `us-east-1` region with Static Website Hosting enabled, pointing to `index.html` as the index document and `error.html` as the error document.

![AWS S3 Static Website Hosting Setup](assets/aws-s3-hosting-setup.png)

---

## 🔐 S3 Bucket Policy

Public read access was granted through the following bucket policy:

```json
{
  "Version": "2012-10-17",
  "Statement": [
    {
      "Sid": "PublicReadGetObject",
      "Effect": "Allow",
      "Principal": "*",
      "Action": "s3:GetObject",
      "Resource": "arn:aws:s3:::anascv1/*"
    }
  ]
}
```

---


## 👤 Author

**Syed Anas Imam**  
Computer Science Undergraduate | Systems & AI Trainee  
* [LinkedIn](https://linkedin.com/in/syed-anas-imam-133681323) • [GitHub](https://github.com/anasimam10) • [Portfolio](http://anascv1.s3-website-us-east-1.amazonaws.com/)
