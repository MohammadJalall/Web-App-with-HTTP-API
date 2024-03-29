These steps for deploying a web application project with an HTTP API using AWS services. Here's a recap of the process:

1. **CloudFormation Stack Setup**:
   - Navigate to the CloudFormation main page.
   - Create a new stack and upload the YAML template file.
   - Proceed through the setup, acknowledging and creating the stack.

2. **S3 Bucket Configuration**:
   - Create an S3 bucket with a specific name for static hosting.
   - Enable static website hosting and specify the index document.
   - Edit the bucket policy to allow public read access.
   - Configure CORS settings for the bucket.

3. **API Gateway Configuration**:
   - Check the API created as part of the CloudFormation stack.
   - Copy the Invoke URL for use in the frontend configuration.
   - Modify routes, integrations, stages, and CORS settings in API Gateway.
   - Deploy the API to the desired stage.

4. **Frontend Configuration**:
   - Configure the frontend with the API's Invoke URL.
   - Install dependencies and build the frontend application.
   - Upload the production build to the S3 bucket.
   - Ensure the correct folder structure and file placement in S3.
   - Access the frontend application using the provided HTTPS URL in the index.html file.

5. **Frontend Application Usage**:
   
   - After all uploading is done, open index.html at the root of S3 bucket, inside it shows an HTTPS URL, use that to access the frontend application
   - The frontend application typically opens a dashboard page.
   - The dashboard allows users to add new items via a form, specifying ID, name, and price.
   







