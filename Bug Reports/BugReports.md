# Navch Android App – Bug Reports

**Application:** Navch Android App  
**Testing Type:** Manual Functional Testing  
**Environment:** Android Studio Emulator  
**Computer OS:** Windows 11  

---

## NAVCH-001: Add-to-Cart Button Not Visible in Landscape Mode

**Severity:** High  
**Priority:** High  
**Module:** Product Selection

**Description:**

When the device is rotated to landscape mode while the product options modal is open, the add-to-cart button becomes hidden and cannot be accessed.

**Preconditions:**
- The Navch app is running.
- A product with selectable options is available.

**Steps to Reproduce:**
1. Open the Navch app.
2. Select a product.
3. Open the product options modal.
4. Rotate the device to landscape mode.
5. Try to locate and use the add-to-cart button.

**Expected Result:**

The modal should adjust to landscape mode. All options and the add-to-cart button should remain visible or be accessible through scrolling.

**Actual Result:**

The modal does not support scrolling in landscape mode, and the add-to-cart button becomes hidden.

**Impact:**

Users may be unable to add products to their shopping cart when using landscape mode.

---

## NAVCH-002: Inconsistent Authentication Behavior and Missing Email Verification

**Severity:** High  
**Priority:** High  
**Module:** Authentication

**Description:**

Authentication behavior is inconsistent when using Google sign-in and email/password login. The application also does not provide a clear duplicate-account warning or send an email verification message during the tested registration flow.

**Preconditions:**
- The user has an account created through Google sign-in.
- The user can access the login and registration screens.

**Steps to Reproduce:**
1. Sign in using a Google account.
2. Return to the login screen.
3. Attempt to log in using the same email address and password.
4. Attempt to register again using the same email address.
5. Check the registered email inbox for a verification message.

**Expected Result:**

The application should handle existing accounts consistently, display an appropriate message when an email is already registered, and send an email verification message when required.

**Actual Result:**
- Email/password login displayed an "Invalid credentials" message.
- The registration flow did not provide a clear duplicate-account warning.
- No email verification message was received.

**Impact:**

Users may become confused about their account status or experience difficulties accessing their accounts.

---

## NAVCH-003: Shopping Cart Items Not Consistently Saved

**Severity:** High  
**Priority:** High  
**Module:** Shopping Cart

**Description:**

Shopping cart items are not consistently retained after refreshing or restarting the application.

**Preconditions:**
- The user can access the shopping cart.
- Products are available to add to the cart.

**Steps to Reproduce:**
1. Add one or more products to the shopping cart.
2. Refresh the application.
3. Check the shopping cart.
4. Add additional products.
5. Refresh the application again.
6. Close the app completely and reopen it.
7. Check the shopping cart again.

**Expected Result:**

All previously added products should remain in the shopping cart after refreshing or restarting the application.

**Actual Result:**
- Some products remained after refreshing.
- Newly added products disappeared after another refresh.
- Cart items were lost after restarting the application.

**Impact:**

Users may lose selected products and need to add them again.

---

## NAVCH-004: Newly Added Address Not Displayed Immediately

**Severity:** Medium  
**Priority:** Medium  
**Module:** Address Management

**Description:**

After saving a new delivery address, the address does not appear immediately in the address list.

**Preconditions:**
- The user is logged in.
- The address management section is accessible.

**Steps to Reproduce:**
1. Open the address management section.
2. Select the option to add a new address.
3. Enter the required address information.
4. Save the address.
5. Check the address list immediately.

**Expected Result:**

The newly saved address should appear in the address list immediately after saving.

**Actual Result:**

The new address does not appear immediately. It becomes visible only after navigating away and reopening the address section.

**Impact:**

Users may think their address was not saved successfully.

---

## NAVCH-005: Application Crashes When Entering Special Characters in Phone Number Field

**Severity:** High  
**Priority:** High  
**Module:** Address Management / Input Validation

**Description:**

The application crashes when special characters are entered into the phone number field while adding a delivery address.

**Preconditions:**
- The user is logged in.
- The checkout section is accessible.

**Steps to Reproduce:**
1. Open the checkout section.
2. Select the option to add a new address.
3. Enter special characters in the phone number field.
4. Attempt to save the address.

**Expected Result:**

The application should validate the phone number and display an appropriate error message without crashing.

**Actual Result:**

The application crashes after special characters are entered and the form is submitted.

**Impact:**

