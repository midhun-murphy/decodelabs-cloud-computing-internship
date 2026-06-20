# Task 4 - Serverless Cost Calculator

## Project Overview

This project demonstrates a simple serverless application using AWS Lambda. The function accepts two numbers as input and returns their sum. The solution follows a serverless architecture, eliminating the need to manage servers while providing automatic scaling and pay-per-use execution.

---

## Services Used

- AWS Lambda
- Amazon CloudWatch Logs

---

## Programming Language

- Python 3.14

---

## Architecture

```text
Test Event
    ↓
AWS Lambda Function
    ↓
Sum Calculation
    ↓
JSON Response
```

---

## Lambda Function Code

```python
def lambda_handler(event, context):

    num1 = event.get('num1')
    num2 = event.get('num2')

    total = num1 + num2

    return {
        "Sum": total
    }
```

---

## Test Event

```json
{
  "num1": 15,
  "num2": 25
}
```

---

## Output

```json
{
  "Sum": 40
}
```

---

## Execution Status

- Function Created Successfully
- Code Deployed Successfully
- Test Event Executed Successfully
- Output Verified

---

## Learning Outcomes

- Understanding Serverless Computing
- Creating AWS Lambda Functions
- Writing Event-Driven Python Code
- Testing Lambda Functions
- Monitoring Execution with CloudWatch Logs

---

## Author

Midhun Kumar V
Cloud Computing Internship - Decodelabs
