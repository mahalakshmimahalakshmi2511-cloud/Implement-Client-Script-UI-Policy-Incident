# Task 4 – onSubmit Client Script

## Client Script Name
Prevent save if Assigned To missing

## Table
Incident

## Type
onSubmit

## Active
Yes

## Script

function onSubmit() {
    if (g_form.getValue('impact') == '1' &&
        g_form.getValue('assigned_to') == '') {

        g_form.showErrorBox(
            'assigned_to',
            'Assigned To is mandatory for High impact incidents.'
        );
        return false;
    }
    return true;
}

## Purpose
Prevents saving a High Impact Incident when the Assigned To field is empty.

## Expected Result
- Impact = High
- Assigned To = Empty
- Submit → Save is blocked
- Error message is displayed

When Assigned To is filled, the Incident can be saved.
