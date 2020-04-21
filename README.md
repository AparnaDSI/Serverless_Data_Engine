# Serverless_Data_Engine
Steps-
1. Create a DynamoDB Table on AWS
2. Create a AWS Lambda function (producer) to read data from DynamoDB
3. Enable a Cloudwatch trigger to the Lambda function which will send the messages in a timely manner to SQS (Simple Queue Sevice) of AWS
4. Create a SQS Queue to poll messages once the Lambda fucntion is deplpoyed
5. Create another AWS Lambda fucntion (Consumer) to take data that is triggered by the messages received from SQS, and send to S3 for storage.
6. Create a S3 bucket in which the data will be stored after the NLP has been run on it.
