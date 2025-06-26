# 🚨 CloudWatch Alarms - Setup Docs & Scripts

Welcome to the **CloudWatch Alarms Toolkit!** 🎉  

In this repo, I've shared useful documentation, configuration files, and filter patterns that will help you quickly set up **AWS CloudWatch Alarms** for monitoring your infrastructure.

---

## 📂 Repository Contents

| File | Description |
|---- | ---- |
| `cloudwatch-agent-setup-guide.md` | Step-by-step guide to **install and configure the CloudWatch Agent** on EC2 instances. |
| `cloudwatch-metric-filter-patterns.md` | Collection of **ready-to-use Metric Filter Patterns** for ALB, API, and application log monitoring. |
| `config.json` | Sample **CloudWatch Agent configuration file** for collecting CPU, Memory, Disk, and application logs. |

---

## ✅ Use Cases Covered

- Installing and starting the **CloudWatch Agent**
- Setting required **IAM Role permissions**
- Creating **Metric Filters** for error monitoring (4xx, 5xx, etc.)
- Setting up **CloudWatch Alarms** based on log patterns
- Sending notifications via **SNS**

---

## 🚀 Coming Soon: Part 2 Teaser

> In Part 2, we’ll share how we handled a **unique client request** to monitor **Target Group EC2 instance health and events** using a **Lambda-based alarm mechanism!**  
Stay tuned 😎

---

## 👨‍💻 Contributions Welcome!

If you find this helpful or want to add more examples:  
- **Fork the repo**  
- **Raise issues**  
- **Submit PRs**

---

## ⭐ If this helped you, don’t forget to give the repo a ⭐ star!

