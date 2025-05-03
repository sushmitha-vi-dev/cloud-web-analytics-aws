# Real-Time Web Analytics Platform on AWS

A serverless analytics solution to capture, stream, and analyze user interaction data using AWS services. Built for real-time insights into marketing campaign performance and content effectiveness.

---

## 🚀 Architecture Overview

- **API Gateway**: Accepts client events (clicks, page views).
- **AWS Lambda**: Processes incoming events and triggers downstream actions.
- **Amazon Kinesis Firehose**: Streams event data to S3 for analytics.
- **Amazon S3**: Stores raw events for downstream processing.
- **Amazon CloudWatch**: Monitors function performance and errors.
- **Amazon SES**: Sends email alerts for predefined thresholds.


---

## 🧰 Tech Stack

- **Cloud Services**: AWS Lambda, S3, API Gateway, Kinesis Firehose, CloudWatch, SES  
- **Language**: Python  
- **Formats**: JSON, REST API

---

## 🔁 Workflow

1. User triggers an event (e.g., page click)
2. API Gateway receives and forwards to Lambda
3. Lambda validates and sends to Kinesis
4. Kinesis stores in S3
5. CloudWatch monitors performance
6. SES notifies based on event volume/alerts

---


