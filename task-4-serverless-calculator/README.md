# AWS Serverless Cost Calculator

## Project Overview

The AWS Serverless Cost Calculator is a simple cloud-native application built using AWS Lambda. The function accepts two numbers as input through a test event, performs an addition operation, and returns the result in JSON format. This project demonstrates the fundamentals of serverless computing, event-driven execution, and AWS Lambda deployment.

---

## Objectives

- Understand Serverless Computing concepts
- Create and deploy an AWS Lambda Function
- Process event-based input using Python
- Return JSON responses
- Monitor execution using Amazon CloudWatch Logs

---

## Architecture

```text
User/Test Event
       │
       ▼
 AWS Lambda Function
       │
       ▼
 Sum Calculation
       │
       ▼
 JSON Response
```

---

## AWS Services Used

| Service | Purpose |
|----------|----------|
| AWS Lambda | Execute code without managing servers |
| Amazon CloudWatch | Store logs and monitor execution |

---

## Programming Language

- Python 3.14

---

## Test Event

```json
{
  "num1": 15,
  "num2": 25
}
```

---

## Expected Output

```json
{
  "statusCode": 200,
  "message": "Calculation successful",
  "num1": 15,
  "num2": 25,
  "sum": 40
}
```

---

## Execution Steps

1. Login to AWS Console.
2. Navigate to AWS Lambda.
3. Create a new Lambda Function named `cost-calculator`.
4. Select Python Runtime.
5. Paste the Lambda function code.
6. Deploy the function.
7. Create a Test Event with input values.
8. Invoke the Lambda function.
9. Verify the output.
10. Review execution logs in CloudWatch.

---

## CloudWatch Monitoring

Amazon CloudWatch automatically captures:

- Invocation details
- Execution duration
- Memory usage
- Function logs
- Error messages

This helps in monitoring and troubleshooting serverless applications.

---

## Project Outcomes

- Successfully deployed an AWS Lambda function.
- Implemented event-driven serverless execution.
- Performed arithmetic operations using Lambda.
- Generated JSON responses.
- Monitored execution through CloudWatch Logs.

---

## Key Concepts Learned

- Serverless Architecture
- AWS Lambda
- Event-Driven Computing
- CloudWatch Logging
- JSON Processing
- Error Handling
- Python in Cloud Environments

---

## Repository Structure

```text
task-4-serverless-calculator/
│
├── lambda_function.py
├── README.md
├── screenshots/
│   ├── lambda-code.png
│   ├── test-event.png
│   └── output.png
```

---

## Author

**Midhun Kumar V**
