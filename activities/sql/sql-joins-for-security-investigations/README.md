# SQL JOINs for Security Investigations

## Overview

A hands-on SQL activity completed as part of the Google Cybersecurity Certificate. This exercise involved combining employee, machine, and login attempt records to support a simulated security investigation.

## Objective

Use SQL JOIN operations to retrieve related information from multiple database tables and identify relationships between employees, assigned machines, and login activity.

## Tables Examined

- `employees` – Employee IDs, usernames, departments, office locations, and device IDs.
- `machines` – Device IDs, operating systems, email clients, and OS patch dates.
- `log_in_attempts` – Login dates, times, countries, IP addresses, and login success status.

## SQL Concepts

- `INNER JOIN`
- `LEFT JOIN`
- `RIGHT JOIN`
- `ON` clause and matching columns

## Investigation Tasks

1. Match employees with their assigned machines.
2. Identify machines without assigned employees.
3. Identify employees without assigned machines.
4. Retrieve login attempts associated with employee records.

## Skills Demonstrated

- SQL table joins
- Relational database querying
- Identifying unmatched records
- Connecting employee and machine information
- Analyzing login activity

## Evidence and Query Results

The following screenshots demonstrate the SQL JOIN operations performed during the investigation.

### 1. INNER JOIN – Employees and Machines

Combines employee records with their assigned machine information using the matching device ID.

### 2. LEFT JOIN – Machines and Employees

Displays all machine records, including machines without an assigned employee.

### 3. RIGHT JOIN – Machines and Employees

Displays all employee records, including employees without an assigned machine.

### 4. INNER JOIN – Employees and Login Attempts

Combines employee information with their associated login activity using matching usernames.

## Disclaimer

This activity was completed in a simulated training environment as part of the Google Cybersecurity Certificate. It does not represent an actual organizational security investigation.
