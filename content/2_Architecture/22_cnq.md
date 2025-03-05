---
title: "Cloud-Native Qumulo" 
chapter: true
weight: 2 
---


# **Cloud-Native Qumulo**  

## **Introduction**  
As organizations shift workloads to the cloud, storage solutions must be **highly scalable, cloud-optimized, and deeply integrated with cloud services**. **Cloud-Native Qumulo (CNQ)** is designed to run natively in the **AWS cloud environment**, delivering **the same enterprise-grade file storage performance, security, and scalability** as on-premises deployments—without requiring specialized hardware.

This module explores how **CNQ leverages AWS-native infrastructure** to provide a **scalable, cost-efficient, and high-performance file storage solution** that integrates seamlessly with AWS services.

---

## **Key Takeaways**  
By the end of this module, you will:  

- Understand the **Cloud-Native Qumulo (CNQ) architecture** and its key benefits.  
- Learn how CNQ is **optimized for AWS compute and storage infrastructure**.  
- Explore **deployment models** for CNQ, including **persistent storage vs. ephemeral compute storage**.  
- Understand how CNQ integrates with **AWS services such as EC2, S3, IAM, and CloudFormation**.  

---

## **Topics Covered**  

### **What is Cloud-Native Qumulo (CNQ)?**  
- How CNQ extends **Qumulo’s file system into the cloud**.  
- **Key architectural differences** between CNQ and on-prem Qumulo.  
- The benefits of running a **fully cloud-native storage solution**.  

### **AWS-Optimized Qumulo Infrastructure**  
- **Compute & Storage**: How CNQ runs on AWS EC2 instances.  
- **EBS-backed storage**: Leveraging AWS **Elastic Block Store (EBS) for persistent storage**.  
- **High-performance workloads**: How CNQ optimizes storage for cloud applications.  

### **Deployment Models for CNQ**  
- **Persistent Storage Deployment**:  
  - Uses **AWS CloudFormation or Nexus GUI**.  
  - Ideal for **long-term storage solutions** that require **durability and resilience**.  
- **Ephemeral Compute Storage Deployment**:  
  - Designed for **short-term, high-performance computing workloads**.  
  - Uses AWS instances for **temporary, high-speed storage needs**.  

### **CNQ and AWS Service Integration**  
- **Amazon S3**: CNQ’s **Shift-to and Shift-from** S3 capabilities.  
- **IAM (Identity & Access Management)**: Securing data access within AWS.  
- **CloudFormation (CF) templates** for automated deployment.  
- **AWS Auto-Scaling**: Expanding and contracting Qumulo storage as needed.  

---

## **Why Cloud-Native Qumulo (CNQ)?**  
- **Cloud-Optimized**: Purpose-built for **AWS elasticity and scalability**.  
- **Enterprise-Grade Performance**: Delivers **low-latency, high-throughput file storage** in the cloud.  
- **Deep AWS Integration**: Seamlessly connects with **EC2, S3, IAM, and CloudFormation**.  
- **Scalability & Agility**: Rapidly scale storage **up or down** based on demand.  

CNQ allows organizations to **leverage AWS’s infrastructure while maintaining full control over their file storage**, making it an ideal solution for **media, healthcare, research, and analytics-driven workloads**.

---

### **Next Steps**  
In the next section, we will introduce **Cloud Data Fabric (CDF)**, a key component that enables **hybrid data management** across cloud and on-prem environments.