Users may lose their entered information and cannot continue adding an address.

---

## NAVCH-006: Address Form Cannot Be Fully Accessed and Can Close Accidentally

**Severity:** Medium–High  
**Priority:** Medium  
**Module:** Address Management / User Interface

**Description:**

The address form has accessibility problems in landscape mode and can close unexpectedly when the user taps outside the form.

**Preconditions:**
- The user is logged in.
- The add-address form is open.

**Steps to Reproduce:**
1. Open the add-address form.
2. Rotate the device to landscape mode.
3. Try to access all form fields.
4. Enter some address information.
5. Tap outside the form.

**Expected Result:**

The form should allow users to access all fields through scrolling or proper layout adjustment. It should not close unexpectedly without warning or confirmation.

**Actual Result:**
- The form does not support scrolling properly in landscape mode.
- The form closes when the user taps outside it.
- Entered information may be lost.

**Impact:**

Users may be unable to complete the address form or may lose information they already entered.

---

## NAVCH-007: Back Navigation from Payment Skips Address Selection

**Severity:** Medium  
**Priority:** Medium  
**Module:** Checkout Navigation

**Description:**

When the user navigates backward from the payment section, the application skips the address selection step and returns directly to the shopping cart.

**Preconditions:**
- The user is logged in.
- The checkout process has reached the payment section.
- An address has been selected.

**Steps to Reproduce:**
1. Open the shopping cart.
2. Continue to checkout.
3. Select a delivery address.
4. Navigate to the payment section.
5. Select the back navigation option.

**Expected Result:**

The application should return to the previous checkout step, such as address selection.

**Actual Result:**

The application skips the address selection step and returns directly to the shopping cart.

**Impact:**

Users may need to repeat checkout steps and may experience confusion during the purchase process.

---

## NAVCH-008: Payment Options Are Unresponsive

**Severity:** High  
**Priority:** High  
**Module:** Payment

**Description:**

The available payment options do not respond when the user attempts to select them.

**Preconditions:**
- The user is logged in.
- The checkout process has reached the payment section.

**Steps to Reproduce:**
1. Open the shopping cart.
2. Continue to checkout.
3. Navigate to the payment section.
4. Review the available payment options.
5. Attempt to select a payment method.

**Expected Result:**

The user should be able to select an available payment method and continue the checkout process.

**Actual Result:**

The payment options are unresponsive and cannot be selected.

**Impact:**

Users may be unable to complete the checkout process.

---

## NAVCH-009: Profile Input Field Hidden by Keyboard

**Severity:** Medium  
**Priority:** Medium  
**Module:** User Profile / User Interface

**Description:**

When the user selects a profile input field, the keyboard covers the field and makes it difficult to view or edit the information.

**Preconditions:**
- The user is logged in.
- The profile section is accessible.

**Steps to Reproduce:**
1. Open the profile section.
2. Select an editable input field.
3. Allow the keyboard to appear.
4. Check the visibility of the selected field.

**Expected Result:**

The application should adjust its layout when the keyboard appears so that the selected input field remains visible.

**Actual Result:**

The keyboard covers the profile input field.

**Impact:**

Users may have difficulty entering or updating their profile information.

---

## NAVCH-010: Profile Updates Not Retained After App Restart

**Severity:** High  
**Priority:** High  
**Module:** User Profile / Data Persistence

**Description:**

Updated profile information is not reliably retained. After restarting the application, the previous profile information appears instead of the updated information.

**Preconditions:**
- The user is logged in.
- The profile section is accessible.

**Steps to Reproduce:**
1. Open the profile section.
2. Update the user's profile information.
3. Save the changes.
4. Close the application completely.
5. Reopen the application.
6. Open the profile section.
7. Check the displayed information.

**Expected Result:**

The updated profile information should remain saved and displayed after restarting the application.

**Actual Result:**

The previous profile information appears after restarting the application instead of the updated information.

**Impact:**

Users may lose profile changes and may need to update their information again.

---

## 11. Improvement Suggestion

### NAVCH-SUG-001: Add an Option to Delete Saved Addresses

**Type:** Improvement Suggestion  
**Priority:** Low–Medium  
**Module:** Address Management

**Description:**

The address management section does not provide an option to delete previously saved addresses.

**Expected Improvement:**

Users should be able to remove addresses they no longer need. A confirmation message should appear before deleting an address.

**Benefit:**

This would give users better control over their saved delivery information and improve the overall user experience.