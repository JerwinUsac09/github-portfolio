
# Linux File Permissions and Access Control

## Overview
A hands-on Linux permissions activity completed as part of the Google Cybersecurity Certificate training.

## Objective
Examine existing file and directory permissions within the `/home/analyst/projects` directory and modify them to match the organization's authorization requirements.

## Tools and Commands
- Linux terminal
- `ls -la` – Inspect file and directory permissions, including hidden files.
- `chmod` – Modify file and directory permissions.

## Tasks Performed

### 1. Inspect Existing Permissions
Used `ls -la` to display detailed information about files, directories, ownership, and permissions.

### 2. Modify File Permissions
Used:
`chmod o-w project_k.txt`

Removed write permission for other users. The initial listing already showed that other users did not have write access, so this command reinforced the intended permission state.

### 3. Modify Hidden File Permissions
Used:
`chmod u-w,g-w,g+r .project_x.txt`

- Removed write permission from the owner.
- Removed write permission from the group.
- Added read permission to the group.

### 4. Restrict Directory Permissions
Used:
`chmod g-x drafts`

Removed execute permission from the group, restricting directory traversal to the authorized owner, `researcher2`, under the existing ownership and permissions shown in the lab.

## Security Concepts Demonstrated
- Linux file permissions
- User, group, and other access rights
- Access control and authorization
- Hidden file permissions
- Directory access restrictions
- Principle of least privilege

## Skills Demonstrated
- Inspecting Linux permissions
- Modifying access rights with chmod
- Interpreting permission strings
- Applying access restrictions
- Reviewing permission changes

## Supporting Documentation
See the `reports` folder for the original file permissions report completed during training.

## Disclaimer
This activity was completed in a simulated training environment as part of the Google Cybersecurity Certificate.
