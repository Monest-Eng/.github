## What does this PR do:
* Example: Added email validation to user registration
* Example: Fixed the login button not working on Safari
* Example: Added POST /api/users endpoint
* 

## How to test:
* Example: Try to register with invalid email "test@" - should show error message
* Example: Open Safari and check if login button works after entering credentials
* Example: POST /api/users with body:
```json
{
    "name": "John",
    "email": "john@test.com",
    "role": "admin"
}
```
* 

## Business Rules and Tests:
1. Rule: [Email must contain @ and valid domain]
   - Test: [test_invalid_email_registration in UserRegistrationTest]

2. Rule: [Login button should work across all supported browsers]
   - Test: [test_login_cross_browser in LoginComponentTest]