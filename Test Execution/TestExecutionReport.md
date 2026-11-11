# Navch Android App – Test Execution Report

## 1. Project Information

| Item | Details |
|---|---|
| Application | Navch Android App |
| Testing Type | Manual Functional Testing |
| Testing Environment | Android Studio Emulator |
| Computer OS | Windows 11 |
| Total Test Cases | 20 |
| Testing Approach | Manual and Exploratory Testing |

## 2. Testing Objective

The objective of this testing was to evaluate the main features and functionality of the Navch Android application.

The testing focused on identifying functional issues, usability problems, navigation errors, and unexpected application behavior.

## 3. Testing Scope

The following application areas were tested:

- User authentication and registration
- Product details and product options
- Shopping cart functionality
- Cart item persistence
- Address management
- Input validation
- Checkout navigation
- Payment method selection
- User profile management
- Application behavior in landscape mode

## 4. Test Execution Summary

A total of 20 test cases were documented and evaluated.

| Test Result | Total | Percentage |
|---|---:|---:|
| Passed | 5 | 25% |
| Failed | 15 | 75% |
| Not Executed | 0 | 0% |
| **Total** | **20** | **100%** |

## 5. Test Results by Module

| Module | Total | Passed | Failed |
|---|---:|---:|---:|
| Authentication | 4 | 1 | 3 |
| Product and Shopping Cart | 5 | 2 | 3 |
| Address Management | 5 | 1 | 4 |
| Checkout and Payment | 3 | 1 | 2 |
| User Profile | 3 | 0 | 3 |
| **Total** | **20** | **5** | **15** |

## 6. Identified Issues

The following issues were identified during testing:

| Bug ID | Issue Summary | Severity | Priority |
|---|---|---|---|
| NAVCH-001 | Add-to-cart button hidden in landscape mode | High | High |
| NAVCH-002 | Inconsistent authentication behavior and missing email verification | High | High |
| NAVCH-003 | Shopping cart items not consistently saved | High | High |
| NAVCH-004 | Newly added address not displayed immediately | Medium | Medium |
| NAVCH-005 | Application crashes when entering special characters in phone number field | High | High |
| NAVCH-006 | Address form cannot be fully accessed and can close accidentally | Medium–High | Medium |
| NAVCH-007 | Back navigation from payment skips address selection | Medium | Medium |
| NAVCH-008 | Payment options are unresponsive | High | High |
| NAVCH-009 | Profile input field is hidden by keyboard | Medium | Medium |
| NAVCH-010 | Profile updates are not retained after app restart | High | High |

## 7. Main Findings

Several important problems were discovered during testing:

- Authentication behavior was inconsistent between Google sign-in and email/password login.
- Product options and address forms had layout problems in landscape mode.
- Shopping cart information was not consistently retained after refreshing or restarting the application.
- The application crashed when special characters were entered in the phone number field.
- Payment options could not be selected.
- Profile information was not reliably saved after restarting the application.

These issues could negatively affect the user experience and prevent users from completing important actions.

## 8. Recommendations

The following improvements are recommended:

1. Fix authentication and account registration behavior.
2. Improve application layouts for landscape orientation.
3. Fix shopping cart data persistence.
4. Improve address form validation and prevent accidental form dismissal.
5. Fix the application crash caused by invalid phone number input.
6. Correct checkout navigation and payment selection.
7. Improve profile data saving and persistence.
8. Improve keyboard handling on profile input fields.

## 9. Overall Conclusion

Manual and exploratory testing identified several functional and usability problems in the Navch Android application.

The most important issues were related to authentication, shopping cart persistence, application crashes, payment selection, and profile data persistence.

The application needs further improvements before it can provide a reliable user experience.

This project helped demonstrate practical QA skills, including test planning, test scenario creation, test case design, manual testing, defect identification, and test result documentation.