# RESTful Application Programming for Human Resource Management

## Overview
This project is a Human Resource Management Application built using RESTful principles. It includes examples of both managed and unmanaged scenarios for handling employees and timesheets.

## Features
- **Employee Management**: Create, read, update, and delete employee records.
- **Department Management**: Manage departmental data and hierarchy.
- **Timesheet Management**: Track and manage employee working hours and leaves.
- **Job Management**: Maintain job titles and types.
- **Address Management**: Store and update employee addresses.
- **Draft Handling**: Support for draft operations for managed scenarios.

## Application Structure
The application utilizes several key tables to manage data efficiently:

### Department Table (`YHRM_DEPARTMENT`)
- Stores department information.
- Fields: `department_id`, `department_name`, `hod`, `address_id`.

### Employee Table (`YHRM_EMPLOYEE`)
- Stores employee details.
- Fields: `emp_id`, `first_name`, `last_name`, `email`, `phone_no`, `dob`, `gender`, `salary`, `hire_date`, `active`, `resign_date`, `address_id`, `job_id`, `department_id`, `supervisor_id`.

### Job Table (`YHRM_JOB`)
- Maintains job-related information.
- Fields: `job_id`, `job_title`, `job_type`.

### Address Table (`YHRM_ADDRESS`)
- Stores address details.
- Fields: `address_id`, `street_add1`, `street_add2`, `street_add3`, `pin_code`, `city`, `state`, `country`.

### Timesheet Table (`YHRM_TIMESHEET`)
- Records timesheet entries for employees.
- Fields: `emp_id`, `ydate`, `available`, `workinghours`, `leavetype`, `overtime_hrs`, `approved_by`.

### Draft Tables
These tables support draft functionality, typically used in managed applications:
- `YHRM_DEPART_D` (Draft Department Table)
- `YHRM_EMPLOYEE_D` (Draft Employee Table)

## Application Diagrams

### Database Schema
![Database Schema](path/to/database_schema.png)

### Application Flow
![Application Flow](path/to/application_flow.png)


## Usage

### Employee Management
- **Create Employee**: Use the form to add new employee details.
- **View Employees**: See a list of all employees with their details.
- **Update Employee**: Edit existing employee information.
- **Delete Employee**: Remove an employee from the system.

### Timesheet Management
- **Add Timesheet Entry**: Record working hours and leaves for employees.
- **View Timesheets**: Check the timesheet entries for all employees.
- **Update Timesheet**: Modify timesheet entries.
- **Approve Timesheet**: Approve timesheets for final processing.
