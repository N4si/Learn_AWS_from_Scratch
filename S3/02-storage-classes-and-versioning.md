# 🏷️ S3 Storage Classes and Versioning

## S3 Storage Classes  
S3 offers a range of storage classes for different use cases, helping you optimize costs based on your data access patterns.

### Storage Classes:
1. **Standard**  
   - High availability and durability. Suitable for frequently accessed data.
   - **Durability**: 99.999999999%  
   - **Availability**: 99.99%
   
2. **Intelligent-Tiering**  
   - Automatically moves objects between access tiers when access patterns change.
   - Optimizes costs by placing infrequently accessed data into a lower-cost tier.
   
3. **Standard-IA (Infrequent Access)**  
   - Lower-cost for infrequently accessed data that requires high availability.
   
4. **One Zone-IA**  
   - Low-cost storage for infrequently accessed data in a single AZ (availability zone).

5. **Glacier & Glacier Deep Archive**  
   - Designed for long-term archival storage. Retrieval times can vary from minutes (Glacier) to hours (Glacier Deep Archive).
   
---

## 🔄 S3 Versioning  
Versioning allows you to preserve, retrieve, and restore every version of an object stored in an S3 bucket. 

### Benefits of Versioning:
- **Accidental deletion protection**: If an object is deleted, previous versions can be restored.
- **Object overwrite protection**: Retain older versions in case of unintended overwrites.

### Managing Versioning:
- **Enable/Disable versioning**: Once enabled, versioning cannot be fully disabled (can only be suspended).
- **Delete markers**: When you delete an object, a delete marker is created instead of permanently removing the data.

---

## 🔄 Lifecycle Policies for Object Management
Lifecycle policies enable you to automate the migration of objects between different storage classes based on rules you define.

### Use Cases:
- **Transition**: Move objects to lower-cost storage (e.g., Standard to Glacier) after a specified time.
- **Expiration**: Automatically delete objects after a set retention period.

### Policy Types:
1. **Transition Policies**: Move objects to cheaper storage.
2. **Expiration Policies**: Set rules to delete objects after a certain time.
