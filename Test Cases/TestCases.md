# Navch Android App – Detailed Test Cases

**Application:** Navch Android App  
**Testing Type:** Manual Functional Testing  
**Environment:** Android Studio Emulator  
**Computer OS:** Windows 11  

---

## 1. Authentication

### TC-001: Login with Google Account

**Test Scenario:** TS-001 – Google Login

**Preconditions:**
- The Navch app is installed and running.
- The user has a valid Google account.

**Test Steps:**
1. Open the Navch app.
2. Select the Google sign-in option.
3. Choose a Google account.
4. Complete the sign-in process.

**Expected Result:** The user should successfully log in and access the application.

**Actual Result:** The user successfully signed in using a Google account.

**Status:** Passed

---

### TC-002: Login Using an Existing Google Account's Email and Password

**Test Scenario:** TS-002 – Login with Existing Google Email and Password

**Preconditions:**
- An account has already been created using Google sign-in.
- The user is on the login screen.

**Test Steps:**
1. Open the login screen.
2. Enter the email address associated with the Google account.
3. Enter the account password.
4. Select the login button.

**Expected Result:** The application should recognize the existing account and allow the user to log in with valid credentials, or clearly explain the supported login method.

**Actual Result:** The application displayed an "Invalid credentials" message even though the email belonged to an existing Google account.

**Status:** Failed

**Related Bug:** NAVCH-002

---

### TC-003: Register Using an Existing Email Address

**Test Scenario:** TS-003 – Duplicate Account Registration

**Preconditions:**
- An account already exists with the email address being tested.
- The user is on the registration screen.

**Test Steps:**
1. Open the registration screen.
2. Enter an email address already associated with an account.
3. Complete the required registration fields.
4. Submit the registration form.

**Expected Result:** The application should recognize the existing email and display a message explaining that the account already exists.

**Actual Result:** The application did not provide a clear duplicate-account warning.

**Status:** Failed

**Related Bug:** NAVCH-002

---

### TC-004: Verify Email After Registration

**Test Scenario:** TS-004 – Email Verification

**Preconditions:**
- The user has completed the registration process.
- Access to the registered email account is available.

**Test Steps:**
1. Register a new account.
2. Submit the registration form.
3. Check the registered email inbox.
4. Check the spam or junk folder if necessary.

**Expected Result:** The application should send an email verification message when email verification is required.

**Actual Result:** No verification email was received.

**Status:** Failed

**Related Bug:** NAVCH-002

---

## 2. Product and Shopping Cart

### TC-005: View Product Details and Options

**Test Scenario:** TS-005 – View Product Details and Options

**Preconditions:**
- The Navch app is open.
- Products are available.

**Test Steps:**
1. Open the product listing.
2. Select a product.
3. Open the product details or options section.
4. Review the available product information and options.

**Expected Result:** The application should display the selected product's details and available options.

**Actual Result:** The product details and options were accessible during testing.

**Status:** Passed

---

### TC-006: Check Product Options Modal in Landscape Mode

**Test Scenario:** TS-006 – Product Modal in Landscape Mode

**Preconditions:**
- The app is open.
- A product with selectable options is available.

**Test Steps:**
1. Select a product.
2. Open its options modal.
3. Rotate the emulator to landscape mode.
4. Check whether all modal content and the add-to-cart button are accessible.

**Expected Result:** The modal should adjust to landscape mode. All options and the add-to-cart button should remain visible or be accessible through scrolling.

**Actual Result:** The modal did not support scrolling in landscape mode. The add-to-cart button became hidden and inaccessible.

**Status:** Failed

**Related Bug:** NAVCH-001

---

### TC-007: Add a Product to the Shopping Cart

**Test Scenario:** TS-007 – Add Product to Cart

**Preconditions:**
- The app is open.
- At least one product is available.

**Test Steps:**
1. Select a product.
2. Choose the required product options.
3. Select the add-to-cart button.
4. Open the shopping cart.

**Expected Result:** The selected product should be added to the shopping cart and displayed correctly.

**Actual Result:** Products could be added to the shopping cart during testing. However, cart items were not consistently retained after refreshing or restarting the app.

**Status:** Passed

