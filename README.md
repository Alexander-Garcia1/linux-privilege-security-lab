# Linux Privilege Escalation and Set-UID Security Lab

## Project Overview

This project was completed as part of COMP 452: Introduction to Computer Vulnerabilities at Loyola University Chicago during Fall 2026.

The objective was to investigate Linux environment variables, process privileges, Set-UID programs, and security vulnerabilities associated with improper privilege management.

Through controlled laboratory exercises, I examined how environment variables and inherited resources can influence the behavior of privileged applications.

## Technical Skills Demonstrated

- Linux System Security
- Linux Command Line
- Set-UID Permissions
- Privilege Escalation Analysis
- Environment Variable Manipulation
- Process Environment Inheritance
- PATH Security
- C Programming and GCC
- File Descriptor Security
- Vulnerability Analysis and Documentation

## Laboratory Investigations

### 1. Linux Environment Variable Management

Created, inspected, and removed Linux environment variables using commands including `export`, `printenv`, `env`, and `unset`.

Verified changes through terminal output and documented variable behavior.

### 2. Parent and Child Process Environments

Investigated environment variable inheritance between parent and child processes.

Used Linux utilities to compare process environments and observed how environment variables were inherited through process creation.

### 3. Set-UID Environment Variable Security

Examined how privileged Set-UID applications handle environment variables.

Observed that ordinary variables could remain available while security-sensitive variables such as `LD_LIBRARY_PATH` were restricted during privileged execution.

### 4. PATH Manipulation and Privilege Escalation

Investigated the security implications of user-controlled PATH variables in a controlled Linux laboratory.

Demonstrated how a privileged application could execute an unintended command through PATH manipulation.

Examined the relationship between shell behavior, real user IDs, effective user IDs, and privileged execution.

### 5. File Descriptor Inheritance and Privilege Management

Investigated how file descriptors behave when applications drop elevated privileges.

Demonstrated that access to an already-open protected file could persist after a process changed its user privileges.

Documented the security implications of inherited file descriptors and improper resource handling.

## Key Security Findings

The laboratory demonstrated several important Linux security principles:

- Privileged applications should not blindly trust user-controlled environment variables.
- Set-UID programs require careful management of execution environments.
- Improper PATH handling can create opportunities for unauthorized command execution.
- Dropping privileges does not automatically revoke access to previously opened resources.
- Secure privilege management requires careful handling of both permissions and inherited resources.

## Tools and Technologies

**Operating System:** Linux (SEED Ubuntu laboratory environment)

**Languages:** C, Bash shell commands

**Tools:** GCC, Linux Terminal, Environment Variable Utilities, Process Inspection Tools

**Security Concepts:** Set-UID, Process Privileges, PATH Manipulation, Environment Inheritance, File Descriptors

## Academic Information

**University:** Loyola University Chicago  
**Degree:** Master of Science in Cybersecurity  
**Course:** COMP 452 — Introduction to Computer Vulnerabilities  
**Semester:** Fall 2026

## Disclaimer

This repository documents security research conducted in an authorized academic laboratory environment. The experiments were performed for educational purposes to understand Linux vulnerabilities and defensive security principles.
