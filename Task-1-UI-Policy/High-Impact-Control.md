# Task 1 – UI Policy

## UI Policy Name
High Impact Control

## Table
Incident

## Condition
Impact is 1 - High

## Active
Yes

## Reverse if False
Yes

## Purpose
This UI Policy is triggered when the Incident Impact is set to High.

It is used to control Incident fields dynamically based on the Impact value.

## Configuration
- Navigate to System UI → UI Policies
- Create a new UI Policy
- Select Incident as the table
- Set Impact to High
- Enable Active
- Enable Reverse if False

## Expected Result
When Impact is set to High, the configured UI Policy Actions are applied automatically.
