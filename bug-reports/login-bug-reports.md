# Trendyol Login – Bug Reports

Application: Trendyol Web  
Feature: Login  
Test Type: Manual Testing  
Bug Tracking Style: Jira (Manual)
---


## Bug-01

**Title:** Error message persists after entering a valid email on login page

**Status:** Open

**Environment:**
- Browser: Google Chrome 143.0.7499.194
- OS: macOS

**Precondition:**
- User is on the Trendyol login page

**Linked Test Case:**
- TC-04: Login attempt with invalid email

**Steps to Reproduce:**
1. Enter an invalid email address (e.g. "test@gmail")
2. Click on the "Devam Et" button
3. Enter a valid email address (e.g. "validuser@gmail.com")
4. Click on the "Devam Et" button

**Actual Result:**
- Error message remains displayed after entering a valid email, preventing the user from continuing

**Expected Result:**
- User should be able to continue after entering a valid email without receiving an error message

**Test Data:**
- Invalid email address: "test@gmail"
- Valid email address: "validuser@gmail.com"

**Severity:** Medium  
**Priority:** Medium  

**Note:**
- This bug report is created for learning and portfolio purposes.
- The issue is based on realistic test scenarios and expected application behavior.



## Bug-02 

**Title:** Login page doesn't redirect user to the sign-up page after entering an email that is not associated with any existing user account

**Status:** Open

**Environment:**
- Browser: Google Chrome 143.0.7499.194
- OS: macOS

**Precondition:**
- User is on the Trendyol login page

**Linked Test Case:**
- TC-05: Login attempt with an email that is not associated with any user account

**Steps to Reproduce:**
1. Enter an email address that is not associated with any user account (e.g. "test@gmail.com")
2. Click on the "Devam Et" button

**Actual Result:**
- User remains on the login page and is not redirected to any sign-up or registration flow

**Expected Result:**
- User should be redirected to the sign-up page to create a new account
- The previously entered email address should be automatically filled in the email field of the sign-up form


**Test Data:**
- An unregistered email address: "test@gmail.com"

**Severity:** Medium  
**Priority:** High  

**Note:**
- This bug report is created for learning and portfolio purposes.
- The issue is based on realistic test scenarios and expected application behavior.



## Bug-03 

**Title:** Password reset email is not sent after entering a registered email

**Status:** Open

**Environment:**
- Browser: Google Chrome 143.0.7499.194
- OS: macOS

**Precondition:**
- User is on the Trendyol login page

**Linked Test Case:**
- TC-07: Password reset request via "Şifrenizi mi unuttunuz?" option
  
**Steps to Reproduce:**
1. Enter an email address that is associated with user account (e.g. "testing@gmail.com")
2. Click on the "Devam Et" button
3. Click on the ''Şifrenizi mi unuttunuz?'' button
4. Click on the ''Şifremi Yenile'' button

**Actual Result:**
- User does not receive a password reset email despite seeing a confirmation message on the UI

**Expected Result:**
- User should receive an email to reset the password

**Test Data:**
- A registered email address: "testing@gmail.com"

**Severity:** Medium  
**Priority:** Medium  

**Note:**
- This bug report is created for learning and portfolio purposes.
- The issue is based on realistic test scenarios and expected application behavior.



## Bug-04 

**Title:** User is not directed back to login page after canceling login via Google (404 Error)

**Status:** Open

**Environment:**
- Browser: Google Chrome 143.0.7499.194
- OS: macOS

**Precondition:**
- User is on the Trendyol login page

**Linked Test Case:**
- TC-06: Successful login with Google

**Steps to Reproduce:**
1. Click on the ''Google ile devam et'' button
2. Click on the browser back button (top-left corner)

**Actual Result:**
- User is redirected to a 404 Page Not Found screen
  
**Expected Result:**
- User should be redirected back to the login page without encountering any error page
  

**Severity:** Low  
**Priority:** Low  

**Note:**
- This bug report is created for learning and portfolio purposes.
- The issue is based on realistic test scenarios and expected application behavior.
