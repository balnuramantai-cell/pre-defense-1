# Verification and Evaluation Plan

**Project:** Development of an AI-powered chatbot for customer support

**Responsible:** Karakat — System Analyst, Balnur — Developer

**Status:** Planned (Pre-Defense 1)

## 1. Purpose

The purpose of this document is to describe how the chatbot system will be tested and evaluated. The evaluation will focus on functionality, response quality, reliability, security, and performance.

## 2. Verification Objectives

The main objectives are:

- Verify that the chatbot accepts and processes customer questions correctly.
- Check that each business uses its own configuration and knowledge sources.
- Evaluate the correctness and relevance of chatbot answers.
- Test fallback behavior when the chatbot cannot answer a question.
- Check system performance and error handling.
- Verify that the API works according to the documented requirements.

## 3. Testing Methods

| Test Type | Description | Expected Result |
|---|---|---|
| Functional Testing | Test the main chatbot functions. | Functions work according to requirements. |
| API Testing | Send valid and invalid requests to the backend. | Correct responses and error messages. |
| Integration Testing | Test interaction between the backend, business configuration, and response service. | Components exchange data correctly. |
| Security Testing | Check business data separation and access restrictions. | One business cannot access another business's information. |
| Performance Testing | Measure response time for customer questions. | Response time is recorded and evaluated against the baseline. |
| Response Quality Testing | Compare chatbot answers with expected answers. | Answers are relevant, correct, and supported by available information. |
| Fallback Testing | Ask questions that cannot be answered using available knowledge. | The system returns an appropriate fallback response. |

## 4. Planned Test Scenarios

| ID | Test Scenario | Expected Result |
|---|---|---|
| TC-01 | Submit a valid customer question. | The chatbot returns a structured response. |
| TC-02 | Submit an empty question. | The system returns a validation error. |
| TC-03 | Use an invalid business identifier. | The system rejects the request safely. |
| TC-04 | Ask a question using Business A's knowledge source. | The answer uses the correct business information. |
| TC-05 | Attempt to access Business B's information through Business A. | Access is prevented. |
| TC-06 | Ask a question outside the available knowledge. | The chatbot returns a fallback response. |
| TC-07 | Simulate an unavailable AI service. | The system handles the error without crashing. |
| TC-08 | Change a supported business configuration. | Subsequent requests use the updated settings. |

## 5. Baseline Comparison

The project will use a simple FAQ-based response method as a proposed baseline.

The team will prepare a test dataset containing common customer support questions and expected answers.

The baseline and the selected chatbot response method will be evaluated using the same test questions.

The comparison will consider:

- Answer correctness.
- Answer relevance.
- Fallback behavior.
- Response time.

The final response-generation method has not yet been confirmed. Direct LLM responses and Retrieval-Augmented Generation (RAG) are possible approaches for further evaluation.

## 6. Evaluation Metrics

| Metric | Measurement Method |
|---|---|
| Answer Accuracy | Percentage of test questions answered correctly. |
| Response Time | Time between submitting a question and receiving a response. |
| Fallback Correctness | Percentage of unsupported questions handled with an appropriate fallback. |
| API Test Pass Rate | Percentage of API tests completed successfully. |
| Business Isolation | Number of detected cross-business information access failures. |

The team will define the final test dataset size and numerical acceptance thresholds after initial prototype measurements.

## 7. Testing Tools

The planned tools include:

- Python for automated testing.
- Pytest as a candidate framework for backend tests.
- FastAPI testing utilities if FastAPI is selected.
- Manual test cases for chatbot responses and usability.
- GitHub for storing test code and results.
- YouTrack for tracking testing tasks and identified defects.

## 8. Team Responsibilities

**Karakat — System Analyst**
- Define test scenarios.
- Check that tests cover the documented requirements.
- Evaluate answer relevance and correctness.

**Balnur — Developer**
- Implement automated tests.
- Test API endpoints and system components.
- Measure response times.
- Fix technical defects.

**Karina — Project Manager**
- Monitor testing progress in YouTrack.
- Track defects and deadlines.
- Review completion of planned evaluation activities.

## 9. Expected Deliverables

The evaluation process is expected to produce:

- Documented test cases.
- Automated test scripts where applicable.
- Test execution results.
- Response quality comparison.
- Performance measurements.
- A summary of detected problems and improvements.

## 10. Current Status

At the first pre-defense stage, this document describes the planned verification and evaluation activities.

No completed testing results are claimed in this plan. Actual measurements and test outcomes will be added after the corresponding prototype functions are implemented.

## 11. Conclusion

The verification and evaluation plan will help the team assess whether the chatbot meets its functional and non-functional requirements. Testing will also identify limitations and support improvements during further development.
