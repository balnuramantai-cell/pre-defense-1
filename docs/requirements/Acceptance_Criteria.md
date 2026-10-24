# Acceptance Criteria

**Project:** Development of an AI-powered chatbot for customer support
**Responsible:** Karakat — System Analyst  
**Status:** Proposed Acceptance Criteria (Pre-Defense 1)

## 1. Purpose

This document defines how the planned chatbot functions will be checked during development and testing.

## 2. Acceptance Criteria

| ID | Related Requirement | Acceptance Criterion |
|---|---|---|
| AC-01 | FR-01 | Given a valid business identifier, the system loads the configuration associated with that business. |
| AC-02 | FR-02, FR-03 | An authorized administrator can change supported chatbot settings, and the updated settings are used in later requests. |
| AC-03 | FR-04 | The system can access a configured business-specific knowledge source when the selected response method requires it. |
| AC-04 | FR-05 | The API accepts a correctly formatted customer question and returns a response. |
| AC-05 | FR-06, FR-07 | A valid customer request produces a structured answer or an appropriate fallback result. |
| AC-06 | FR-08 | Missing or invalid required fields produce a clear error response without crashing the application. |
| AC-07 | FR-09 | When the system cannot produce a reliable answer, it returns the configured fallback instead of presenting unsupported information as fact. |
| AC-08 | FR-10 | Requests associated with Business A cannot retrieve the configuration or knowledge sources of Business B. |
| AC-09 | FR-11 | If escalation is implemented, an unresolved request can be passed to the defined human-support workflow. |
| AC-10 | NFR-04 | If an external AI service becomes unavailable, the application handles the failure and returns a controlled error or fallback response. |
| AC-11 | NFR-09 | The team can run documented tests and record their results. |
| AC-12 | NFR-10 | Another team member can follow the setup instructions to start and test the prototype. |

## 3. Planned Testing Methods

**Functional Testing:** Check API inputs, outputs, configuration changes, and fallback behavior.

**Integration Testing:** Check communication between the backend, business configuration, and the selected response service.

**Security Testing:** Check that different businesses cannot access each other's information.

**Response Quality Evaluation:** Use a prepared set of customer questions and expected answers.

**Performance Testing:** Measure response time and compare it with a documented baseline.

## 4. Acceptance Status

All criteria are currently proposed and have not yet been verified.

Each criterion will be marked as Passed, Failed, or Not Tested after the corresponding functionality has been implemented and evaluated.
