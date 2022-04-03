## Amazon API Gateway

Amazon API Gateway => is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale.
APIs act as the "front door" for applications to access data, business logic, or functionality from your backend services. Using API Gateway, you can 
create RESTful APIs and WebSocket APIs that enable real-time two-way communication applications. API Gateway supports containerized and serverless workloads, 
as well as web applications.

API Gateway handles all the tasks involved in accepting and processing up to hundreds of thousands of 
concurrent API calls, including traffic management, CORS support, authorization and access control, throttling, monitoring, and API version management. 
API Gateway has no minimum fees or startup costs. You pay for the API calls you receive and the amount of data transferred out and, with the API Gateway 
tiered pricing model, you can reduce your cost as your API usage scales.

## API Types

- RESTful APIs
Build RESTful APIs optimized for serverless workloads and HTTP backends using HTTP APIs. HTTP APIs are the best choice for building APIs that only
require API proxy functionality. If your APIs require API proxy functionality and API management features in a single solution, API Gateway also offers
REST APIs. 
- WEBSOCKET APIs
Build real-time two-way communication applications, such as chat apps and streaming dashboards, with WebSocket APIs. API Gateway maintains a persistent
connection to handle message transfer between your backend service and your clients.

## Amazon DynamoDB

Amazon DynamoDB is a fully managed, serverless, key-value NoSQL database designed to run high-performance applications at any scale. DynamoDB offers built-in
security, continuous backups, automated multi-Region replication, in-memory caching, and data export tools.

## Dynamoose
Dynamoose is a modeling tool for Amazon's DynamoDB. Dynamoose is heavily inspired by Mongoose, which means if you are coming from Mongoose the syntax will 
be very familar.
