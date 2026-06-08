🚀 Event-Driven Order Processing System

An event-driven workflow automation project built with n8n that demonstrates producer-consumer architecture using webhooks, HTTP requests, scheduled triggers, and conditional business logic.

📌 Overview

This project simulates a real-world order processing system where multiple workflows communicate through APIs and webhooks.

The system consists of three interconnected workflows:

Producer Workflow
Consumer Workflow
Scheduled Processing Workflow

Together, these workflows automate order creation, processing, validation, and response handling.

🏗️ Architecture
Producer Workflow

The Producer Workflow initiates order requests and sends them to the Consumer Workflow through an HTTP request.

Functions:

Generates order data
Sends orders via HTTP POST
Receives processing confirmation
Validates response status
Handles success and failure scenarios
Consumer Workflow

The Consumer Workflow acts as an API endpoint using a webhook.

Functions:

Receives incoming order requests
Extracts order information
Adds processing metadata
Generates timestamps
Returns confirmation responses
Scheduled Workflow

The Scheduled Workflow automatically executes every 30 minutes.

Functions:

Performs automated health checks
Creates scheduled batch orders
Executes only during business hours
Prevents processing outside allowed time windows
⚙️ Workflow Components
Producer Workflow
Manual Trigger
HTTP Request
Conditional Logic (IF Node)
Response Handling
Data Transformation
Consumer Workflow
Webhook Trigger
Data Processing
Metadata Enrichment
Response to Webhook
Scheduled Workflow
Schedule Trigger
Business Hour Validation
Batch Order Creation
Automated Processing
🛠 Tech Stack
n8n
Webhooks
HTTP APIs
JSON
Workflow Automation
Event-Driven Architecture
🎯 Features

✅ Producer-Consumer Architecture

✅ Webhook-Based Communication

✅ HTTP API Integration

✅ Scheduled Automation

✅ Business Hour Validation

✅ Automated Order Processing

✅ Error Handling

✅ Conditional Routing

✅ Workflow Orchestration

🔄 Workflow Flow
Manual Processing
User executes Producer Workflow
Order data is generated
HTTP request is sent to Consumer Workflow
Consumer processes order
Confirmation response is returned
Producer validates response
Scheduled Processing
Schedule Trigger executes every 30 minutes
Business hours are checked
Batch order is generated
Order is sent to Consumer Workflow
Processing confirmation is returned
📷 Workflow Screenshots

Add screenshots of:

Producer Workflow
<img width="1425" height="508" alt="Workflow A the producer" src="https://github.com/user-attachments/assets/c97bbef6-16bc-4c7e-a0b9-aae53b30b422" />


Consumer Workflow
<img width="1445" height="728" alt="Consumer Workflow" src="https://github.com/user-attachments/assets/9a44621a-63f7-4764-b1bd-c7923665f4bd" />

Scheduled Workflow
<img width="1392" height="720" alt="Scheduled Workflow" src="https://github.com/user-attachments/assets/66838b47-63f8-49df-accd-d362fcd64c5e" />


Example:

screenshots/
├── producer-workflow.png
├── consumer-workflow.png
└── scheduled-workflow.png
🚀 Getting Started
Prerequisites
n8n installed locally or on cloud
Active n8n instance
Webhook endpoint configured
Installation
Clone the repository
git clone https://github.com/Maaz708/event-driven-order-processing-system.git
Import all workflow JSON files into n8n
Activate the Consumer Workflow webhook
Update webhook URLs if required
Execute the Producer Workflow
📚 Key Concepts Demonstrated
Event-Driven Architecture
API Communication
Webhook Integration
Producer-Consumer Pattern
Workflow Automation
Business Logic Implementation
Scheduled Processing
Backend System Design
🎓 Learning Outcomes

Through this project I gained practical experience in:

Designing distributed workflow systems
Implementing webhook-based communication
Automating business processes
Building event-driven architectures
Handling API responses and validation
Creating scalable automation pipelines
👨‍💻 Author

Mohd Maaz

LinkedIn:
https://www.linkedin.com/in/mohd-maaz-1277121b1

GitHub:
https://github.com/Maaz708
