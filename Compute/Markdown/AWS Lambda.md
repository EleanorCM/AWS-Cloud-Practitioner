
## What is AWS Lambda?

Serverless compute service - run your app without managing EC2 instances or provisioning compute resources
- Highly scalable with excellent cost optimization compared to EC2
- Serverless from the user perspective
- More time to focus on your code
- Sub-second metering: Charged per 100 milliseconds of use only when your code is running plus the number of times your code runs

## Working with AWS Lambda

1. Upload code or write it in build-in code editor (supports Node.js, Java, C#, Python, Go, PowerShell and Ruby
2. Configure Lamba functions to execute on triggers from your event sources. Ie object uploaded to S3 bucket
3. Lambda runs your code using only required compute
4. AWS records compute time in milliseconds and the quantity of functions

## Components of AWS Lambda

**Lambda Function**: Your code to be invoked

**Event Source**: AWS services used to trigger functions

**Trigger**: an operation from an event source

**Downstream resources**: resources required during execution

**Log streams**: to troubleshoot issues. A sequence of events from a function, recorded in CloudWatch

## Creating Lambda Functions

1.  Select a Blueprint (function template provided by Lambda)
2.  Configure Triggers
3.  Configure Function (upload code or edit inline