# Functional Requirements

**Project:** Development of an AI-powered chatbot for customer support
**Responsible:** Karakat — System Analyst  
**Status:** Initial Requirements (Pre-Defense 1)

## 1. Purpose

This document describes the main functions planned for the AI-powered customer support chatbot. The system is designed to support multiple businesses with separate configurations and knowledge sources.

## 2. Functional Requirements

| ID | Requirement | Priority |
|---|---|---|
| FR-01 | The system shall identify the business associated with each customer request. | High |
| FR-02 | The system shall allow an authorized business administrator to manage company-specific chatbot settings. | High |
| FR-03 | The system shall support configuration of the company name, chatbot greeting, and support rules. | High |
| FR-04 | The system shall support business-specific knowledge sources, such as FAQs or documents. | High |
| FR-05 | The system shall accept customer questions through a defined API. | High |
| FR-06 | The system shall process questions using the selected response-handling method. | High |
| FR-07 | The system shall return a structured response to the customer. | High |
| FR-08 | The system shall validate incoming requests and handle invalid input. | High |
| FR-09 | The system shall provide a fallback response when a reliable answer cannot be produced. | High |
| FR-10 | The system shall keep configurations and knowledge sources of different businesses separated. | High |
| FR-11 | The system should support escalation of unresolved questions to a human support operator. | Medium |
| FR-12 | The system should provide a simple interface for configuring and testing chatbot behavior. | Medium |

## 3. Main User Roles

**Business Administrator:** Manages chatbot settings and business-specific knowledge sources.

**Customer:** Sends questions and receives chatbot responses.

**Support Operator:** Handles questions that cannot be resolved automatically, when escalation is supported.

## 4. Main Workflow

1. A customer submits a question.
2. The system identifies the relevant business.
3. The backend loads the business configuration.
4. The system validates the request.
5. The question is processed using the configured response method.
6. The system returns an answer or a fallback response.
7. If supported, unresolved questions can be escalated to a human operator.

## 5. Current Status

These requirements describe the planned system. Implementation details and priorities may be refined after prototype development, testing, and stakeholder feedback.
