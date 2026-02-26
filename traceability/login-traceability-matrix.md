# Trendyol Login – Requirement Traceability Matrix (RTM)

**Application:** Trendyol Web  
**Feature:** Login  
**Test Type:** Manual Testing  

---

## 1️⃣ Requirements

### REQ-01 – Successful Login
The system shall allow a registered user to log in using a valid email and correct password and redirect the user to the home page.

### REQ-02 – Invalid Password Handling
The system shall display an error message when a registered user enters an incorrect password and shall not grant access.

### REQ-03 – Empty Email Prevention
The system shall prevent the user from proceeding when the email field is left empty.

### REQ-04 – Invalid Email Format Validation
The system shall display a validation message when the entered email address format is invalid.

### REQ-05 – Unregistered Email Handling
The system shall redirect the user to the sign-up page when an unregistered email is entered and pre-fill the email field.

### REQ-06 – Google Login
The system shall allow users to log in via Google authentication if the Google account is linked to a user account.

### REQ-07 – Password Reset Flow
The system shall allow users to request a password reset email via the “Şifrenizi mi unuttunuz?” option and display a confirmation message.

### REQ-08 – Empty Email UI Feedback
The system shall visually highlight the email input field and display a validation message when the email field is left empty.

---

## 2️⃣ Requirement Traceability Table

| Requirement ID | Test Case ID | Linked Bug | Coverage Status |
|---------------|-------------|------------|------------------|
| REQ-01 | TC-01 | — | Covered |
| REQ-02 | TC-02 | — | Covered |
| REQ-03 | TC-03 | — | Covered |
| REQ-04 | TC-04 | Bug-01 | Covered |
| REQ-05 | TC-05 | Bug-02 | Covered |
| REQ-06 | TC-06 | Bug-04 | Covered |
| REQ-07 | TC-07 | Bug-03 | Covered |
| REQ-08 | TC-08 | — | Covered |

---

## 3️⃣ Coverage Summary

- **Total Requirements:** 8  
- **Total Test Cases:** 8  
- **Linked Defects:** 4  
- **Requirement Coverage:** 100%  
- **Status:** All requirements are covered by at least one test case.
