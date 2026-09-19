# Lectify Analytics Product Status

**Last updated:** September 2026
**Current stage:** Working prototype preparing for cloud deployment

## Overview

Lectify Analytics is an agentic AI financial-analysis system designed for finance analysts, investors and researchers. It processes public-company SEC filings, calculates multi-year financial metrics, supports peer analysis, grounds explanations in company disclosures and answers natural-language questions with independent verification of numerical claims.

The current build is a working prototype validated against live SEC EDGAR data and real language models. It operates today as a single-instance local development deployment rather than a hosted, multi-user production service.

This public document provides a high-level product-status summary. Proprietary source code, detailed implementation logic, security configuration and internal deployment documentation are intentionally not included in this repository.

## Status at a Glance

| Area                                    | Current status                                                         |
| --------------------------------------- | ------------------------------------------------------------------------ |
| SEC filing ingestion                    | Working in prototype                                                   |
| Financial-data normalization            | Working in prototype                                                   |
| Financial metric calculation            | Working in prototype                                                   |
| Natural-language financial Q&A          | Working in prototype                                                   |
| Independent numerical verification      | Working in prototype                                                   |
| Source-grounded narrative analysis      | Working in prototype                                                   |
| Peer benchmarking and anomaly detection | Working in prototype                                                   |
| Industry-wide benchmarking              | Working in prototype                                                   |
| Authentication and role-based access    | Working in prototype                                                   |
| Audit logging and administration        | Working in prototype                                                   |
| Guardrails and observability            | Implemented, with selected enforcement behaviour still being finalized |
| User interface and visualizations       | Working in prototype                                                   |
| AWS infrastructure design               | Prepared                                                                |
| Hosted AWS deployment                   | Planned                                                                 |
| Multi-user and multi-tenant operation   | Planned                                                                 |
| Production-scale processing             | Planned                                                                 |

## Working in the Current Prototype

The following capabilities have been implemented and tested:

### SEC Filing Ingestion

The system retrieves and consolidates multi-year financial information from live SEC EDGAR filings, including structured XBRL facts associated with annual and quarterly reports.

### Financial-Data Normalization

Reported financial facts are transformed into a consistent analytical structure that supports calculations across reporting periods and companies.

### Financial Metrics and Analysis

The prototype calculates financial measures covering areas such as:

* Revenue growth
* Margins
* Free cash flow
* Leverage
* Common-size financial statements
* Trends and financial anomalies

### Natural-Language Financial Q&A

Users can ask financial questions in plain English. The system routes questions to the appropriate financial-data, retrieval or comparison workflow.

### Independent Numerical Verification

Numerical claims produced during analysis are independently recalculated from structured financial facts before they are presented to the user. Claims that cannot be confirmed can be identified rather than presented as verified results.

### Source-Grounded Explanations

Narrative explanations are grounded in relevant company disclosures, including Management's Discussion and Analysis and filing footnotes. Structured numerical facts are retrieved through deterministic data access rather than similarity search.

### Peer Benchmarking

The prototype supports cross-company comparison and routes appropriate questions to its peer-analysis workflow.

### Industry-Wide Benchmarking

In addition to comparing a company against a named set of peers, the prototype classifies each company into an industry and compares it against the broader set of companies in that same industry — the industry's typical value, the range most companies fall into, and where the company ranks by percentile. This is a distinct comparison from peer benchmarking, which is scoped to a specific, user-selected set of companies. Where there isn't yet enough classified data in an industry to support a meaningful comparison, the system reports that plainly rather than presenting an incomplete one.

### Authentication and Governance

The current implementation includes:

* JWT-based authentication
* Role-based permissions
* Administrative user management
* Session revocation
* Audit-log review
* Guardrails for personally identifiable information, prompt injection and toxicity
* Tracing and monitoring across the analysis workflow

### Reports and User Interface

The prototype includes:

* A business workspace
* Natural-language Q&A
* Static company reports
* Financial visualizations
* Drill-down views

### Automated Testing

The application is supported by an automated test suite covering its data, financial-analysis, orchestration, verification, security and user-interface components.

## Current Boundaries

The prototype currently operates in a local development environment.

It has not yet been operated as:

* A publicly hosted production service
* A multi-user or multi-tenant application
* A horizontally scaled API platform
* A production-scale SEC filing-processing service

The product views and figures shown in the public demonstration are illustrative and should not be interpreted as live production data or a generally available commercial service.

Some guardrail enforcement behaviour remains under product review even though the underlying screening capabilities have been implemented.

## AWS Deployment Preparation

Infrastructure-as-code and migration planning have been prepared for the next stage of development. The intended migration will move the existing prototype from its local development environment to a secure AWS-hosted deployment.

The planned AWS deployment is expected to support:

* Scalable SEC filing ingestion and processing
* Application and workflow compute
* Amazon Bedrock model inference
* Hosted storage and retrieval
* Multi-user access
* Tenant isolation
* Secrets management
* Network and security controls
* Production logging and monitoring
* Auditability and operational oversight

The final service selection and configuration may evolve as the prototype is deployed, tested and optimized.

## Next Development Stage

The next stage is focused on:

1. Executing the prepared AWS migration
2. Moving production model inference to Amazon Bedrock
3. Deploying the application as a hosted service
4. Supporting multiple authenticated users
5. Strengthening tenant and data isolation
6. Increasing filing-processing capacity
7. Hardening monitoring, security and operational controls
8. Preparing the product for controlled pilot use

## Role of AWS Infrastructure

AWS infrastructure will help Lectify Analytics progress from a validated working prototype to a secure, hosted and scalable product.

Cloud resources will primarily support:

* Higher-volume document ingestion and processing
* Amazon Bedrock inference
* Application hosting
* Retrieval infrastructure
* Monitoring and auditability
* Security and identity controls
* Multi-user operation

## Important Notice

Lectify Analytics is under active development. This document describes the current prototype and planned direction as of the date shown above. Planned capabilities are not commitments and may change as technical validation, deployment and product development continue.

Lectify Analytics provides technology-assisted financial analysis and does not provide investment, legal, accounting or tax advice. Users remain responsible for reviewing source filings and independently evaluating information used in financial or business decisions.
