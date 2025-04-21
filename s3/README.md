# AWS S3 Task List for Students

This README outlines a comprehensive set of tasks for working with **Amazon S3** including access controls, hosting, replication, and more.

---

## ✅ S3 Tasks to Perform

1. **Create an S3 Bucket**
   - Name it uniquely and select a region

2. **Enable Public Access for the Bucket**
   - Disable block public access settings
   - Add a bucket policy to allow public read

3. **Upload Objects to the Bucket**
   - Upload sample HTML, image, or text files

4. **Access Public Object via URL**
   - Copy and test the object URL in a browser

5. **Enable Static Website Hosting**
   - Turn on static website hosting for the bucket
   - Set index and error documents (e.g., `index.html`, `error.html`)

6. **Access the Website via S3 Endpoint**
   - Use the provided endpoint to test your hosted site

7. **Enable Bucket Versioning**
   - Enable versioning for the bucket
   - Upload multiple versions of the same file

8. **View and Restore File Versions**
   - List and manage previous versions of objects

9. **Create an IAM User with S3 Programmatic Access**
   - Grant the user `AmazonS3FullAccess` or limited access via a policy
   - Generate and store access key and secret

10. **Access the Bucket Using Access Tokens**
   - Use AWS CLI or SDK with access key/secret to upload/download files

11. **Enable Cross-Region Replication**
   - Create a second bucket in another region
   - Enable versioning on both source and destination
   - Create a replication rule from source to destination

12. **Verify Replication**
   - Upload files to the source bucket and confirm replication in the destination bucket

13. **Set Lifecycle Rules**
   - Add rules to transition files to Glacier or delete after a specific period

14. **Enable Logging or Object-Level Events (Optional)**
   - Enable logging or event notifications for uploads/deletions

15. **Clean Up Resources**
   - Delete objects, empty buckets, and remove IAM users to avoid charges

---

> 📌 Submit screenshots for bucket policies, website URLs, versioning, replication, and access via token to validate task completion.
