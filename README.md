# shell-scripting-project
# Event-driven project with S3, Lambda and SNS

 This code is to create Amazon S3, AWS Lambda, and Amazon SNS. It sets up an event-driven architecture where
an S3 bucket triggers a Lambda function, which then publishes a message to an SNS topic.

# Here's a breakdown of the project:

It sets the necessary variables, such as AWS region, bucket name, Lambda function name, role name, and email address.
It creates an IAM role with the required permissions for Lambda and S3.
It attaches policies to the IAM role to grant necessary permissions.
It creates an S3 bucket.
It uploads a file to the S3 bucket.
It creates a Lambda function using the provided code.
It grants the S3 bucket permission to invoke the Lambda function.
It sets up an S3 event trigger to invoke the Lambda function when a new object is created in the bucket.
It creates an SNS topic and subscribes an email address to it.
It publishes a message to the SNS topic when a new object is created in the S3 bucket.

 With this code, you can create a system that sends real-time notifications whenever a new object is created
 in an S3 bucket. The Lambda function can publish messages to an SNS topic, which can be subscribed by various
 endpoints such as email addresses, SMS, or even other Lambda functions.
