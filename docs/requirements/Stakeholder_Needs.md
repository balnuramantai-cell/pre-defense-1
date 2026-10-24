# Stakeholder Needs

**Project:** Development of an AI-powered chatbot for customer support
**Responsible:** Karakat — System Analyst, Karina — Project Manager  
**Status:** Preliminary Stakeholder Analysis (Pre-Defense 1)

## 1. Purpose

This document identifies the main stakeholders of the proposed chatbot platform and describes their expected needs.

The analysis is based on the initial project proposal and preliminary requirements-gathering materials.

## 2. Main Stakeholders

| Stakeholder | Main Needs |
|---|---|
| Business Owner | A customer support solution that can be adapted to the business without extensive technical work. |
| Business Administrator | Simple configuration of chatbot settings, greetings, support rules, and knowledge sources. |
| Customer | Quick, understandable, and relevant answers to common questions. |
| Support Operator | A way to handle questions that the chatbot cannot answer reliably. |
| Development Team | Clear requirements, modular architecture, testable functions, and documented interfaces. |
| Academic Supervisor | Evidence of research, requirements analysis, implementation progress, testing, and team contributions. |

## 3. Preliminary Problems Identified

The initial requirements-gathering materials identify three main concerns.

**Problem 1: Complex Setup**

Businesses may find it difficult to configure a customer support chatbot without technical assistance.

**Proposed Need:** Simple configuration of business information and chatbot behavior.

**Problem 2: Limited Flexibility**

Different businesses require different information, rules, and customer support responses.

**Proposed Need:** Separate configurations and knowledge sources for each business.

**Problem 3: Difficult Handling of Complex Questions**

Some customer questions cannot be answered reliably through automated responses.

**Proposed Need:** Clear fallback behavior and a possible escalation process.

## 4. Requirements Derived from Stakeholder Needs

| Need ID | Stakeholder Need | Related Requirements |
|---|---|---|
| SN-01 | Easy chatbot configuration | FR-02, FR-03 |
| SN-02 | Business-specific information | FR-04, FR-10 |
| SN-03 | Customer question answering | FR-05, FR-06, FR-07 |
| SN-04 | Reliable handling of unknown questions | FR-09 |
| SN-05 | Human support for unresolved requests | FR-11 |
| SN-06 | Secure separation of business data | FR-10, NFR-01 |
| SN-07 | Simple customer interaction | FR-12, NFR-06 |

## 5. Validation Plan

The preliminary needs should be reviewed through additional stakeholder discussions or feedback from a potential business user.

The team plans to clarify:

- Which chatbot settings are most important for business administrators.
- What knowledge sources businesses need.
- Which questions should be handled automatically.
- When human support is necessary.
- What makes the chatbot easy to use.

## 6. Limitations

The available preliminary report does not provide documented interview dates, participant details, or verbatim interview responses. Therefore, these needs are treated as preliminary findings rather than confirmed results from a completed interview study.

## 7. Conclusion

The main stakeholder needs are simple configuration, business-specific responses, reliable question handling, and secure separation of business information. These needs will guide system design, implementation, and evaluation.
