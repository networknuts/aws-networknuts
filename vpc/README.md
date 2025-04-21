# AWS VPC Task List for Students

This README outlines tasks for creating and managing **custom VPCs**, working with **subnets**, launching instances, and establishing **inter-VPC communication**.

---

## ✅ VPC Tasks to Perform

### Part 1: Create a Custom VPC with Two Subnets

1. **Create a Custom VPC**
   - CIDR block: `10.0.0.0/16`

2. **Create Two Subnets in the VPC**
   - Subnet A (e.g., `10.0.1.0/24`) in Availability Zone 1
   - Subnet B (e.g., `10.0.2.0/24`) in Availability Zone 2

3. **Create an Internet Gateway and Attach to VPC**

4. **Update Route Tables**
   - Create or modify route tables to allow internet access from one subnet
   - Associate route tables with appropriate subnets

5. **Launch EC2 Instances in Each Subnet**
   - Instance A in Subnet A
   - Instance B in Subnet B
   - Ensure security groups allow ICMP (ping) and SSH between instances

6. **Test Connectivity Between Subnets**
   - SSH into one instance and ping the other

---

### Part 2: Create Another VPC

7. **Create a Second VPC**
   - CIDR block: `192.168.0.0/16`

8. **Create a Subnet in Second VPC**
   - Subnet C (e.g., `192.168.1.0/24`)

9. **Launch an EC2 Instance in Subnet C**

---

### Part 3: Enable Communication Between VPCs

10. **Create a VPC Peering Connection**
    - Between VPC1 (`10.0.0.0/16`) and VPC2 (`192.168.0.0/16`)
    - Accept the peering request

11. **Update Route Tables in Both VPCs**
    - Add routes in each VPC to allow traffic to the other VPC's CIDR block

12. **Modify Security Groups**
    - Allow ICMP and SSH traffic between instances across both VPCs

13. **Test Inter-VPC Communication**
    - SSH or ping from an instance in VPC1 to an instance in VPC2

---

14. **Clean Up Resources**
    - Terminate EC2 instances
    - Delete VPCs, subnets, and peering connection

---

> 📌 Submit screenshots for VPC setup, subnets, peering connection, and successful ping/SSH tests between instances to validate task completion.
