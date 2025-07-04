
# AWS CloudWatch Agent Setup Guide

## Step 1: Create/Edit CloudWatch Agent Config File

### Config file is in the same repo

```bash
vi /opt/aws/amazon-cloudwatch-agent/bin/config.json
```

---

## Step 2: Stop the CloudWatch Agent (If Running)

```bash
sudo /opt/aws/amazon-cloudwatch-agent/bin/amazon-cloudwatch-agent-ctl -a stop
```

---

## Step 3: Fetch Config and Start the CloudWatch Agent

```bash
sudo /opt/aws/amazon-cloudwatch-agent/bin/amazon-cloudwatch-agent-ctl \
  -a fetch-config \
  -m ec2 \
  -c file:/opt/aws/amazon-cloudwatch-agent/bin/config.json \
  -s
```

---

## Step 4: Check CloudWatch Agent Status

```bash
sudo /opt/aws/amazon-cloudwatch-agent/bin/amazon-cloudwatch-agent-ctl -a status
```

---

## ✅ Notes

- Ensure the EC2 instance has the correct **IAM Role** attached with CloudWatch write permissions.
- Confirm the config file path is correct.
- CloudWatch Agent logs (for debugging) are usually found at:

```bash
/opt/aws/amazon-cloudwatch-agent/logs/
```
