# API Test Automation with Postman and GitHub Actions

## Overview

This project demonstrates how to execute Postman collections using **Newman** along with the **QA environment**. It also includes automated test execution through **GitHub Actions** for continuous integration, ensuring your API tests are run on every push or pull request.

## Authors

- Chaitali SDET with 10 years of experience in Automation Testing for UI-API-Mobile 
- [GitHub](https://github.com/cchaudhari295)
  
## Features

Tested api on following paramaters-:
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

For continuous integration, GitHub Actions is configured to automatically run tests on each push and pull request to the main branch.

