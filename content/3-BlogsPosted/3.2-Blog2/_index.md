---
title: "Blog 2"
date: 2026-11-24
weight: 1
chapter: false
pre: " <b> 3.2. </b> "
---

# WHAT IS EC2 & COMPUTE COST OPTIMIZATION FOR SMALL AND MEDIUM PROJECTS ON AWS?

When moving applications to AWS, Amazon EC2 is often the most familiar service—yet also one of the fastest ways to burn through a budget if instance types are chosen by guesswork. For small and medium projects, you can save significantly while maintaining steady performance by following a few straightforward principles below.

### 1. Choose the Right Pricing Models

Instead of defaulting to On-Demand for everything (pay-as-you-go flexibility, but the highest unit rate), consider combining:

* **On-Demand Instances:** Ideal for early development, short-term experiments, or workloads with unpredictable traffic.
* **Savings Plans / Reserved Instances:** If your project runs steadily 24/7 and you plan to keep it running for at least 1 year, committing to consistent usage lowers costs substantially compared to On-Demand.
* **Spot Instances:** Take advantage of spare AWS capacity at a steep discount. Well-suited for background jobs, batch processing, test/CI-CD pipelines, or fault-tolerant workloads that can handle sudden interruptions.

### 2. Avoid Over-Provisioning (Right-Sizing)

A common mistake for beginners is picking an oversized instance "just to be safe," leaving actual CPU and RAM utilization below 15–20%.

* Start with a right-sized instance (e.g., `t3` / `t4g` families for small web apps or internal APIs) and monitor metrics with **Amazon CloudWatch**.
* Consider **AWS Graviton** processors (ARM-based architecture such as `t4g`, `m7g`), which typically deliver better price-performance than comparable x86 instances.

### 3. Turn Off Idle Resources

For Dev / Staging / Test environments, teams usually work during business hours:

* Turning off instances outside working hours and on weekends can cut runtime from ~730 hours/month down to roughly 180–200 hours/month.
* You can use **AWS Instance Scheduler** or combine **Amazon EventBridge + AWS Lambda** to automatically start and stop EC2 instances on a schedule.

### 4. Consider Serverless for Non-Continuous Workloads

You don't always need an EC2 instance running 24/7. If your project has low-traffic APIs, webhooks, or short scheduled tasks, moving to **AWS Lambda** (billed per request and execution duration in milliseconds) keeps costs near zero when there is no traffic.

### Summary

Cost optimization on AWS isn't about cutting corners at any cost—it's about paying accurately for what your system actually uses. By reviewing utilization regularly, picking the right Pricing Model, and automatically stopping test environments off-hours, your small project can save a meaningful amount of budget every month.

**References:**
1. AWS Documentation, Amazon EC2 billing and purchasing options — <https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/instance-purchasing-options.html>
2. AWS Documentation, Choosing a purchasing option for Amazon EC2 — <https://docs.aws.amazon.com/decision-guides/latest/decision-guides/ec2-purchasing-options-aws-how-to-choose.html>
3. AWS Solutions, Instance Scheduler on AWS — <https://docs.aws.amazon.com/solutions/instance-scheduler-on-aws/>
4. AWS, AWS Lambda Pricing — <https://aws.amazon.com/lambda/pricing/>

**Images:**
<img width="960" height="504" alt="image" src="https://github.com/user-attachments/assets/dd96e8bf-14aa-48ca-aeba-ff0dee411ca8" />

**Post link:**
<https://www.facebook.com/share/1EugopND2c/?>
