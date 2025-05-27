# 🌐 AWS Serverless Website with DoS Detection & Alert System

This project documents the setup of [Phishy.Cloud](https://phishy.cloud), a personal cybersecurity &amp; cloud portfolio site hosted using GitHub and AWS. In addition to deployment, I implemented a lightweight **Denial of Service (DoS) alert system** using AWS CloudWatch and tested it with ApacheBench (ab).

---

## 📌 Objective

Host a personal cybersecurity &amp; cloud portfolio website using GitHub and AWS Amplify, and implement a basic DoS alerting system to monitor for abnormal traffic patterns.

---

## 🛠️ Tools & Technologies

- GitHub
- AWS Amplify
- AWS CloudWatch
- ApacheBench (ab)
- Bash / Linux
- DNS / Google Domains
- VPN
- HTML, CSS, JavaScript

![Mock](https://www.phishy.cloud/assets/img/proj/mock1.jpg)

---

## 📖 Overview

[Phishy.Cloud](https://phishy.cloud) serves as a centralized portfolio for showcasing my cybersecurity and cloud projects. It also acts as a real-world environment to apply cloud security concepts. This repo outlines the process of hosting the site and deploying an alerting mechanism for potential denial of service attacks.

---

## ⚙️ Implementation Steps

### 1. 📂 Website Content on GitHub
- Created static site files representing my cybersecurity work
- Uploaded the content to a public GitHub repository

### 2. 🚀 AWS Amplify Deployment
- Set up an AWS account
- Connected Amplify to my GitHub repo for CI/CD deployment
- Amplify automatically built and hosted the site on AWS infrastructure

### 3. 🌐 DNS Routing via Google Domains
- Pointed my custom domain `phishy.cloud` to AWS Amplify
- Updated DNS records in Google Domains for seamless routing

### 4. 📈 DoS Alert System via CloudWatch
- Defined thresholds in AWS CloudWatch to monitor for abnormal request spikes
- Created a custom alarm for high-request volume (indicative of a DoS event)

### 5. 🧪 Load Testing with ApacheBench
- Installed `ab` on a Linux VM
- Simulated a DoS-like traffic pattern against the hosted site

### 6. 📬 Alert Verification
- Verified that CloudWatch correctly detected the traffic surge
- Received an email alert confirming the system’s functionality
- CloudWatch dashboard reflected the triggered alarm

![Mock](https://www.phishy.cloud/assets/img/proj/mock2.jpg)

---

## 📉 Challenges & Lessons Learned

While integrating AWS services, I encountered some initial friction around resource linking and metric configurations. AWS documentation was crucial for working through these issues, supplemented by community forums and tutorials that helped build deeper confidence in the AWS ecosystem.

---

## ✅ Conclusion

This project provided hands-on experience with:
- GitHub-hosted content
- AWS Amplify deployment
- Custom DNS configurations
- Basic DoS alerting via AWS CloudWatch

The successful test of the DoS alert system validated the ability to monitor and respond to suspicious traffic. The project also laid the groundwork for future enhancements.

---

## 🚧 Next Steps

Future improvements include:
- Adding a **Web Application Firewall (WAF)** to block brute-force or DoS/DDoS traffic
- Automating IP bans for repeated offenders
- Expanding monitoring rules for other threat patterns

---

## 📎 License

This project is provided for educational purposes under the MIT License.

---

## 🙋‍♂️ Author

Richard Gergely  
[LinkedIn](https://www.linkedin.com/in/richgerg) | [Portfolio](https://phishy.cloud)
