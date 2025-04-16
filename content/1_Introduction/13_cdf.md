---
title: "Cloud Data Fabric Introduction" 
chapter: true
weight: 3
---

# Introduction to Qumulo Cloud Data Fabric (CDF)

## 1. Introduction

Qumulo Cloud Data Fabric (CDF) is an enterprise-wide cloud data platform designed to provide access to unstructured data regardless of location. It creates a single, globally-consistent file system that spans edge, core data centers, and cloud environments, enabling teams to share data across long distances with minimal latency and without version conflicts.

CDF provides a transformative approach to data management by:
* Creating local access to data regardless of where it resides
* Enabling real-time collaboration between geographically dispersed teams
* Simplifying data governance through unified access controls
* Accelerating time-to-value by minimizing data transfer requirements

## 2. CDF Architecture

### Hub and Spoke Model
CDF is built on a hub-and-spoke architecture where:
* **Hub**: Central Qumulo instance that hosts the source data
* **Spoke**: Remote Qumulo instances that can access the hub's data
* **Portal**: Connection between hub and spoke that defines which directories are shared

![Hub and Spoke Model](../images/cdf-portals.png)

### Data Portal Details
* Defined at a directory level (not entire file systems)
* Can be configured as read-only or bidirectional (read-write)
* Each portal supports one hub folder and up to 32 spokes
* Directories within a portal appear as if they're local to spoke clients

![Data Portal Details](../images/cdf-portal2.png)

### Data Synchronization Process
1. **Metadata First**: Directory structure and file metadata are synchronized immediately
2. **Data On-Demand**: File data blocks (4K) are only transferred when requested by a client
3. **Local Caching**: Accessed data is cached locally on the spoke for future requests
4. **Block-Level Changes**: Only modified blocks are synchronized, not entire files

![Data Synchronization Process](../images/cdf-caching.png)

### NeuralCache Intelligence
NeuralCache is a predictive caching engine that:
* Monitors data access patterns over time
* Anticipates future data requests based on learned patterns
* Proactively prefetches data into local cache before it's requested
* Features a heat-scoring system that prioritizes frequently accessed data

![NeuralCache Detail](../images/cdf-neuralcache.png)

## 3. CDF Common Use Cases

![Common Use Cases](../images/cdf-usecase.png)

### Cloud Bursting for Compute-Intensive Workloads
* **Challenge**: Need more computing power for rendering or analysis
* **Solution**: Express on-premises data to cloud instances via CDF
* **Benefit**: Scale compute resources without copying entire datasets

### Real-Time Global Collaboration
* **Challenge**: Teams in different locations need to work on the same files
* **Solution**: Set up bidirectional portals between locations
* **Benefit**: Everyone works on the same data without version conflicts

### AI/ML Pipeline Optimization
* **Challenge**: AI engines need access to large datasets without moving them
* **Solution**: Express on-premises data to cloud-based AI services
* **Benefit**: Process data where it makes most sense without duplication

### Edge Data Collection with Central Processing
* **Challenge**: Data collected at the edge needs central processing
* **Solution**: Set up portals from edge locations to central hub
* **Benefit**: Data appears instantly at the hub without full transfer

## 4. Key Takeaways

* **Not Replication**: CDF doesn't replicate entire datasets; it synchronizes metadata globally and transfers data blocks only when needed
* **Strict Consistency**: All endpoints maintain the same view of data with guaranteed consistency
* **Intelligent Caching**: 90% of global read requests are served from cache, minimizing WAN traffic
* **Performance Optimization**: NeuralCache anticipates data needs, reducing latency significantly
* **Unified Management**: A single platform for managing data across any location

## 5. Topics Covered

In this overview, we've explored:
* The fundamental concept and benefits of Cloud Data Fabric
* The hub-spoke architecture and portal configuration
* How data synchronization works at the metadata and block levels
* The intelligent caching system with NeuralCache
* Common use cases where CDF provides unique advantages
* What differentiates CDF from traditional replication solutions

## 6. Next Steps

* Review Workshop Prerequisites
* Set Up Your AWS Environment


