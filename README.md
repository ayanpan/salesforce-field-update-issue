# Saesforce Field Update Issue

## Problem Statement:
Some fields are getting updated in Salesforce even though we are passing their values in Boomi (via the Salesforce SOAP Connector), and there's no error thrown by Salesforce.

## Root Cause:
This issue happens when there's a metadata change in the referenced Salesforce Object.

## Solution:
1. Re-import the Salesforce XML Profile.
2. Redo the required fields' mapping.
3. Re-deploy the Process and re-test.
