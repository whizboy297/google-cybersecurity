# Module 1: Operating Systems

**Course:** Google Cybersecurity Professional Certificate — Course 4  
**Course Title:** Tools of the Trade: Linux and SQL  
**Module:** 1 — Operating Systems  
**Date Studied:** October 14, 2026  
**Status:** Completed

---

## 1. Overview

This module introduced operating systems, their main functions, and how they connect computer hardware, applications, and users.

It also explored graphical user interfaces (GUIs) and command-line interfaces (CLIs), including when each interface is more effective.

Understanding operating systems is important in cybersecurity because security professionals need to understand how computers run applications, allocate resources, manage files, and control access.

## 2. What Is an Operating System?

An operating system (OS) is system software that manages computer hardware and resources and provides an environment for applications to run.

It acts as an interface between computer hardware and the user.

### Examples of Operating Systems

- Windows
- macOS
- Linux
- Android
- iOS

Computers, smartphones, and tablets use operating systems to support their functions.

## 3. Main Functions of an Operating System

Operating systems manage the resources required for computers and applications to operate efficiently.

### Process Management

The operating system manages running programs and processes.

### Memory Management

The operating system manages the allocation of memory to applications and processes.

### File Management

The operating system supports the organisation, storage, retrieval, and management of files and directories.

### Device Management

The operating system coordinates communication between software and hardware devices.

### Resource Allocation

Computer resources are limited. The operating system manages these resources and allocates them where they are needed.

Examples of resources include:

- CPU processing time
- Random Access Memory (RAM)
- Storage capacity
- Hardware devices

## 4. Applications, Operating Systems, and Hardware

Applications, operating systems, and hardware work together to perform computing tasks.

| Component | Function | Example |
|---|---|---|
| Hardware | Provides the physical resources needed for computing | CPU, RAM, SSD |
| Operating system | Manages hardware resources and provides services to applications | Windows, Linux, macOS |
| Application | Performs a specific task for the user | Calculator, web browser |
| User | Interacts with applications to perform tasks | A person using a computer |

### Example: Performing a Calculation

When a user performs a calculation:

1. The user enters numbers into a calculator application.
2. The application sends a request to the operating system.
3. The operating system coordinates the resources needed to perform the task.
4. The hardware performs the required computation.
5. The result is returned through the operating system to the application.
6. The application displays the result to the user.

This illustrates how applications, operating systems, and hardware work together.

## 5. The Operating System Boot Process

The boot process describes how a computer starts its operating system.

The sequence covered in this module is:

1. The computer is switched on.
2. The BIOS or UEFI firmware begins the startup process.
3. The BIOS or UEFI loads the bootloader.
4. The bootloader starts the operating system.

### Key Terms

**BIOS:** Basic Input/Output System firmware used to initialise hardware and begin the boot process.

**UEFI:** Unified Extensible Firmware Interface, a modern firmware interface used to initialise the system and begin booting.

**Bootloader:** A program that starts the operating system.

### Remember the Sequence

**BIOS/UEFI → Bootloader → Operating System**

Understanding the boot process provides a foundation for learning about system integrity and boot-level security.

## 6. Graphical User Interface (GUI)

A Graphical User Interface allows users to interact with a computer through visual elements.

Common GUI components include:

- Icons
- Windows
- Menus
- Buttons
- Taskbars
- Start menus
- Desktop shortcuts

### Example

Opening Finder on macOS and clicking folders to browse files is an example of using a GUI.

### Advantages of a GUI

- Often easier for beginners to learn.
- Provides visual feedback.
- Makes navigating files and applications intuitive.
- Useful for demonstrations involving users with different levels of technical expertise.

### Cybersecurity Applications

GUIs are useful when working with graphical security tools, reviewing dashboards, and examining security alerts.

## 7. Command-Line Interface (CLI)

A Command-Line Interface allows users to interact with a computer by entering text-based instructions.

Instead of selecting icons or menus, users type commands to perform tasks.

### Examples of Linux Commands

```bash
pwd
```

Displays the current working directory.

