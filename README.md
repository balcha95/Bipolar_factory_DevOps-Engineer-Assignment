# Web Application CI/CD Pipeline

## Overview

This repository contains the setup and configuration for a basic CI/CD pipeline for a web application. The pipeline is designed to automatically build, test, and deploy the application on each push to the main branch.

## Contents

1. [Version Control Setup](#version-control-setup)
2. [CI/CD Pipeline Implementation](#ci-cd-pipeline-implementation)
3. [Monitoring and Logging](#monitoring-and-logging)
4. [Documentation and Reporting](#documentation-and-reporting)

## Version Control Setup

- A GitHub repository has been created for the simple web application.
- The web application is a basic Java based web app displaying 'Hello World!'

## CI/CD Pipeline Implementation

### CI/CD Platforms Used

- The CI/CD pipeline is implemented using [Jenkins](https://jenkins.io/). Include the installation File in repo.

### Pipeline Configuration

- The pipeline is configured to automatically trigger a build on every push to the main branch.
- It follows the steps outlined below:
  1. **Build the Application:** The pipeline builds the web application.
  2. **Run Automated Tests:** Automated tests are executed, including a main test to check for the presence of 'Hello World!'
  3. **Deploy the Application:** The application can be deployed to a test server Tommcat platform.

### Usage

1. Fork/Clone the repository.
2. Configure your Jenkins instance with the necessary plugins and settings.
3. Set up a Jenkins job with the pipeline script provided in the repository.

## Monitoring and Logging

- Basic monitoring and logging have been set up for the deployed application using grafana & promathus.
- Alerts and notifications are configured to notify on any failures or issues during deployment.

## Documentation and Reporting

- [**CI/CD Setup Documentation:**](/docs/CI_CD_SETUP.md) Detailed documentation on the steps and configurations done for the entire CI/CD process.
- [**Observations Report:**](/docs/OBSERVATIONS_REPORT.md) A brief report highlighting challenges faced and potential improvements.
