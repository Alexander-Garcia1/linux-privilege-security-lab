# Linux Privilege Escalation and Set-UID Security Lab

## Project Overview

This project was completed as part of COMP 452: Introduction to Computer Vulnerabilities at Loyola University Chicago during Fall 2026.

The objective was to investigate Linux operating system security, environment variables, privileged application behavior, and vulnerabilities associated with improper privilege management.

Through hands-on exercises in a controlled laboratory environment, I examined how system configuration, process privileges, and inherited resources can affect application security.

## Technical Skills Demonstrated

- Linux System Security
- Linux Command-Line Operations
- Set-UID Permissions and Privileged Processes
- Environment Variable Management
- Process Environment Inheritance
- PATH Security and Command Execution Risks
- Privilege Escalation Analysis
- C Program Compilation with GCC
- File Descriptor Security
- Vulnerability Analysis and Technical Documentation

## Laboratory Investigations and Findings

### 1. Linux Environment Variable Management

**Objective:** Investigate how Linux environment variables are created, modified, inspected, and removed.

**Work Performed:**
- Created and managed environment variables using Linux command-line utilities.
- Verified configuration changes through terminal output.
- Examined how environment variables influence process execution.

**Finding:** Environment variables affect application behavior and require careful management in security-sensitive environments.

### 2. Parent and Child Process Environments

**Objective:** Examine how environment variables are inherited during process creation.

**Work Performed:**
- Investigated the relationship between parent and child process environments.
- Compared environment information using Linux utilities.
- Documented observations regarding process environment inheritance.

**Finding:** Child processes can inherit environment information from their parent processes, making environment configuration relevant to application security.

### 3. Set-UID Application Security

**Objective:** Investigate how Linux handles environment variables during privileged program execution.

**Work Performed:**
- Examined environment variable behavior in Set-UID applications.
- Compared the availability of ordinary and security-sensitive environment variables.
- Observed how privileged execution affected application environments.

**Finding:** Linux restricts certain security-sensitive environment variables during privileged execution to help reduce risks associated with untrusted environment configuration.

### 4. PATH Manipulation and Privileged Application Behavior

**Objective:** Examine security risks associated with privileged applications that rely on user-controlled execution environments.

**Work Performed:**
- Investigated command resolution and PATH configuration in an authorized Linux laboratory.
- Demonstrated how environment manipulation could affect command execution within a privileged application.
- Compared process privilege behavior across different shell configurations.

**Finding:** Improper handling of user-controlled environment information can allow privileged applications to execute unintended commands and create security risks.

### 5. File Descriptor Inheritance and Privilege Management

**Objective:** Examine how file access and inherited resources behave when a process changes its privileges.

**Work Performed:**
- Investigated protected file access in a controlled Linux laboratory.
- Examined the behavior of previously opened file descriptors after a change in process privileges.
- Documented how inherited resources can retain access capabilities.

**Finding:** Dropping elevated privileges does not automatically revoke access to resources opened while privileged.

## Key Security Lessons

This project demonstrated several important Linux security principles:

- Privileged applications should not blindly trust user-controlled environment variables.
- Process environments and inherited configuration can influence application behavior.
- Set-UID applications require careful handling of permissions and execution environments.
- Improper command resolution can introduce vulnerabilities.
- Inherited file descriptors can preserve access to protected resources after privileges change.
- Secure system design requires careful management of privileges, resources, and external input.

## Tools and Technologies

**Operating System:** Linux (SEED Ubuntu Laboratory Environment)

**Programming and Scripting:** C, Bash Shell Commands

**Development Tools:** GCC

**Linux Utilities:** export, printenv, env, unset, diff, chmod

**Security Concepts:** Set-UID, Privilege Escalation, Process Environment Inheritance, PATH Security, File Descriptors, Access Controls

## Professional Relevance

This project strengthened my practical understanding of Linux system security and vulnerability analysis.

The techniques and concepts investigated are relevant to:

- Cybersecurity Analysis
- Linux System Administration
- Vulnerability Assessment
- Security Engineering
- Information Security
- Privileged Access Management

## Academic Information

**University:** Loyola University Chicago

**Degree:** Master of Science in Cybersecurity

**Course:** COMP 452 - Introduction to Computer Vulnerabilities

**Semester:** Fall 2026

## Documentation and Academic Integrity

This repository provides a sanitized technical summary of work performed in an authorized academic laboratory environment.

Detailed exploitation procedures, complete assignment solutions, and original laboratory screenshots are intentionally excluded from the public documentation.

The project is presented for educational and professional portfolio purposes.