```bash
ls
```

Lists files and directories in the current directory.

```bash
whoami
```

Displays the current username.

These commands are examples introduced for familiarisation; further Linux lessons will explore command-line use in more detail.

### Advantages of a CLI

- Efficient for repetitive tasks.
- Supports automation through scripts.
- Can process multiple files using commands.
- Allows users to review command history.
- Useful for system administration and investigation.

### Cybersecurity Applications

Security professionals may use command-line tools to:

- Search files and logs.
- Investigate system activity.
- Examine user accounts and permissions.
- Perform repetitive administrative tasks.
- Support incident investigations.

## 8. GUI vs. CLI

| Feature | GUI | CLI |
|---|---|---|
| Interaction | Visual elements | Text-based commands |
| Learning curve | Often easier for beginners | Requires familiarity with commands |
| Repetitive tasks | May require repeated manual actions | Can automate many repetitive tasks |
| Automation | Possible through GUI automation | Commonly supported through scripts |
| Typical cybersecurity use | Reviewing dashboards and graphical tools | Searching logs and investigating systems |

Neither interface is inherently more secure than the other. Their effectiveness depends on the task, configuration, permissions, and how they are used.

### Scenario 1: Training Employees to Change Passwords

A GUI is generally more effective because employees with different levels of technical expertise can follow visual instructions more easily.

### Scenario 2: Renaming Hundreds of Log Files

A CLI is generally more efficient because commands or scripts can rename multiple files in one operation.

### Scenario 3: Installing Multiple Applications and Reviewing Commands

A CLI can maintain command history, helping a user review the commands they entered.

However, command history is not necessarily a complete audit log and does not guarantee that every command succeeded.

## 9. Command History and Security Investigations

A command-line history can help users review previously entered commands.

In a security investigation, available command history may provide clues about actions performed on a system.

Security analysts should not rely on command history alone because it may be incomplete, deleted, or unavailable.

Other evidence, such as authentication records, system logs, and process information, may be needed to establish what happened.

## 10. Key Cybersecurity Takeaways

This module established several foundations for cybersecurity work:

- Operating systems manage hardware and computer resources.
- Applications rely on operating system services to perform tasks.
- Resource allocation helps a computer use its limited capacity effectively.
- The bootloader starts the operating system.
- GUIs provide visual interaction with computers.
- CLIs provide text-based interaction and can support automation.
- Command history can assist with reviewing activity but is not a complete audit record.
- Understanding operating systems is foundational to investigating computer activity.

## 11. Assessment Results

| Assessment | Score | Result |
|---|---:|---|
| Operating Systems — Introduction | 100% | Passed |
| Operating Systems — Functions and Boot Process | 100% | Passed |
| GUI vs. CLI Practical Scenarios | 100% | Passed |
| GUI and CLI Knowledge Check | 100% | Passed |
| Operating Systems Module Assessment | 88.88% | Passed |

**Module assessment pass mark:** 80%

**Overall result:** Passed.

## 12. Key Terms

| Term | Definition |
|---|---|
| Operating System (OS) | System software that manages computer resources and provides services to applications |
| Application | Software designed to perform a specific task |
| Hardware | The physical components of a computer |
| CPU | Central Processing Unit; executes instructions |
| RAM | Random Access Memory; temporary working memory used by running programs |
| BIOS | Firmware interface used to initialise hardware and begin the boot process |
| UEFI | Modern firmware interface used to initialise the system and begin booting |
| Bootloader | Program that starts the operating system |
| GUI | Graphical User Interface |
| CLI | Command-Line Interface |
| Resource Allocation | Distribution of limited computer resources among tasks and processes |
| Command History | A record of commands entered into a command-line environment |

## 13. Next Steps

The next stage of Course 4 will develop my understanding of Linux and SQL.

I will continue learning how to use command-line tools and query data, with the goal of applying these skills to cybersecurity investigations.

---

**Learning pathway:** Google Cybersecurity Professional Certificate  
**Course:** Tools of the Trade: Linux and SQL  
**Module 1:** Operating Systems
