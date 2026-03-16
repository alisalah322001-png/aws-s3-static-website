# AWS S3 Static Website with Cross-Region Replication (CRR)

![Architecture](diagrams/architecture.png)

## Project Overview
This project demonstrates how to host a **static website** on **Amazon S3** with **Cross-Region Replication (CRR)** for high availability and disaster recovery.

- **Primary Bucket:** Hosts the website with versioning enabled.
- **Replica Bucket:** Automatically receives replicated objects from the primary bucket.
- **Automation:** Infrastructure deployed using **AWS CloudFormation**.
- **Website:** HTML/CSS static pages including images.

---

## Features
- Static website hosting on S3.
- Cross-Region Replication to another AWS region.
- IAM role configured for S3 replication.
- Versioning enabled for primary and replica buckets.
- Fully automated deployment via CloudFormation.
- Publicly accessible website URL.

---

## Project Structure

```text
aws-s3-static-website-crr/
│
├── cloudformation/
│   └── s3-website-crr.yaml      # CloudFormation template for S3 buckets + CRR
│
├── website/
│   ├── index.html
│   ├── style.css
│   └── images/                  
│
├── diagrams/
│   └── architecture.png         # Architecture diagram
│
└── README.md                   