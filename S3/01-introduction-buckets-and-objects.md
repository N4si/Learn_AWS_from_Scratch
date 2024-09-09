# 🌐 Introduction to S3, Buckets, and Objects

## What is Amazon S3?  
Amazon S3 (Simple Storage Service) is an object storage service that provides scalability, data availability, security, and performance for a wide range of use cases.

### Key Features:
- **Object storage**: Store unlimited data as objects in buckets.
- **Durability & Availability**: Designed for **99.999999999%** (11 9's) durability.
- **Use cases**: Backup & restore, data lakes, hosting static websites, and more.

---

## 🗂️ S3 Buckets  
A bucket is a container for storing objects. Buckets are region-specific and have globally unique names.

### Key Concepts:
- **Bucket creation**: Choose a name and region.
- **Global namespace**: Bucket names must be unique across all AWS accounts.
- **Region-specific**: Buckets are located in an AWS region for latency optimization and compliance.

---

## 📄 S3 Objects  
Objects are the fundamental entities stored in S3, and they consist of:
- **Key** (Unique identifier)
- **Data** (Binary content)
- **Metadata** (Additional information such as file type, permissions)

### Object Versioning:
- **Versioning**: Stores multiple variants of an object in the same bucket, useful for protecting against unintended overwrites and deletions.
- **Object lifecycle**: Controls the creation, retention, and deletion of versions through lifecycle policies.

---

## 🔄 Data Consistency Model
S3 provides strong **read-after-write consistency** for PUTs of new objects and eventual consistency for overwrite PUTs and DELETEs.
