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
- User should be redirected to the sign-up page to create a new account

**Test Data:**
- Valid email format that is not associated with any user account: "testingacc@gmail.com"

**Status:** Not Executed

**Note:**
- Behavior observed during manual testing on Trendyol web application







