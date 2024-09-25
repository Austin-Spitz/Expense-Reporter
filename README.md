# Application Status

Work in progress. PDF file types are not supported currently.

# Setup: Backend

- Requirements: AWS Textract, S3 Buckets, Lambda, DynamoDB, and Python.
- Create a default S3 bucket with a folder named "upload/" for receipts.
- Configure a lambda with the necessary code from the provided backend folder.
- Add AWS Layer to lambda: AWSSDKPandas-Python312, version 4.
- Connect the S3 buckets to the Lambda by creating a trigger in the Lambda
- Generate Access Key ID and Secret Access Key from your AWS account.
- Create a Dynamodb

# Setup: Frontend

- Navigate to the .env file in the frontend
- Update the values based on what you have

```

ACCESS_KEY = your_access_key_here

SECRET_ACCESS_KEY = your_secret_access_key_here

REGION = your_aws_region_here

BUCKET_NAME = your_bucket_name_here

TABLE_NAME = your_table_name_here

```
  
# Known Bugs / Limitations

- Uploading a PDF image to S3 results in an "unsupported file type" error.
