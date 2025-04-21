# AWS Cross-Region Load Balancer Task List for Students

This README outlines the tasks to set up a **Global Accelerator-based solution** to load balance traffic across **EC2 instances in two different VPCs and regions**.

---

## ✅ Cross-Region Load Balancer Tasks to Perform

### Part 1: VPC and EC2 Setup in Two Regions

1. **Create VPC in Region A**
   - CIDR block: `10.0.0.0/16`
   - Create a public subnet: `10.0.1.0/24`

2. **Launch an EC2 Instance in Region A**
   - Install a web server (e.g., return a region-specific message)
   - Ensure the instance is in a public subnet with internet access

3. **Create VPC in Region B**
   - CIDR block: `192.168.0.0/16`
   - Create a public subnet: `192.168.1.0/24`

4. **Launch an EC2 Instance in Region B**
   - Install a web server with a different region-specific response

### Part 2: Create Load Balancers in Both Regions

5. **Create an Application Load Balancer in Region A**
   - Internet-facing
   - Add EC2 instance in Region A to the target group

6. **Create an Application Load Balancer in Region B**
   - Internet-facing
   - Add EC2 instance in Region B to the target group

### Part 3: Global Traffic Management

7. **Create a Global Accelerator**
   - Add both regional ALBs as endpoints
   - Configure traffic distribution (e.g., 50-50 or failover)

8. **Test the Global Accelerator Endpoint**
   - Access the provided DNS name
   - Confirm traffic reaches both instances across regions

### Part 4: Clean Up

9. **Clean Up Resources**
   - Delete EC2 instances
   - Delete both ALBs and target groups
   - Remove the Global Accelerator
   - Delete VPCs and subnets

---

> 📌 Submit screenshots of Global Accelerator, ALBs, EC2 instances, and test results showing region-based responses to validate task completion.
