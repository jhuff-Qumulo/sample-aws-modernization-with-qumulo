---
title: "Introduction"
chapter: true
weight: 1
---

# Introduction


## **Learning Objectives**
By the end of this workshop, you will be able to:  
- Understand the **Qumulo ScaleAnywhere™ architecture** and how it enables seamless data management across hybrid and cloud environments.
- Deploy and configure **Qumulo on AWS**, including **persistent storage, compute storage, and client infrastructure**.
- Navigate the **Qumulo GUI**, analyze storage performance with built-in metrics, and manage multi-protocol file sharing (**NFS, SMB, and S3**).
- Scale **Qumulo clusters dynamically**, both horizontally (scale-out/in) and vertically (scale-up/down).
- Leverage **Cloud Data Fabric (CDF)** to create a hub/spoke data portal and optimize access scenarios across global namespace.
- Implement **High Availability (HA) and Disaster Recovery (DR)** strategies using snapshots and replication
- How to migratye data using **Shift-to/from Amazon S3**.

---

## **Workshop Structure (Modules)**  

### **Qumulo Architecture ScaleAnywhere**
- Introduction to **Qumulo’s ScaleAnywhere™ and RunAnywhere™ architecture**  
- **Cloud-Native Qumulo Architecture** overview  
- **Cloud Data Fabric (CDF)** and hybrid data management  

### **Deploying Qumulo on AWS**
- **Prerequisites** for deployment  
- Deploying **client infrastructure**  
- **Persistent Storage Deployment** (CloudFormation or Nexus GUI)  
- **Compute Storage Deployment** (CloudFormation or Nexus GUI)  

### **Qumulo GUI**
- **Dashboard overview** and system status  
- **Analytics & Metrics**: Monitoring performance  
- **Sharing**: Creating **multi-protocol shares** (NFS, SMB, S3)  
- **Access Control & Security**  

### **Scalability**
- **Scale-out**: Adding a node to the cluster  
- **Scale-in**: Removing a node  
- **Scale-up**: Increasing performance of existing instances  

### **Cloud Data Fabric**
- **Creating a hub/spoke portal** for hybrid cloud workflows  
- **Testing access scenarios** across on-prem and cloud environments  

### **High Availability & Disaster Recovery**
- **Snapshots and replication** for data protection  
- **Continuous replication** and disaster recovery  
- **Shift-to Amazon S3**: Archiving data to AWS storage  
- **Shift-from Amazon S3**: Restoring data from AWS storage  

---

This structured approach ensures a hands-on learning experience, providing participants with **real-world skills** in deploying, managing, and scaling Qumulo storage solutions in AWS.  


{{% notice warning %}}
The examples and sample code provided in this workshop are intended to be consumed as instructional content. These will help you understand how various AWS services can be architected to build a solution while demonstrating best practices along the way. These examples are not intended for use in production environments.
{{% /notice %}}
