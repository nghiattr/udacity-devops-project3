
# Overview

Udacity final project Ensuring Quality Releases.

![pipeline](pipeline-diagram.png)

# Project Structure 

- **azure-pipelines.yaml**: azure pipelines yaml
- **automatedtesting**: suites of different tests
  - **jmeter**: load test (JMeterPlan.jmx), CSV inputs, and TestReports (endurance-report, stress-report)
  - **postman**: functional tests postman collections and environments
  - **selenium**: ui tests (uitests.py)
- **fakerestapi**: api files to deplopy webapp
- **screenshoots**: all screen shots requests
- **terraform**: terraform scripts

---

# Screenshoots Log

## Environment Creation & Deployment

- Terraform to apply Infrastructure as Code (IaC)
  - screenshot of the log output of Terraform when executed by the CI/CD pipeline
   ![capture-terraform-output](screenshots/1.png)
   ![capture-terraform-state](screenshots/2.png)

- Automated testing tasks
  - screenshot of the successful execution of the pipeline build results page (/_build/results?buildId={id}&view=results)
    ![capture-pipeline](screenshots/3.png)

## Webapp Depdeloyment

- Deploy Azure Webapp http://was-eqr.azurewebsites.net/
  ![](screenshots/4.png)

## Automated Testing

- Load test suite 
  - screenshot of the log output of JMeter when executed by the CI/CD pipeline
    ![capture-load-test](screenshots/5.png)
    ![capture-load-test](screenshots/6.png)
  
- Functional test suites 
  - screenshot of the execution of the test suite by the CI/CD pipeline
   ![capture-functional-test](screenshots/7.png)

- API-integration tests
  - screenshot of the Run Summary page (which contains 4 graphs)
    ![capture-summary-page-part1](screenshots/8.png)
    ![capture-summary-page-part1](screenshots/9.png)
  - screenshot of the Test Results page (which contains the test case titles from each test) 
    ![capture-test-result-page-part2](screenshots/10.png)
  - screenshot of the output of the Publish Test Results step
    ![capture-publish-tests-output-part3](screenshots/11.png)

## Monitoring & Observability

- Configure Azure Monitor
  - screenshots of the email received when the alert is triggered
    ![capture-emails-part1](screenshots/12.png)
  - screenshots of the graphs of the resource that the alert was triggered
    
    ![capture-alerts-part3a](screenshots/14.png)
  - screenshots of the alert rule
    ![capture-webapp-part2](screenshots/13.png)


- Azure Log Analytics
  - screenshots of log analytics queries and result sets which will show specific output of the Azure resource
    ![capture-log-analytics](screenshots/15.png)