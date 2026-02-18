# newman-tests-demonstration

This repository contains a collection of automated API tests for various free public services. By integrating Postman with GitHub, all collections are automatically synced and ready for execution via **Newman**, Postman’s command-line runner.

## 📂 Project Structure

* **/postman/collections**: Contains the JSON exported Postman collections.
* **/postman/environments**: (Optional) Contains environment variables used for different API stages.

## Public APIs used: 

* **Nameday API**: https://nameday.abalin.net/
* **Nameday API documentation**: https://nameday.abalin.net/docs/api#/

## 🚀 Getting Started

### Prerequisites

Ensure you have [Node.js](https://nodejs.org/) installed, then install Newman globally:

```bash
npm install -g newman

```

### Running Tests

To run a specific test suite, navigate to the root directory and execute the following command:

```bash
newman run postman/collections/your-collection-name.json

```

## 📊 Features

* **Automated Validation:** Checks for status codes, response times, and data integrity.
* **CI/CD Ready:** This structure is designed to be easily plugged into GitHub Actions or Jenkins.
* **Version Controlled:** All changes made in the Postman UI are automatically synced to this repo.