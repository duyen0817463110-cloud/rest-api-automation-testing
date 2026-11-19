# REST API Automation Testing Framework

## 1. Project Overview
This project involves developing a REST API automation testing framework for a recruitment management system using Java, REST Assured, TestNG, and Maven.

The framework automates API validation for user authentication and work creation functionalities.

## 2. Testing Scope

**API Login**
- Send authentication requests using account credentials.
- Validate HTTP response status codes.
- Verify response messages.
- Validate authentication token generation.
- Verify returned user information.

**API Create Work**
- Send POST requests to create work information.
- Validate HTTP 201 Created responses.
- Verify generated work IDs.
- Validate returned work details, including work name, experience, and education.

## 3. Tools & Technologies
- Java
- REST Assured
- TestNG
- Maven
- JSON
- Properties Files

## 4. Framework Structure

text
assignment-3/
├── configuration/
│   └── configs.properties.example
├── src/
│   ├── main/
│   │   └── java/
│   │       └── com/api/auto/utils/
│   │           └── PropertiesFileUtils.java
│   └── test/
│       └── java/
│           ├── testng.xml
│           └── com/api/auto/testcase/
│               ├── TC_API_Login.java
│               └── TC_API_CreateWork.java
└── pom.xml


## 5. Test Implementation

**TC_API_Login**
- Validate HTTP 200 OK.
- Verify successful login messages.
- Validate authentication token.
- Verify returned user account and user type.

**TC_API_CreateWork**
- Validate HTTP 201 Created.
- Verify generated work ID.
- Compare returned work name with submitted data.
- Validate experience and education information.

## 6. Test Execution
The project uses TestNG annotations to organize test execution and assertions to validate API responses.

Test execution reports are generated in TestNG report formats to support result analysis.

The supplied execution records include successful validations for the Login and Create Work test suites.

## 7. Key Learning Outcomes
- Gained practical experience in REST API automation testing.
- Learned to construct HTTP requests and validate JSON responses.
- Practiced using REST Assured and TestNG assertions.
- Improved understanding of authentication tokens and configuration management.
- Gained experience in organizing automation projects using Maven.

## 8. Security & Configuration
- API base URL and test credentials must be configured locally.
- Sensitive credentials and authentication tokens must not be committed to the repository.
- Use environment variables or local configuration files excluded through `.gitignore`.
- The original API environment may need to be configured before executing the tests.

## 9. Project Notes
This is an individual academic project developed to practice REST API automation testing using Java.
