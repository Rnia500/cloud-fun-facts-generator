# Cloud Fun Facts Generator

A serverless cloud application built on AWS that fetches cloud computing facts and makes them witty using generative AI.

## Architecture & Tech Stack
* **Frontend**: HTML/JS hosted or run locally, interacting with API Gateway / Lambda.
* **AWS Lambda**: Serverless Python function (`lambda_function.py`) handling core logic.
* **Amazon DynamoDB**: NoSQL table named **`CloudFacts`** with a primary key attribute **`FactText`**.
* **Amazon Bedrock**: Uses **Claude Sonnet 4.5** (`eu.anthropic.claude-sonnet-4-5-20250929-v1:0`) via an EU cross-region inference profile to rewrite facts.
