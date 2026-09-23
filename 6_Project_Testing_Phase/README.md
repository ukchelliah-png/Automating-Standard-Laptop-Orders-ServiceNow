# 6. Project Testing Phase

## Project Title
Streamlining IT Procurement: Automating Standard Laptop Orders with Flow Designer

## 6.1 Testing Overview

The testing phase verifies that the Standard Laptop procurement workflow works correctly after implementation in ServiceNow Flow Designer.

The main purpose of testing is to confirm that an approved Standard Laptop request automatically creates the required Catalog Task and assigns it to the Hardware assignment group.

## 6.2 Test Case 1 – Flow Trigger

### Objective
To verify that the Flow Designer flow is triggered correctly for the Standard Laptop service request.

### Test Steps
1. Open ServiceNow.
2. Navigate to the Service Catalog.
3. Open the Hardware category.
4. Select Standard Laptop.
5. Click Order Now.
6. Submit the request.
7. Check the request record.

### Expected Result
The Standard Laptop request should be created successfully and the workflow should be triggered according to the configured flow.

### Status
Passed

## 6.3 Test Case 2 – Approval

### Objective
To verify that the Standard Laptop request can be approved successfully.

### Test Steps
1. Open the created request.
2. Open the Approvers section.
3. Select the approval record.
4. Approve the request.
5. Open the Requested Item.

### Expected Result
The request should show the approved status and the flow should continue to the next stage.

### Status
Passed

## 6.4 Test Case 3 – Catalog Task Creation

### Objective
To verify that a Catalog Task is automatically created after approval.

### Test Steps
1. Open the approved Requested Item.
2. Scroll to the Catalog Tasks section.
3. Open the generated Catalog Task.
4. Check the task details.

### Expected Result
A Catalog Task should be created automatically.

### Status
Passed

## 6.5 Test Case 4 – Short Description

### Objective
To verify the configured short description of the Catalog Task.

### Expected Result
The Catalog Task should display:

**Laptop need to Configured**

### Status
Passed

## 6.6 Test Case 5 – Assignment Group

### Objective
To verify that the Catalog Task is assigned to the correct group.

### Expected Result
The Assignment Group should be:

**Hardware**

### Status
Passed

## 6.7 Test Case 6 – End-to-End Workflow

### Objective
To verify the complete Standard Laptop procurement workflow.

### Test Flow

Standard Laptop Request
→ Approval
→ Requested Item
→ Catalog Task Creation
→ Hardware Assignment

### Expected Result
The complete workflow should execute successfully without manual intervention in the task creation and assignment process.

### Status
Passed

## 6.8 Testing Result

The testing phase confirms that the implemented Standard Laptop procurement workflow performs the configured activities successfully.

The approved request generates the Catalog Task with the required short description and assigns the task to the Hardware group.

## 6.9 Conclusion

The testing phase verifies the functionality of the automated procurement workflow and confirms that the implemented Flow Designer configuration operates as expected for the Standard Laptop request process.
