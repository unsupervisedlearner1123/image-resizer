# S3 Trigger with Lambda

This project provides an example of how to trigger a Lambda function using an Amazon S3 event. The function retrieves metadata for the object that has been updated.

This repo consists of a Lambda function and a test JSON file. The Lambda function is responsible for retrieving metadata for the object, and the test JSON file is used to simulate an S3 event.

## Usage

To use this project, follow these steps:

* Clone the repository to your local machine.
* Create an AWS Lambda function using the code provided in the lambda_function.py file.
* Create an S3 bucket and add an object to the bucket.
* Use the test JSON file (test_event.json) to simulate an S3 event by executing the following command:

```
aws lambda invoke --function-name <YOUR LAMBDA FUNCTION NAME> --payload file://test_event.json output.txt

```