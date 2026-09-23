# 5. Project Development Phase

## Project Title
Streamlining IT Procurement: Automating Standard Laptop Orders with Flow Designer

## Project Overview
This phase focuses on developing and implementing the automated IT procurement workflow using ServiceNow Flow Designer.

The workflow is designed to automate the creation of a Catalog Task when a Standard Laptop request is approved. The task is automatically assigned to the Hardware assignment group for laptop configuration.

## Development Activities

### 1. Create Flow
A Flow Designer flow named **Standard Laptop Task** was created.

- Application: Global
- Run As: System User
- Trigger: Service Catalog
- Action: Create Catalog Task

### 2. Configure Catalog Task
The Catalog Task was configured with the following values:

- Short Description: Laptop need to Configured
- Description: Laptop need to Configured
- Assignment Group: Hardware
- Approval: Approved

### 3. Assign Flow to Standard Laptop
The created flow was assigned to the **Standard Laptop** service catalog item through the Process Engine configuration.

### 4. Place Standard Laptop Request
A Standard Laptop request was placed through the Service Catalog.

The request was then opened and approved through the Approvers section.

### 5. Verify Catalog Task
After approval, the Requested Item was opened and the **Catalog Tasks** section was checked.

The generated task displayed the configured:
- Short Description
- Assignment Group
- Task status

## Expected Outcome
The Standard Laptop procurement process is automated so that an approved request automatically generates a configuration task and assigns it to the Hardware team.

## Result
The development phase successfully implements the automated workflow for Standard Laptop requests using ServiceNow Flow Designer.
