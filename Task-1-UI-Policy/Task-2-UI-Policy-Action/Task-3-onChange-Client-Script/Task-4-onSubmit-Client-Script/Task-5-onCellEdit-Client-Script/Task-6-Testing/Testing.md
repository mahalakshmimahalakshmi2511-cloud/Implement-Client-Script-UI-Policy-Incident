# Task 6 – Testing

## Test 1 – Mandatory Enforcement

1. Open Incident → Create New.
2. Set Impact = High.
3. Leave Assigned To empty.
4. Click Submit.

### Expected Result
The Incident should not be saved and an error message should be displayed.

---

## Test 2 – Successful Save

1. Set Impact = High.
2. Fill the Assigned To field.
3. Click Submit.

### Expected Result
The Incident should save successfully.

---

## Test 3 – Reverse Condition

1. Open an Incident with Impact = High.
2. Change Impact from High to Medium.

### Expected Result
- Assigned To is no longer mandatory.
- Urgency becomes editable.
- Incident can be submitted successfully.

---

## Test 4 – List Edit Blocking

1. Open Incident → All.
2. Try to edit State directly from the list.
3. Change the State value.

### Expected Result
An alert is displayed and the State remains unchanged.

---

## Test 5 – Form-Based Update

1. Open the same Incident.
2. Change State from the Incident form.
3. Click Update.

### Expected Result
The State should be updated successfully through the form.

---

## Conclusion

The project demonstrates the use of UI Policies and Client Scripts in ServiceNow Incident Management. These configurations provide dynamic field control, automatic updates, save validation, and protection against unwanted list-based changes.
