# SQL Filtering for Security Investigations

## Overview
A SQL activity completed as part of the Google Cybersecurity Certificate. This exercise involved examining employee records and login attempt data to investigate potential security issues.

## Objective
Use SQL queries and filtering techniques to retrieve relevant records from the `employees` and `log_in_attempts` tables.

## Tables Examined
- `employees` – Employee information, including usernames, departments, office locations, and device IDs.
- `log_in_attempts` – Login activity, including timestamps, countries, IP addresses, and login success status.

## SQL Concepts and Commands
- `SELECT` and `FROM` – Retrieve information from database tables.
- `WHERE` – Filter records based on specified conditions.
- `AND` and `OR` – Combine multiple filtering conditions.
- `NOT` – Exclude records matching a condition.
- `LIKE` and `%` – Search for text patterns.

## Investigation Tasks
- Identify unsuccessful login attempts occurring after 6 PM.
- Retrieve login attempts from specific dates.
- Identify login attempts originating outside Mexico.
- Filter Marketing employees working in East offices.
- Retrieve employees from Finance and Sales departments.
- Identify employees who are not part of the IT department.

## Skills Demonstrated
- SQL data retrieval and filtering
- Database querying
- Logical operators and conditional filtering
- Pattern matching
- Basic security investigation using database records

## Supporting Documentation
See the `reports` folder for supporting documentation from the training activity.

## Disclaimer
This activity was completed in a simulated training environment as part of the Google Cybersecurity Certificate. It does not represent an actual organizational security investigation.
