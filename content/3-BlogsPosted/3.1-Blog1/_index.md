---
title: "Blog 1"
date: 2026-11-24
weight: 1
chapter: false
pre: " <b> 3.1. </b> "
---

# SECURE ACCESS CONTROL FOLLOWING THE LEAST PRIVILEGE PRINCIPLE WITH AWS IAM

When getting started with AWS, many beginners tend to attach `AdministratorAccess` to every user or application to "get things running quickly and avoid permission errors." However, in production environments, this is one of the biggest security risks. The standard solution to mitigate this issue is applying the **Principle of Least Privilege** using AWS IAM.

### 1. What is the Principle of Least Privilege?

Simply put: **Grant only the exact permissions required for a user or service to perform their intended tasks—no more, no less.**

**Examples:**
* An application running on EC2 that only needs to read images from a specific S3 bucket → grant only `s3:GetObject` on that exact bucket, rather than attaching `AmazonS3FullAccess` across the entire account.
* An intern who only needs to view logs for debugging → grant read-only access to CloudWatch Logs rather than permissions to delete or modify infrastructure.

If an account or application's credentials are ever compromised, the potential blast radius is strictly contained within a minimal scope.

### 2. How to Effectively Apply Least Privilege in AWS IAM

You can start implementing this principle right away through these four core practices:

* **Use IAM Roles instead of hardcoded Access Keys:** When applications on EC2 or Lambda need to interact with services like S3 or DynamoDB, attach an IAM Role to the compute resource. AWS automatically issues and rotates temporary security credentials, eliminating the risk of exposing Access Keys in source code or configuration files.
* **Manage permissions via IAM Groups:** Instead of attaching standalone policies to individual users, organize users into role-based groups (e.g., `Developers`, `Testers`, `ReadOnly-Audit`) to simplify permission management and revocation.
* **Narrow the scope in IAM Policies:** When authoring or selecting a policy, pay close attention to three key elements:
  * **Action:** Explicitly specify allowed actions (e.g., `s3:GetObject`, `s3:PutObject` instead of `s3:*`).
  * **Resource:** Specify the exact ARN of the target resource instead of using a wildcard `*` (all resources).
  * **Condition (when needed):** Add extra guardrails, such as restricting access to specific IP ranges or enforcing Multi-Factor Authentication (MFA).
* **Periodically review and remove unused permissions:** Leverage **IAM Access Analyzer** (or the *Last Accessed* tab in the IAM console) to identify users or roles holding permissions they haven't used in months, and trim them down to match actual usage.

### 3. Essential Accompanying Security Best Practices

* **Do not use the Root account for daily tasks:** Enable MFA on the Root user, store its credentials securely, and use appropriately scoped IAM users or roles for day-to-day operations.
* **Enable MFA for all IAM Users:** Adding an extra layer of authentication significantly reduces the risk of account takeover if a password is accidentally exposed.

### Summary

Applying Least Privilege does not make your system harder to manage; rather, it gives you clear visibility and control over who is doing what in your AWS account. Building the habit of granting "just enough" permissions from your very first hands-on labs will serve as a critical foundation throughout your Cloud journey.

**References:**
1. AWS Well-Architected Framework, SEC03-BP02: Grant least privilege access — <https://docs.aws.amazon.com/wellarchitected/latest/security-pillar/sec_permissions_least_privileges.html>
2. AWS IAM FAQs, What are least-privilege permissions? — <https://aws.amazon.com/iam/faqs/>
3. AWS IAM User Guide, IAM roles — <https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles.html>
4. AWS Service Authorization Reference, Actions, resources, and condition keys — <https://docs.aws.amazon.com/service-authorization/latest/reference/reference_policies_actions-resources-contextkeys.html>

**Images:**
<img width="955" height="540" alt="image" src="https://github.com/user-attachments/assets/9eecce7d-14d8-431e-83db-1f04d5b46517" />

**Post link:**
<https://www.facebook.com/share/153tbhDi7kk/?>
