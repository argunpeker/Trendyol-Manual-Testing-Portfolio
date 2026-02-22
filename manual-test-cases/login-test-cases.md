# Trendyol Login - Manual Test Cases

Application: Trendyol Web  
Feature: Login  
Test Type: Manual Testing
---

## TC-01: Successful login with valid credentials

**Precondition:**
- User is on the Trendyol login page

**Test Steps:**
1. Enter a valid email address
2. Enter a valid password
3. Click the "Giriş Yap" button

**Expected Result:**
- User should be logged in successfully
- User should be redirected to the homepage

**Test Data:**
- Valid registered email
- Valid password


**Status:** Not Executed



## TC-02: Login attempt with invalid password

**Precondition:**
- User is on the Trendyol login page

**Test Steps:**
1. Enter a valid email address
2. Enter an invalid password
3. Click the "Giriş Yap" button

**Expected Result:**
- User should not be logged in
- An error message should be displayed

**Test Data:**
- Valid registered email
- Invalid password

- **Status:** Not Executed



## TC-03: Login attempt with empty email field

**Precondition:**
- User is on the Trendyol login page

**Test Steps:**
1. Leave the email field empty
2. Click the "Devam Et" button

**Expected Result:**
- User should get ''E-posta adresinizi girin.'' message

**Status:** Not Executed



## TC-04: Login attempt with invalid email

**Precondition:**
- User is on the Trendyol login page

**Test Steps:**
1. Enter an invalid email address (e.g. "test@gmail")
2. Click the "Devam Et" button

**Expected Result:**
- User should get ''Geçersiz e-posta adresi'' message

**Test Data:**
- Invalid email format: "test@gmail"

**Status:** Not Executed



## TC-05: Login attempt with an email that is not associated with any user account

**Precondition:**
- User is on the Trendyol login page

**Test Steps:**
1. Enter an email address that is not associated with any user account (e.g. testingacc@gmail.com)
2. Click the "Devam Et" button

**Expected Result:**
- User should be redirected to the sign-up page
- The previously entered email address should be automatically filled in the email field of the sign-up form
  
**Test Data:**
- Valid email format that is not associated with any user account: "testingacc@gmail.com"

**Status:** Not Executed

**Note:**
- Behavior observed during manual testing on Trendyol web application



## TC-06: Successful login with Google

**Precondition:**
- User is on the Trendyol login page
- User has a Google account that is associated with a Trendyol user account

**Test Steps:**
1. Click on the ''Google ile devam et'' button
2. Choose a Google account that is associated with a Trendyol user account
3. Complete Google authentication if required


**Expected Result:**
- User should be logged in successfully
- User should be directed to the home page

**Test Data:**
- a Google account that is associated with a Trendyol user account

**Status:** Not Executed

**Note:**
- Behavior observed during manual testing on Trendyol web application
  


## TC-07: Successful password reset flow via "Şifrenizi mi unuttunuz?" option

**Precondition:**
- User is on the Trendyol login page
- User has an existing Trendyol user account

**Test Steps:**
1. Enter a valid email address
2. Click on the "Devam Et" button
3. Click on the "Şifrenizi mi unuttunuz?" link
4. Verify that the email address field is pre-filled or enter the valid email address if required
5. Click on the "Şifremi yenile" button

**Expected Result:**
- User should see a confirmation message indicating that the password reset email has been sent
- User should receive a password reset email

**Test Data:**
- Valid email address associated with a Trendyol user account

**Status:** Not Executed

**Note:**
- Behavior observed during manual testing on Trendyol web application



## TC-08: Login attempt with empty email field

**Precondition:**
- User is on the Trendyol login page


**Test Steps:**
1. Leave the email input field empty
2. Click on the "Devam Et" button


**Expected Result:**
- Email input field should be highlighted with a red border 
- User should see a validation message: "E-posta adresinizi girin."


**Status:** Not Executed

**Note:**
- Behavior observed during manual testing on Trendyol web application