**Related Bug:** NAVCH-003 (Cart persistence issue is covered separately.)

---

### TC-008: Verify Cart Items After Refreshing the App

**Test Scenario:** TS-008 – Cart Persistence After Refresh

**Preconditions:**
- At least one product has been added to the cart.

**Test Steps:**
1. Add a product to the shopping cart.
2. Refresh the app.
3. Open the shopping cart.
4. Check whether the previously added product is still displayed.
5. Add another product and refresh again.

**Expected Result:** All previously added products should remain in the shopping cart after refreshing.

**Actual Result:** Some previously added products remained after refreshing, but newly added products disappeared.

**Status:** Failed

**Related Bug:** NAVCH-003

---

### TC-009: Verify Cart Items After Restarting the App

**Test Scenario:** TS-009 – Cart Persistence After App Restart

**Preconditions:**
- At least one product has been added to the cart.

**Test Steps:**
1. Add one or more products to the cart.
2. Close the Navch app completely.
3. Reopen the app.
4. Open the shopping cart.
5. Check whether the previously added products remain.

**Expected Result:** The shopping cart should retain its items after the application is restarted.

**Actual Result:** The previously added cart items were lost after restarting the application.

**Status:** Failed

**Related Bug:** NAVCH-003

---

## 3. Address Management

### TC-010: Add a New Delivery Address

**Test Scenario:** TS-010 – Add New Address

**Preconditions:**
- The user is logged in.
- The address management section is accessible.

**Test Steps:**
1. Open the address management section.
2. Select the option to add a new address.
3. Enter the required address information.
4. Select the save button.
5. Navigate away from the address section and return to it.

**Expected Result:** The application should save the new address successfully.

**Actual Result:** The address was saved but did not appear immediately after saving. It appeared after navigating away and reopening the address section.

**Status:** Passed

**Related Bug:** NAVCH-004 (Immediate display issue is covered separately.)

---

### TC-011: Verify Newly Saved Address Appears Immediately

**Test Scenario:** TS-011 – Newly Saved Address Display

**Preconditions:**
- The user is logged in.
- The address management section is accessible.

**Test Steps:**
1. Open the address management section.
2. Add a new delivery address.
3. Enter all required information.
4. Select the save button.
5. Check the address list immediately after saving.

**Expected Result:** The newly saved address should appear in the address list immediately.

**Actual Result:** The newly saved address did not appear immediately. It became visible only after navigating away and reopening the section.

**Status:** Failed

**Related Bug:** NAVCH-004

---

### TC-012: Validate Special Characters in the Phone Number Field

**Test Scenario:** TS-012 – Invalid Phone Number Validation

**Preconditions:**
- The user is logged in.
- The add-address form is open.

**Test Steps:**
1. Open the checkout section.
2. Select the option to add a new address.
3. Enter special characters in the phone number field.
4. Attempt to save the address.

**Expected Result:** The application should validate the phone number and display an appropriate error message without crashing.

**Actual Result:** The application crashed after special characters were entered in the phone number field and the form was submitted.

**Status:** Failed

**Related Bug:** NAVCH-005

---

### TC-013: Check Address Form Accessibility in Landscape Mode

**Test Scenario:** TS-013 – Address Form in Landscape Mode

**Preconditions:**
- The user is logged in.
- The add-address form is open.

**Test Steps:**
1. Open the add-address form.
2. Rotate the emulator to landscape mode.
3. Check whether all form fields are accessible.
4. Attempt to scroll through the form.

**Expected Result:** The address form should adjust to landscape mode and allow the user to access all fields.

**Actual Result:** The form did not support scrolling properly in landscape mode, making some fields difficult or impossible to access.

**Status:** Failed

**Related Bug:** NAVCH-006

---

### TC-014: Check Whether the Address Form Closes When Tapping Outside

**Test Scenario:** TS-014 – Accidental Address Form Dismissal

**Preconditions:**
- The user is logged in.
- The add-address form is open.

**Test Steps:**
1. Open the add-address form.
2. Enter some address information.
3. Tap outside the form.
4. Check whether the form closes and whether the entered information is retained.

**Expected Result:** The form should not close unexpectedly without warning or confirmation. Entered information should not be lost accidentally.

