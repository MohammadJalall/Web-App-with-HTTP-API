here are the set of steps for deploying a web application project with an HTTP API using AWS services. Here's a recap of the process:

CloudFormation Stack Setup:

Navigate to the CloudFormation main page.
Create a new stack and upload the YAML template file.
Proceed through the setup, acknowledging and creating the stack.
S3 Bucket Configuration:

Create an S3 bucket with a specific name for static hosting.
Enable static website hosting and specify the index document.
Edit the bucket policy to allow public read access.
Configure CORS settings for the bucket.
API Gateway Configuration:

Check the API created as part of the CloudFormation stack.
Copy the Invoke URL for use in the frontend configuration.
Modify routes, integrations, stages, and CORS settings in API Gateway.
Deploy the API to the desired stage.
Frontend Configuration:

Configure the frontend with the API's Invoke URL.
Install dependencies and build the frontend application.
Upload the production build to the S3 bucket.
Ensure the correct folder structure and file placement in S3.
Access the frontend application using the provided HTTPS URL in the index.html file.
Frontend Application Usage:

The frontend application typically opens a dashboard page.
The dashboard allows users to add new items via a form, specifying ID, name, and price.
A grid displays the added items.
Following these steps should result in a successfully deployed web application with an HTTP API, hosted on AWS infrastructure.






