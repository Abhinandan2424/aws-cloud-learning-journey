# AWS Cloud Learning Journey - Day 4

# Identity and Access Management (IAM)

## What is IAM?

AWS Identity and Access Management (IAM) is a global AWS service that helps securely manage access to AWS resources.

It controls:

- Who can access AWS resources
- What actions they can perform
- Which resources they can access

---

## Why do we use IAM?

Instead of sharing the AWS Root Account with everyone, we create IAM Users and grant only the required permissions.

Benefits:

- Improved Security
- Access Control
- Principle of Least Privilege
- Easy User Management

---

# IAM Components

## IAM User

An IAM User represents an individual person or application that needs access to AWS.

Example:

- Developer
- Tester
- Admin

---

## IAM Group

A Group is a collection of IAM Users.

Instead of assigning permissions individually, permissions are assigned to the Group.

Example:

Developer Group

- Abhii
- Roshan
- Sakshi
- Tanvi
- Yash

All users inherit the same permissions.

---

## IAM Policy

Policies are JSON documents that define permissions.

They specify:

- Allowed Actions
- Denied Actions
- AWS Resources

Example:

AmazonS3ReadOnlyAccess

Allows users to read S3 buckets but not upload or delete objects.

---

# Principle of Least Privilege

Always provide only the minimum permissions required to complete a task.

Example:

If a developer only needs S3 Read access,

Do NOT give:

AmazonS3FullAccess

Instead provide:

AmazonS3ReadOnlyAccess

---

# Practical Performed

✔ Opened IAM Dashboard

✔ Explored Users

✔ Explored Groups

✔ Explored Policies

✔ Understood IAM Permission Model

✔ Learned Principle of Least Privilege

---

# Interview Questions

### What is IAM?

IAM is a global AWS service used to securely manage access to AWS resources.

---

### Difference between Root User and IAM User?

Root User:

- Full access
- Created when AWS account is created

IAM User:

- Limited permissions
- Permissions assigned using Policies

---

### Why should we avoid using the Root User?

Because it has unrestricted access to the AWS account.

AWS recommends using IAM Users for daily work.

---

### What is an IAM Group?

A collection of IAM Users having similar permissions.

---

### What is an IAM Policy?

A JSON document that defines permissions for AWS resources.

---

# Key Takeaways

- IAM is the foundation of AWS Security.
- Never use the Root User for daily work.
- Always follow the Principle of Least Privilege.
- Policies define permissions.
- Groups simplify permission management.