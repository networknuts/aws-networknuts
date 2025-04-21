# AWS EBS Task List for Students (with EC2 Integration)

This README outlines the tasks for working with **Elastic Block Store (EBS)** volumes and connecting them to **EC2 instances**.

---

## ✅ EBS + EC2 Tasks to Perform

1. **Create an EC2 Instance**
   - Launch an instance using Amazon Linux 2
   - Allow SSH access via security group

2. **Create an EBS Volume**
   - Ensure it is in the same Availability Zone as your EC2 instance
   - Choose gp2 type and 1 GiB size

3. **Attach EBS Volume to EC2**
   - Attach the newly created volume to your running EC2 instance

4. **Connect to EC2 via SSH**
   - Use your key pair and public IP to connect

5. **Format and Mount the EBS Volume**
   - Format the volume with XFS or ext4
   - Mount it to a directory like `/data`

6. **Make Mount Persistent (Optional)**
   - Update the `/etc/fstab` file to ensure mount persists after reboot

7. **Verify Persistence**
   - Reboot the EC2 instance
   - Check if the volume is mounted automatically

8. **Detach the Volume**
   - Unmount the volume and detach it from the instance

9. **Attach to a Different EC2 Instance**
   - Attach the volume to a different EC2 instance
   - Mount it and verify any existing data

10. **Clean Up Resources**
   - Terminate EC2 instance(s)
   - Delete the EBS volume

---

> 📌 Submit screenshots of volume creation, mounting, and persistence verification to validate task completion.

