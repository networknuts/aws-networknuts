# AWS EFS Task List for Students

This README outlines the essential tasks for working with **Amazon Elastic File System (EFS)** and connecting it to **EC2 instances**.

---

## ✅ EFS Tasks to Perform

1. **Create an EFS File System**
   - Choose appropriate VPC and availability zones

2. **Create Mount Targets**
   - Ensure mount targets are created in each required Availability Zone
   - Use correct security groups to allow NFS access

3. **Create Two EC2 Instances**
   - Use Amazon Linux 2 in the same VPC and AZs as the EFS mount targets
   - Ensure security group allows NFS (port 2049)

4. **Install NFS Utilities on Both EC2 Instances**
   - Prepare instances to mount EFS

5. **Mount EFS File System on Both EC2 Instances**
   - Mount the file system to a common directory on both instances

6. **Test File Sharing Between Instances**
   - Create a file on one instance and verify it is accessible from the other

7. **Configure EFS to Mount Automatically (Optional)**
   - Add EFS mount entry to `/etc/fstab` for persistence

8. **Enable Backup (Optional)**
   - Enable AWS Backup for the EFS file system

9. **Enable Encryption at Rest and In Transit (Optional)**
   - Ensure encryption settings are properly configured

10. **Clean Up Resources**
   - Unmount EFS from both EC2 instances
   - Terminate EC2 instances
   - Delete the EFS file system and mount targets

---

> 📌 Submit screenshots for mount targets, EFS mount on both instances, and shared file access to validate task completion.
