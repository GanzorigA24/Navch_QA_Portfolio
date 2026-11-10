# Navch Android Application – Test Scenarios

**Project:** Navch QA Portfolio  
**Application:** Navch Android Application  
**Testing Type:** Manual Testing  
**Testing Approach:** Exploratory and Functional Testing  
**Environment:** Android Studio Emulator  
**Operating System:** Windows 11  
**Prepared By:** Ganzorig Arvinbileg

---

## 1. Authentication

| Scenario ID | Test Scenario | Priority |
|---|---|---|
| TS-001 | Verify that users can sign in using valid Google account credentials. | High |
| TS-002 | Verify that the application handles login attempts using an existing Google account email and password. | High |
| TS-003 | Verify that users cannot register multiple accounts using the same email address. | High |
| TS-004 | Verify that email verification is handled correctly during registration. | High |

## 2. Product Selection and Shopping Cart

| Scenario ID | Test Scenario | Priority |
|---|---|---|
| TS-005 | Verify that users can open product details and view product options. | High |
| TS-006 | Verify that the product options modal displays all elements correctly in portrait and landscape orientations. | High |
| TS-007 | Verify that users can add selected products to the shopping cart. | High |
| TS-008 | Verify that shopping cart items remain available after refreshing the application. | High |
| TS-009 | Verify that shopping cart items remain available after closing and reopening the application. | High |

## 3. Address Management

| Scenario ID | Test Scenario | Priority |
|---|---|---|
| TS-010 | Verify that users can add a new address with valid information. | High |
| TS-011 | Verify that newly saved addresses appear immediately in the address list. | Medium |
| TS-012 | Verify that the address form validates invalid phone number inputs. | High |
| TS-013 | Verify that the address form remains usable in landscape orientation. | Medium |
| TS-014 | Verify that the address form handles accidental dismissal without unexpected data loss. | Medium |

## 4. Checkout and Payment

| Scenario ID | Test Scenario | Priority |
|---|---|---|
| TS-015 | Verify that users can navigate through the checkout process. | High |
| TS-016 | Verify that back navigation from the payment page returns users to the correct previous page. | Medium |
| TS-017 | Verify that users can select an available payment method. | High |

## 5. User Profile

| Scenario ID | Test Scenario | Priority |
|---|---|---|
| TS-018 | Verify that profile input fields remain visible when the keyboard is displayed. | Medium |
| TS-019 | Verify that users can update their profile information. | High |
| TS-020 | Verify that updated profile information remains saved after closing and reopening the application. | High |

## 6. Test Scenario Summary

| Category | Number of Scenarios |
|---|---:|
| Authentication | 4 |
| Product Selection and Shopping Cart | 5 |
| Address Management | 5 |
| Checkout and Payment | 3 |
| User Profile | 3 |
| **Total** | **20** |

---

## 7. Conclusion

A total of 20 test scenarios have been identified for the Navch Android application.

These scenarios cover the application's main user workflows, including authentication, product selection, shopping cart functionality, address management, checkout, payment, and profile management.

The scenarios will be used as the foundation for creating detailed test cases and executing functional tests.