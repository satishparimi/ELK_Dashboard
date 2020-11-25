# Welcome to the ELK_Dashboard for Test Automation Setup wiki!

Follow the below steps to setup ELK Dashboard

# Need below server configurations 
  * Elasticsearch - is a search engine based on the Lucene library
  * Kibana - is an open source data visualization dashboard

# Objective: capture the test logs in elasticsearch and will design dashboards in Kibana 

## Problem Statement
### Test Results vs. Environments
   * Current Approach: Emailable reports are generating for all scheduled runs
      * Quite challenging job to see consolidated results at one place for all environments

### Reports vs Time Scale (Over the period of time)
   * Daily Based Reports
   * Weekly Based Reports
   * Monthly Based Reports
   * Quarterly Based …Reports

### Log Panels vs Reports at once place
   * We can easily analyze the Failed and skipped tests at one place wit detailed logs along with test results

### To solve above challenges we started implementing this well suitable test automation dashboard by using following ingredients

# Ingredients used
### TestNG Listeners for event based handling
 * onTestSuccess() - Capturing passed tests information
 * onTestFailure() - Capturing failed tests information
 * onTestSkipped() - Capturing skipped tests information

