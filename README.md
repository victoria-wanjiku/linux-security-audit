# Linux Security Audit

## Overview

A hands-on Linux security audit conducted in an Ubuntu virtual machine to identify, investigate, remediate, and verify common Linux security issues.

The project focuses on practical Linux security administration, access control, process monitoring, and log analysis using command-line tools.

## Objectives

- Audit Linux file and directory permissions
- Review user and group access controls
- Monitor and investigate running processes
- Analyze authentication and security logs
- Identify security weaknesses
- Apply appropriate security controls
- Verify that security issues have been resolved
- Document findings and supporting evidence

## Environment

- **Operating System:** Ubuntu Linux
- **Virtualization:** VirtualBox
- **Shell:** Bash
- **Tools:** Linux command-line utilities
- **Focus:** Linux security administration and basic security monitoring

## Security Areas

| # | Security Area | Status |
|---|---|---|
| 1 | File Permissions | Completed |
| 2 | User & Group Access Control | Completed |
| 3 | Process Monitoring | Completed |
| 4 | Authentication Log Analysis | In Progress |

# Security Findings

## 1. File Permissions
**Status:** Completed

Investigated Linux file and directory permissions to identify inappropriate access levels. The investigation included reviewing permission settings, testing access, applying appropriate permission changes, and verifying that unauthorized access was restricted.

**Skills demonstrated:**
- Linux file permissions
- `chmod`
- Permission verification
- Access control
- Security remediation

## 1.1. User & Group Access Control
**Status:** Completed

Reviewed Linux users and groups to determine whether users had appropriate access to protected resources. Access was tested between different users, and group-based permissions were used to ensure that authorized users could access resources while unauthorized users were denied.

**Skills demonstrated:**
- Linux user management
- Linux group management
- Group-based access control
- User permission testing
- Access verification

## 3. Process Monitoring
**Status:** Completed

Investigated running processes and examined parent-child process relationships. A test process was created and monitored to identify its process ID (PID) and parent process ID (PPID). The process was then investigated and safely terminated.

**Example:**

## Project Structure

**Skills demonstrated:**
- Process monitoring
- PID and PPID identification
- Parent-child process relationships
- Process investigation
- Process termination

## 4. Authentication Log Analysis
**Status:** In Progress

Authentication and security logs are being analyzed to identify successful and failed authentication attempts and other potentially suspicious activity. The investigation includes reviewing relevant Linux authentication logs and identifying patterns that could indicate unauthorized access attempts.

**Skills demonstrated:**
- Linux log analysis
- Authentication monitoring
- Failed login investigation
- Security event identification

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

### Security Investigation
- Identifying security weaknesses
- Testing access controls
- Investigating processes
- Analyzing security events
- Applying security remediation
- Verifying security controls

### Technical Skills
- Linux command line
- Bash
- VirtualBox
- System administration
- Technical documentation

---

## Evidence

Screenshots and other supporting evidence are maintained in the `evidence/` directory.

Detailed investigation steps, findings, remediation actions, and verification results will be documented in the `findings/` directory.

Important commands used during the investigation will be documented in the `commands/` directory.

---

## Methodology

Each security area follows a basic security assessment process:

1. **Identify** — Determine the potential security issue.
2. **Investigate** — Use Linux commands and system information to understand the issue.
3. **Test** — Verify whether the identified weakness can be demonstrated.
4. **Remediate** — Apply an appropriate security control or configuration change.
5. **Verify** — Test again to confirm that the issue has been resolved.
6. **Document** — Record the finding, commands, results, and supporting evidence.

---

## Disclaimer

This project was conducted in a controlled Ubuntu virtual machine for educational and portfolio purposes. No unauthorized systems or third-party environments were targeted during this project.


