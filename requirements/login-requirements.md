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



### User Story-03: Login attempt with empty email field

As a user  
I want to get a validation message indicating that I should enter an email address when I try to log in without entering an email address  
So that I can enter my email address and continue the login flow

#### Acceptance Criteria (BDD)

Scenario: Login attempt with empty email field
Given the user is on the login page
When the user leaves the email input field empty  
And clicks the "Devam et" button   
Then the user should see an validation message indicating that an email address must be entered



### User Story-04: Login attempt with invalid email

As a user  
I want to see a validation message when I try to log in with an invalid email address  
So that I can correct my email address and continue the login process

#### Acceptance Criteria (BDD)

Scenario: Login attempt with invalid email format  
Given the user is on the login page  
When the user enters an invalid email address  
And clicks the "Devam Et" button  
Then the user should see a validation message indicating that the email address format is invalid



### User Story-05: Login attempt with an email that is not associated with any user account

As a user  
I want to be redirected to the sign-up page when I enter an email that is not associated with any user account
So that I can create a new account

#### Acceptance Criteria (BDD)

Scenario: Login attempt with an email that is not associated with any user account
Given the user is on the login page
When the user enters an unregistered email
And clicks on the "Devam Et" button 
Then the user should be redirected to sign-up page
And the entered email address should be pre-filled in the sign-up form



### User Story-06: Successful login with Google

As a user  
I want to log in using my Google account that is linked to my Trendyol account  
So that I can access my account without entering my email and password manually

#### Acceptance Criteria (BDD)

Scenario: Successful login with Google
Given the user is on the login page  
And the user has a Google account linked to a Trendyol account  
When the user clicks on the "Google ile devam et" button  
And selects the linked Google account  
And completes Google authentication successfully  
Then the user should be logged in successfully  
And the user should be redirected to the home page



### User Story-07: Password reset request via "Şifrenizi mi unuttunuz?" option

As a user  
I want to click on the "Şifrenizi mi unuttunuz?" option and click on the "Şifremi yenile" button after seeing that the email address is pre-filled 
So that I receive a password reset email to reset my password and access my account

#### Acceptance Criteria (BDD)

Scenario: Successful password reset flow via "Şifrenizi mi unuttunuz?" option  
Given the user is on the login page  
And has an existing user account  
When the user enters a registered email address  
And clicks on the "Devam et" button  
And clicks on the "Şifrenizi mi unuttunuz?" button  
And clicks on the "Şifremi yenile'' button after verifying that the email input field is pre-filled  
Then the user should see a confirmation message indicating that the password reset email has been sent  
And the user should receive a password reset email  



### User Story-08: Login attempt with empty email field

As a user   
I want to be notified when I attempt to log in without entering an email address  
So that I can enter my email address and continue with the login flow

#### Acceptance Criteria (BDD)

Scenario: Login attempt with empty email field
Given the user is on the login page
When the user leaves the email input field empty
And clicks on the "Devam et" button
Then the email input field should be highlighted with a red border
And a validation message should be displayed
