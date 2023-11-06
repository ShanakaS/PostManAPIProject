# API Test Suite Documentation

## Overview

This API test suite is designed to test the functionality and reliability of the Couple of Test APIs. It includes a collection of test cases that cover various aspects of the API, ensuring it functions as 
expected and meets the required specifications.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Test Structure](#test-structure)
- [Running Tests](#running-tests)
- [Environment Configuration](#environment-configuration)
- [Variables](#variables)
- [Test Reports](#test-reports)
- [Contributing](#contributing)
- [License](#license)

## Prerequisites

Before running the test suite, you will need the following prerequisites:

- Postman: Make sure you have Postman installed on your machine.
- node install to newman report generate


## Getting Started

To get started with the test suite, follow these steps:

1. Clone this repository to your local machine.

2. Open Postman and import the collection file provided in this repository.

3. Import the environment file for your specific environment configuration.

4. Configure environment variables as needed 

5. Configure Global Variables

## Test Structure

The test suite is organized into collections, folders, and individual requests, each designed to test specific API endpoints or scenarios. Here's an overview of the structure:

- API Collection
  - Get Requests
    - List of All Objects
    - List of Objects By IDS
    - Single Object

  - Post Requests 
    - Add object
  
  - Put Requests
    - Update Object

  - Patch Requests
    - Partially Update object

  - Delete Request
    - Delete Object

## Running Tests

To run the tests, follow these steps:

1. Open Postman.

2. Select the imported collection from the left sidebar.

3. Click on the "Run" button.

4. Choose the environment for the test run.

5. Click "Start Run."

6. Monitor the test execution and view the results.

## Environment Configuration

The test suite uses environment variables to configure the API endpoints and authentication settings. Make sure to set up the environment variables based on your testing environment. The environment file is provided in the repository.

## Variables

This test suite uses Global variables.

## Test Reports

After running the tests, you can generate test reports using Newman. To generate an HTML report, use the following command:

```shell
newman run collection.json -e environment.json --reporters cli,html --reporter-html-export report.html

or

use newman run newman run "D:\PostManCollection\APIs Collection.postman_collection.json" -r html

