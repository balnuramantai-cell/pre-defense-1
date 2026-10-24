# Non-Functional Requirements

**Project:** Development of a Configurable AI-Powered Customer Support Chatbot  
**Responsible:** Karakat — System Analyst  
**Status:** Initial Requirements (Pre-Defense 1)

## 1. Purpose

This document describes the expected quality, security, usability, and reliability of the chatbot platform.

## 2. Non-Functional Requirements

| ID | Requirement | Priority |
|---|---|---|
| NFR-01 | The system shall prevent one business from accessing another business's configuration and knowledge sources. | High |
| NFR-02 | Administrative operations shall require appropriate authorization. | High |
| NFR-03 | The system shall validate incoming data and handle invalid requests safely. | High |
| NFR-04 | The system shall handle backend or AI-service errors without exposing sensitive technical information to customers. | High |
| NFR-05 | The system shall provide a consistent API response format for successful and unsuccessful requests. | High |
| NFR-06 | The chatbot interface should be simple and understandable for customers. | Medium |
| NFR-07 | Business configuration should be manageable without modifying the application source code. | High |
| NFR-08 | The system should use a modular architecture that supports future improvements. | Medium |
| NFR-09 | The system shall support testing of response correctness, reliability, and response time. | High |
| NFR-10 | Technical documentation shall explain how to configure, run, and test the prototype. | High |

## 3. Performance Evaluation

Response time will be measured during prototype testing.

The team will record response times for a defined set of test questions and compare the results with a baseline response-handling method.

A final acceptable response-time threshold will be selected after initial measurements.

## 4. Security Considerations

The system design will consider:

- Separation of business-specific data.
- Secure management of configuration values and API credentials.
- Input validation.
- Access restrictions for administrative functions.
- Safe handling of errors and unavailable services.

## 5. Current Status

These requirements are planned quality goals. Their implementation and verification will be documented during development and testing.
