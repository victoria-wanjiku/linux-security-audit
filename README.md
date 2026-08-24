# Linux Security Audit

## Overview

A hands-on Linux security audit conducted in an Ubuntu virtual machine to identify, investigate, remediate, and verify common Linux security issues.

The project focuses on practical Linux security administration, access control, process monitoring, and authentication log analysis using Linux command-line tools.

## Objectives

- Audit Linux file and directory permissions
- Implement and test user and group-based access controls
- Monitor and investigate running processes
- Analyze authentication and security logs
- Identify security weaknesses
- Apply appropriate security controls
- Verify that security controls are working as intended
- Document findings and supporting evidence

## Environment

- **Operating System:** Ubuntu Linux
- **Virtualization:** VirtualBox
- **Shell:** Bash
- **Tools:** Linux command-line utilities
- **Test Environment:** Controlled Ubuntu virtual machine

## Security Areas

| # | Security Area | Status |
|---|---|---|
| 1 | File Permissions & Access Control | Completed |
| 2 | Process Monitoring | Completed |
| 3 | Authentication Log Analysis | In Progress |

## Project Structure

```text
linux-security-audit/
│
├── README.md
│
├── evidence/
│   ├── 01-directory-and-files.png
│   ├── 02-file-content.png
│   ├── 03-groups-and-permissions.png
│   ├── 04-access-testing.png
│   └── 05-process-monitoring.png
│
└── findings/
    ├── 01-file-permissions.md
    └── 02-process-monitoring.md
```

## Security Findings

### 1. File Permissions & Access Control

**Status:** Completed

Investigated Linux file and directory permissions and implemented department-based access controls for protected company resources.

The investigation included:

- Creating a controlled company directory structure
- Creating departmental files
- Creating Linux users and groups
- Assigning users to departmental groups
- Changing group ownership
- Applying restrictive file permissions
- Testing authorized and unauthorized access
- Verifying that the implemented controls worked as intended

**Skills demonstrated:**

- Linux file permissions
- `chmod`
- File ownership
- Group ownership
- `chgrp`
- User management
- Group management
- Group-based access control
- Permission verification
- Security remediation

**Detailed finding:** [01-file-permissions.md](findings/01-file-permissions.md)

---

### 2. Process Monitoring

**Status:** Completed

Investigated a controlled Linux process to understand process identification, ownership, parent-child relationships, and process-management permissions.

The investigation included:

- Creating a controlled background process
- Identifying the process ID (PID)
- Identifying the parent process ID (PPID)
- Determining process ownership
- Examining process ancestry using `pstree`
- Testing process termination permissions
- Terminating the process using appropriate privileges

The investigation demonstrated the following process relationship:

```text
bash
└── sudo
    └── sudo
        └── sleep
```

The `sleep` process was identified as:

```text
PID: 41991
PPID: 41990
User: alice
Command: sleep 500
```

**Skills demonstrated:**

- Process monitoring
- PID and PPID identification
- Parent-child process relationships
- Process ownership
- Process investigation
- `ps`
- `pstree`
- Process termination
- Linux privilege management

**Detailed finding:** [02-process-monitoring.md](findings/02-process-monitoring.md)

---

### 3. Authentication Log Analysis

**Status:** In Progress

Authentication and security logs are being analyzed to identify successful and failed authentication attempts and other potentially suspicious activity.

The investigation will include reviewing relevant Linux authentication logs, identifying failed authentication attempts, and examining patterns that may indicate unauthorized access attempts.

**Planned skills:**

- Linux log analysis
- Authentication monitoring
- Failed login investigation
- Security event identification
- Log filtering and searching

---

## Skills Demonstrated

### Linux Security

- File and directory permissions
- User and group management
- Access control
- Process monitoring
- Process management
- Authentication monitoring
- Log analysis
- Linux privilege management

### Security Investigation

- Identifying security weaknesses
- Testing access controls
- Investigating processes
- Analyzing security events
- Applying security remediation
- Verifying security controls
- Documenting investigation results

### Technical Skills

- Linux command line
- Bash
- VirtualBox
- System administration
- Technical documentation

## Evidence

Supporting screenshots and evidence are maintained in the `evidence/` directory.

Each evidence file corresponds to a specific stage of the security investigation.

Detailed investigation steps, commands, findings, remediation actions, and verification results are documented in the `findings/` directory.

## Methodology

Each security area follows a structured investigation process:

1. **Identify** — Determine the potential security issue or security requirement.
2. **Investigate** — Use Linux commands and system information to understand the environment and issue.
3. **Test** — Demonstrate the behavior or security weakness in the controlled environment.
4. **Remediate** — Apply an appropriate security control or configuration change.
5. **Verify** — Test again to confirm that the control works as intended.
6. **Document** — Record commands, results, evidence, remediation, and conclusions.

## Project Status

| Component | Status |
|---|---|
| File Permissions & Access Control | Completed |
| Process Monitoring | Completed |
| Authentication Log Analysis | In Progress |
| Documentation | Ongoing |
| Evidence Collection | Ongoing |

## Disclaimer

This project was conducted in a controlled Ubuntu virtual machine for educational and portfolio purposes.

No unauthorized systems or third-party environments were targeted during this project.
