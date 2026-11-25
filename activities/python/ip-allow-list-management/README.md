# Python – Automating IP Allow List Management

## Overview
A Python programming activity completed as part of the Google Cybersecurity Certificate. This exercise involved automating the removal of IP addresses from an organization's allow list to maintain appropriate access to restricted resources.

## Scenario
A healthcare organization maintains an IP allow list containing addresses permitted to access a restricted network containing sensitive patient information.

A separate remove list identifies IP addresses that should no longer have access. The task was to develop a Python algorithm that checks the allow list against the remove list and removes matching addresses.

## Objective
Automate the process of updating an IP allow list using Python file handling, conditional statements, loops, and list operations.

## Tools and Programming Concepts

- **Python** – Programming language used to develop the algorithm.
- `open()` – Opens the allow list file.
- `with` – Manages file access and resource handling.
- `.read()` – Reads the file contents.
- `.split()` – Converts the contents into a list.
- `for` loop – Iterates through the remove list.
- `if` statement – Checks whether an IP address exists in the allow list.
- `.remove()` – Removes matching IP addresses.
- `.join()` – Converts the updated list into a string.
- `.write()` – Writes the revised contents back to the file.

## Algorithm Workflow

1. Open `allow_list.txt` in read mode.
2. Read the file contents into a string.
3. Convert the string into a list of IP addresses using `.split()`.
4. Iterate through the IP addresses in the remove list.
5. Check whether each address exists in the allow list.
6. Remove matching addresses.
7. Convert the updated list back into a string using `.join()`.
8. Open the original file in write mode and save the revised list.

## Security Concepts Demonstrated

- IP-based access control
- Allow list management
- Access restriction
- Basic security automation
- File handling and data manipulation

## Skills Demonstrated

- Python programming fundamentals
- Automating repetitive administrative tasks
- Working with files and lists
- Implementing conditional logic and loops
- Applying programming concepts to a cybersecurity scenario

## Supporting Documentation

See the `reports` folder for the completed activity report and code explanations.

## Disclaimer
This activity was completed as part of the Google Cybersecurity Certificate in a simulated training environment. It demonstrates an allow list management algorithm and does not represent an actual production network access-control implementation.
