# Task 5 – onCellEdit Client Script

## Client Script Name
Prevent state change via list edit

## Table
Incident

## Type
onCellEdit

## Field
State

## Active
Yes

## Script

function onCellEdit(sysIDs, table, oldValues, newValue, callback) {

    alert('State cannot be updated using list editing. Please open the Incident.');

    callback(false);
}

## Purpose
Prevents users from changing the Incident State directly through list editing.

## Expected Result
When the State field is edited directly from the Incident list:

- An alert message is displayed.
- The State value remains unchanged.
- User must open the Incident form to update the State.
