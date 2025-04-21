# AWS Elastic Beanstalk Task List for Monolithic App Deployment

This README outlines the tasks for deploying a **monolithic application** (non-containerized) using AWS Elastic Beanstalk.

---

## ✅ Monolith Deployment Tasks to Perform

1. **Prepare the Monolithic Application**
   - Use the following prebuilt `.jar` file for deployment:
     - [Download one-jar-example-0.97.jar](https://sourceforge.net/projects/one-jar/files/one-jar/0.97/one-jar-example-0.97.jar/download)
   - This is a self-contained Java application packaged using the One-JAR tool.

2. **Create a New Elastic Beanstalk Application**
   - Go to the Elastic Beanstalk console
   - Click on "Create a new application"

3. **Create an Environment for the App**
   - Choose **Web Server Environment**
   - Select the **Java** platform
   - Upload the downloaded `.jar` file

4. **Configure Environment Settings**
   - Add Environment Variables if needed
   - Choose instance type (e.g., t2.micro for testing)
   - Configure capacity (single instance or load-balanced)
   - Enable HTTPS (optional)

5. **Deploy the Application**
   - Click "Create Environment"
   - Wait for environment health to turn **Green**

6. **Access the Application**
   - Visit the auto-generated Elastic Beanstalk URL
   - Confirm the application is running successfully

7. **Monitor and Debug**
   - Use the Beanstalk console to:
     - View logs
     - Monitor CPU/memory
     - Restart environment if needed

8. **Update the Application**
   - Upload a new version of your app (you can redeploy the same `.jar` or try a different one)
   - Deploy it using the "Upload and Deploy" option

9. **Terminate the Environment**
   - After testing, delete the environment and application to avoid AWS charges

---

> 📌 Submit screenshots of the environment setup, URL output, and updated deployments to validate completion.