**Actual Result:** The form closed when the user tapped outside it, causing the entered information to be lost.

**Status:** Failed

**Related Bug:** NAVCH-006

---

## 4. Checkout and Payment

### TC-015: Navigate to the Checkout Section

**Test Scenario:** TS-015 – Checkout Navigation

**Preconditions:**
- The user is logged in.
- At least one product is available in the shopping cart.

**Test Steps:**
1. Open the shopping cart.
2. Select the checkout option.
3. Continue through the checkout process.
4. Check whether the checkout and payment sections can be accessed.

**Expected Result:** The application should allow the user to navigate through the checkout process.

**Actual Result:** The checkout process was accessible, and the payment section could be reached.

**Status:** Passed

---

### TC-016: Verify Back Navigation from the Payment Section

**Test Scenario:** TS-016 – Back Navigation from Payment

**Preconditions:**
- The user has entered the checkout process.
- The payment section is open.
- An address has been selected.

**Test Steps:**
1. Navigate to the payment section.
2. Select the back navigation option.
3. Check which screen is displayed.
4. Verify whether the previously selected address remains accessible.

**Expected Result:** The application should return to the previous checkout step, such as address selection.

**Actual Result:** Back navigation from the payment section skipped the address selection step and returned the user directly to the shopping cart.

**Status:** Failed

**Related Bug:** NAVCH-007

---

### TC-017: Select a Payment Method

**Test Scenario:** TS-017 – Payment Method Selection

**Preconditions:**
- The user is logged in.
- The checkout process has reached the payment section.

**Test Steps:**
1. Open the payment section.
2. Review the available payment methods.
3. Select a payment option.
4. Check whether the selected payment method is activated.

**Expected Result:** The user should be able to select an available payment method.

**Actual Result:** The payment options were unresponsive and could not be selected.

**Status:** Failed

**Related Bug:** NAVCH-008

---

## 5. User Profile

### TC-018: Check Profile Field Visibility When the Keyboard Is Open

**Test Scenario:** TS-018 – Profile Field Visibility with Keyboard

**Preconditions:**
- The user is logged in.
- The profile section is accessible.

**Test Steps:**
1. Open the profile section.
2. Select an editable input field.
3. Allow the keyboard to appear.
4. Check whether the selected field and other relevant content remain visible.

**Expected Result:** The application should adjust its layout so that input fields remain visible when the keyboard is open.

**Actual Result:** The keyboard covered the profile input field, making it difficult to view and edit.

**Status:** Failed

**Related Bug:** NAVCH-009

---

### TC-019: Update User Profile Information

**Test Scenario:** TS-019 – Update Profile Information

**Preconditions:**
- The user is logged in.
- The profile section is accessible.

**Test Steps:**
1. Open the profile section.
2. Select an editable profile field.
3. Enter updated information.
4. Save the changes.
5. Check whether the updated information is displayed.

**Expected Result:** The application should save and display the updated profile information.

**Actual Result:** Profile updates were not reliably retained. The previously saved information returned after the application was restarted.

**Status:** Failed

**Related Bug:** NAVCH-010

---

### TC-020: Verify Profile Information After Restarting the App

**Test Scenario:** TS-020 – Profile Persistence After App Restart

**Preconditions:**
- The user is logged in.
- The profile information has been updated.

**Test Steps:**
1. Update the user's profile information.
2. Save the changes.
3. Close the Navch app completely.
4. Reopen the application.
5. Open the profile section.
6. Check whether the updated information is still displayed.

**Expected Result:** The updated profile information should remain saved after restarting the application.

**Actual Result:** The previously saved profile information was displayed instead of the updated information.

**Status:** Failed

**Related Bug:** NAVCH-010

---

## 6. Test Execution Summary

| Result | Number of Test Cases |
|---|---:|
| Passed | 4 |
| Failed | 16 |
| Not Executed | 0 |
| **Total** | **20** |

**Overall Result:** 20 test cases were documented based on the manual exploratory testing performed on the Navch Android application. Four test cases passed, while sixteen failed due to the issues identified during testing.

**Note:** Some test cases are related to the same reported bug. The related bug IDs are included to connect test results with the corresponding bug reports.