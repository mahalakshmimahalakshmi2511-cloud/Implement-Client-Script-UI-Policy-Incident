# Task 3 – onChange Client Script

## Client Script Name
Auto set urgency for high impact

## Table
Incident

## Type
onChange

## Field
Impact

## Active
Yes

## Script

function onChange(control, oldValue, newValue, isLoading) {
    if (isLoading || newValue == '') {
        return;
    }

    if (newValue == '1') {
        g_form.setValue('urgency', '1');
        g_form.addInfoMessage('Urgency set to High for High impact incident.');
    }
}

## Purpose
Automatically sets the Urgency field to High when the Incident Impact is changed to High.

## Expected Result
When Impact is changed to High, Urgency is automatically set to High.
