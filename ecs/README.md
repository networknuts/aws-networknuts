# AWS ECS Task List for Students

This document outlines ECS-related tasks for running an already available container image on AWS Elastic Container Service (ECS).

---

## ✅ ECS Tasks to Perform

1. **Create a new ECS Cluster**
   - Choose the Fargate launch type

2. **Create a Task Definition**
   - Use a public container image (e.g., `nginx` or `httpd`)
   - Define CPU, memory, and port mappings (e.g., expose port 80)

3. **Run a Standalone Task in the ECS Cluster**
   - Use the created task definition
   - Confirm the task runs successfully

4. **Create a Service using the Task Definition**
   - Set the desired task count to 2
   - Enable public IP assignment
   - Skip load balancer configuration (optional)

5. **Access the Running Container via Public IP**
   - Fetch public IP of the task from the console
   - Access the container's web page (e.g., NGINX welcome page)

6. **Stop and Delete All Tasks and the ECS Cluster**
   - Clean up resources to avoid charges

---

> 📌 Submit screenshots of task creation, container web page access, and CloudWatch logs to validate completion.
