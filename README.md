Recruitment Workflow Automation

Python | REST APIs | Lark | Quickin | SQLite | Automated Testing**

Overview

I independently developed a process automation solution that integrates Lark Approval and Quickin through REST APIs.

The system automatically processes approved recruitment requests and creates corresponding job openings in the recruitment platform, reducing manual operations and improving data consistency.

Claude was used as an AI-assisted development tool throughout the implementation process.

Architecture

The solution follows a modular architecture:

1. Lark Integration: Retrieves approved recruitment requests.
2. Polling Mechanism: Periodically checks for new approved requests.
3. Data Mapping: Transforms form information into the destination API payload.
4. Validation Layer: Checks required fields and business rules.
5. Quickin Integration: Creates job openings through the API.
6. Persistence: Uses SQLite to track processed requests.
7. Notifications: Sends execution results through Lark.

Technical Implementation

- Python 3.11+
- REST API integration using HTTPX
- SQLite persistence
- Idempotency to prevent duplicate processing
- Retry mechanism with exponential backoff
- Structured JSON logging
- Error handling and operational notifications
- Automated testing

Engineering Decisions

Some important engineering decisions included:

- Using polling instead of relying exclusively on webhooks.
- Implementing persistent processing control with SQLite.
- Preventing duplicate job creation through idempotency.
- Validating data before submitting requests to the recruitment platform.
- Implementing controlled retries for temporary API failures.
- Using dry-run execution to prevent unintended changes.

Testing

The implementation includes 135 automated tests covering:

- Data mapping
- API behavior
- Field validation
- Persistence and idempotency
- Rate limiting and retries
- Error handling

My Contribution

I independently designed and implemented the automation using Python, with Claude as an AI-assisted development tool.

My work involved API integration, workflow design, data transformation, validation, persistence, error handling, testing and technical documentation.

Technologies

Python | HTTPX | REST APIs | SQLite | Pydantic | FastAPI | Pytest | Lark | Quickin

Confidentiality

This repository presents a sanitized technical overview of a professional project.

It does not contain proprietary source code, production credentials, real recruitment data or confidential company configurations.

The implementation shown in this documentation is not the original corporate source code.
