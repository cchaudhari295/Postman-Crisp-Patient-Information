# API Test Automation with Postman and GitHub Actions

## Overview

This project demonstrates how to execute Postman collections using **Newman** along with the **QA environment**. It also includes automated test execution through **GitHub Actions** for continuous integration, ensuring your API tests are run on every push request.

## Author

- Chaitali SDET with 10 years of experience in Automation Testing for UI-API-Mobile
- [LinkedIn](https://www.linkedin.com/in/chaitali-chaudhari-a2b850177/)
- [GitHub](https://github.com/cchaudhari295)
- EmailID: chaitali1.chaudhari@gmail.com
  
## Features

Tested API on following paramaters-:
- Response Time
- Status Code
- Schema Validation
  
## Prerequisites

To get started, ensure the following tools are installed:

- [Node.js](https://nodejs.org/)
- [Newman](https://www.npmjs.com/package/newman)
- [Newman-HTML Extra](https://www.npmjs.com/package/newman-reporter-htmlextra)

## Running the Collection Locally

To execute the Postman collection locally using the **QA environment file**, follow these steps:

1. Install Newman and Newman-HTML Extra globally on your system:

   ```bash
   npm install -g newman newman-reporter-htmlextra

2. Run the collection on your terminal using the following command:

   ```bash
   newman run <path_to_collection.json> -e <path_to_QA_environment.json> --reporters cli,htmlextra

Replace the placeholders:
  <path_to_collection.json>: Path to your Postman collection file
  <path_to_QA_environment.json>: Path to your Postman environment file

 This will execute collection with the specified environment and generate a test report in both the CLI and HTML formats.

## Automated Execution with GitHub Actions

For continuous integration, GitHub Actions is configured to automatically run tests on each push request to the main branch.
- To view the report, follow these steps:
1. Go to the Actions tab.
2. Select the link for the latest workflow run.
3. In the Artifacts section, click on Postman Test Report to download the report to your system.
4. Open the downloaded HTML report to review the test results.
