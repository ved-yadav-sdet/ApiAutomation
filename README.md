# API Automation Framework

A Java-based API automation testing framework built using **Rest Assured, TestNG and Maven**, with Allure integration for test reporting.

This project demonstrates API automation framework organization, test execution and response validation for authentication-related API scenarios.

## Tech Stack

| Technology | Purpose |
|---|---|
| Java 17 | Programming language |
| Rest Assured 5.3.1 | REST API automation |
| TestNG 7.0.0 | Test execution and assertions |
| Maven | Dependency and build management |
| Allure | Test reporting |
| Jackson | JSON processing |
| JavaFaker | Test data generation |
| Jsoup | HTML parsing |

## Project Structure

```text
ApiAutomation/
│
├── .github/
│   └── workflows/       # GitHub Actions workflows
│
├── Input/
│   ├── Dashboard/
│   └── Auth/
│
├── src/                 # Automation source code
│
├── runner.xml           # TestNG suite configuration
├── pom.xml              # Maven dependencies
└── README.md
```

## Framework Highlights

- REST API automation using Rest Assured.
- Test execution and suite configuration using TestNG.
- Maven-based dependency management.
- Allure reporting integration.
- Test data and input organization.
- Java 17 compatibility.
- TestNG suite configuration with a staging environment parameter.

## Prerequisites

Before running the project, make sure you have:

- Java JDK 17 or later
- Apache Maven
- Git
- An IDE such as IntelliJ IDEA or Eclipse

Verify your installations:

```bash
java -version
mvn -version
```

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/ved-yadav-sdet/ApiAutomation.git
```

### 2. Navigate to the project

```bash
cd ApiAutomation
```

### 3. Install dependencies and build

```bash
mvn clean install
```

### 4. Execute tests

```bash
mvn test
```

The repository also includes a TestNG suite configuration in `runner.xml`, with the environment parameter set to `staging`.

## Test Reporting

The framework includes Allure dependencies for test reporting.

After test execution, check the generated test results and configure the Allure CLI to generate and view the report.

```bash
allure serve allure-results
```

## Configuration

Configure environment-specific values, API base URLs and credentials according to your test environment.

**Security recommendations:**
- Never commit API credentials, access tokens or passwords.
- Use environment variables or GitHub Actions Secrets for sensitive configuration.
- Keep environment-specific configuration separate from test logic.
- Avoid exposing sensitive request or response data in reports.

## Future Improvements

- Add environment-specific configuration management.
- Improve reusable request and response specifications.
- Add JSON schema validation.
- Introduce data-driven API testing.
- Expand negative and boundary-value scenarios.
- Improve parallel test execution.
- Enhance CI/CD execution and reporting.

## Author

**Ved Prakash Yadav**

Senior SDET | QA Automation Engineer

GitHub: https://github.com/ved-yadav-sdet

LinkedIn: https://www.linkedin.com/in/ved-yadav-sdet/

---

*This project is maintained as part of my hands-on learning and practical work in API automation and quality engineering.*
