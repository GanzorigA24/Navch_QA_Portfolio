# Navch Android Application – Test Plan

**Project:** Navch QA Portfolio  
**Application:** Navch Android Application  
**Testing Type:** Manual Application Testing  
**Testing Approach:** Exploratory Testing and Functional Testing  
**Prepared By:** Ganzorig Arvinbileg  
**Platform:** Android  
**Environment:** Android Studio Emulator  
**Operating System:** Windows 11  

---

## 1. Introduction

This document describes the test plan for the Navch Android application. The purpose of this project is to evaluate the application's functionality and usability through manual testing.

Exploratory testing was performed to identify potential defects and issues in different parts of the application. The findings from this testing were used to create structured test scenarios, detailed test cases, and bug reports.

## 2. Testing Objectives

The main objectives of this project are:

- Verify that the application's main features work as expected.
- Identify functional and user interface defects.
- Evaluate the application's behavior in different screen orientations.
- Test input validation and error handling.
- Verify data persistence after refreshing or restarting the application.
- Evaluate navigation between different pages.
- Identify usability issues that may affect the user experience.
- Document defects with clear reproduction steps and expected results.

## 3. Scope of Testing

### 3.1 In Scope

The following application features are included in testing:

| Feature | Testing Focus |
|---|---|
| Authentication | Login, registration, and account validation |
| Product Selection | Product details and product options |
| Shopping Cart | Adding items and cart persistence |
| Checkout | Checkout navigation and functionality |
| Address Management | Adding and saving addresses |
| Payment | Payment method selection and interaction |
| User Profile | Editing and saving profile information |
| User Interface | Layout, screen orientation, and keyboard behavior |
| Navigation | Back navigation and page transitions |
| Input Validation | Handling valid and invalid user inputs |

### 3.2 Out of Scope

The following areas are excluded from this testing project:

- Performance and load testing.
- Security penetration testing.
- Backend API testing.
- Database-level testing.
- Payment gateway security and real financial transactions.
- Compatibility testing across multiple physical Android devices.
- Automated testing.

## 4. Testing Approach

The project uses manual testing techniques to evaluate the application's behavior.

### 4.1 Exploratory Testing

Exploratory testing was performed without following predefined test cases. The tester explored application features, interacted with different elements, and identified unexpected behavior.

### 4.2 Functional Testing

Functional testing verifies whether application features work according to their expected behavior.

### 4.3 Negative Testing

Negative testing checks how the application handles invalid inputs, unexpected actions, and incorrect user behavior.

### 4.4 UI Testing

UI testing evaluates the application's layout, visibility, responsiveness, and usability.

## 5. Test Environment

| Component | Configuration |
|---|---|
| Application | Navch Android Application |
| Device | Android Emulator |
| Testing Tool | Android Studio |
| Operating System | Windows 11 |
| Network | Wi-Fi |
| Testing Type | Manual Testing |
| Testing Approach | Exploratory and Functional Testing |

## 6. Test Deliverables

The following documents were created as part of this project:

1. Test Plan
2. Test Scenarios
3. Detailed Test Cases
4. Bug Reports
5. Test Execution Report

## 7. Entry Criteria

Testing can begin when:

- The application is available and can be launched.
- The Android emulator is configured.
- The tester has access to the application's main features.
- A suitable network connection is available.

## 8. Exit Criteria

Testing is considered complete when:

- Planned test scenarios have been documented.
- Detailed test cases have been created and evaluated.
- Identified defects have been documented.
- Test execution results have been recorded.
- The test execution report has been completed.

## 9. Risks and Limitations

Potential risks and limitations include:

- Application crashes may interrupt testing.
- Network issues may affect application behavior.
- Some features may depend on backend services.
- Testing is limited to an Android emulator.
- Application behavior may differ on physical devices.
- Some defects may be difficult to reproduce consistently.

## 10. Conclusion

This test plan establishes the scope, objectives, approach, and environment for testing the Navch Android application.

The project demonstrates practical manual QA testing skills through exploratory testing, functional testing, test case development, defect documentation, and test execution reporting.

The results are organized and maintained in this GitHub QA portfolio.