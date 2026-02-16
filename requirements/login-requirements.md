# Trendyol Login Feature - Requirements

Application: Trendyol Web  
Feature: Login  
Test Type: Manual Testing
---

#### Note
The requirements document was created after writing the login test cases and login bug reports, in order to demonstrate reverse-engineering skills and understanding of system behavior. User stories are related to the corresponding login test case number.



### User Story-01: Login with valid credentials

As a registered user  
I want to log in using a valid email address and password  
So that I can access my account

#### Acceptance Criteria (BDD)

Scenario: Successful login with valid credentials  
Given the user has an existing account  
And the user is on the login page  
When the user enters a registered email address and correct password  
And clicks the "Giriş Yap" button   
Then the user should be logged in successfully  
And redirected to the home page



### User Story-02: Login attempt with invalid password

As a registered user  
I want to get an error message indicating that my email or password is not correct when I log in using a valid email address and an invalid password  
So that I can correct my password and successfully log in

#### Acceptance Criteria (BDD)

Scenario: Login attempt with invalid password
Given the user has an existing account  
And the user is on the login page  
When the user enters a registered email address and an invalid password  
And clicks the "Giriş Yap" button   
Then the user should see an error message indicating that the email or password is incorrect

**Note:** Acceptance Criteria are derived from observing the actual behavior of the Trendyol login page.

