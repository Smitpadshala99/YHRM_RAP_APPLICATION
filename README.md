# RESTful Application Programming for Human Resource Management

## Overview
This repository is designed to help you learn SAP RAP (Restful Application Programming) concepts through a comprehensive Human Resource Management (HRM) project. The project covers various aspects of SAP RAP, including:

- **Managed and Unmanaged Scenarios**: Understand the differences between managed and unmanaged implementations within SAP RAP.
- **Core Data Services (CDS)**: Learn how to define and utilize CDS views to represent and manipulate data in your application.
- **Metadata Extensions**: Explore how metadata extensions can be used to enhance your CDS views with additional information such as UI annotations.
- **Behavior Definitions**: Define the behavior of your entities, including CRUD operations, validations, and actions.
- **Service Binding**: Discover how to expose your CDS views and behavior definitions as OData services.
- **RAP Concepts**: Gain a deeper understanding of various RAP concepts that are crucial for building robust and scalable applications.

This HRM application includes functionalities to manage employees, departments, jobs, addresses, and timesheets. It provides practical examples of both managed and unmanaged scenarios, helping you to grasp the core principles and best practices of SAP RAP.

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
![Database Schema](https://github.com/Smitpadshala99/YHRM_RAP_APPLICATION/blob/main/Img/Database%20Diagram.png)

### Application Flow

#### Managed Example (Only Employee)
![Managed Application Flow](https://github.com/Smitpadshala99/YHRM_RAP_APPLICATION/blob/main/Img/Managed%20Employee%20App%20Diagram.png)

#### Unmanaged Example (Employee & Timesheet)
![Unmanaged Application Flow](https://github.com/Smitpadshala99/YHRM_RAP_APPLICATION/blob/main/Img/UnManaged%20Employee%20Timesheet%20App%20Diagram.png)

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

## Additional Information

For more detailed information, please read the PDF document [Restful Application Programming.pdf](https://github.com/Smitpadshala99/YHRM_RAP_APPLICATION/blob/main/Restful%20Application%20Programming.pdf).
