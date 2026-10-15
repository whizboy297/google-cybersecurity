# Module 2 — Linux

**Programme:** Google Cybersecurity Professional Certificate  
**Course:** Course 4 — Tools of the Trade: Linux and SQL  
**Module:** Module 2 — Linux  
**Topic:** Linux Operating Systems, Architecture, Distributions, Command-Line Interfaces, and Package Management  
**Status:** ✅ Completed

---

## 1. Module Overview

This module introduced Linux, its architecture, different Linux distributions, and the Linux shell.

I learned how Linux systems are structured, how users interact with the operating system through the command line, and how to manage software packages using the Advanced Package Tool (APT).

I also explored how the operating system interacts with hardware and applications, the difference between graphical and command-line interfaces, and how commands produce input, output, and error messages.

As part of the practical work, I used APT to install, remove, reinstall, and verify software applications in a Debian-based Linux environment.

These skills are important in cybersecurity because security analysts regularly work with operating systems, command-line tools, network analysis applications, and software packages.

### Learning Objectives

By the end of this module, I learned how to:

- Explain what Linux is and why it is important.
- Identify the major components of Linux architecture.
- Distinguish between hardware and software.
- Explain the purpose of the Linux kernel and shell.
- Identify different Linux distributions.
- Understand the differences between graphical and command-line interfaces.
- Explain standard input, standard output, and standard error.
- Use basic Linux commands.
- Understand how APT manages software packages.
- Install, remove, and verify applications using the Linux command line.
- Explain how Linux tools support cybersecurity investigations.

---

## 2. Understanding Linux

Linux is an open-source operating system.

An operating system manages computer resources and provides an environment in which applications can run. It acts as an intermediary between applications, users, and the computer's hardware.

Linux is widely used in servers, cloud infrastructure, embedded systems, and cybersecurity environments.

### What Does Open Source Mean?

Open-source software makes its source code available for people to inspect, modify, and distribute according to its licence.

Because Linux is open source, developers can study its code and build different distributions around the Linux kernel.

### Why Is Linux Important in Cybersecurity?

Linux is important in cybersecurity because it provides access to powerful command-line tools and security applications.

Security professionals use Linux to:

- Investigate suspicious system activity.
- Monitor network traffic.
- Analyse network packets.
- Manage files and permissions.
- Install and manage security tools.
- Automate repetitive tasks.
- Work with servers and cloud environments.
- Conduct authorised penetration testing.
- Perform digital forensics.

Linux is not limited to cybersecurity. It is also used for everyday computing, software development, server administration, and many other purposes.

---

## 3. Understanding Operating Systems

An operating system (OS) is system software that manages a computer's hardware and software resources.

It provides an environment in which applications can execute tasks.

Examples of operating systems include:

- Linux
- Microsoft Windows
- macOS
- Android
- iOS

Operating systems are used on computers, smartphones, tablets, and other computing devices.

### Functions of an Operating System

An operating system performs several important functions:

1. **Resource management:** Allocates system resources such as CPU time and memory.
2. **Process management:** Manages running programs and processes.
3. **Memory management:** Controls how memory is allocated and used.
4. **Hardware interaction:** Coordinates communication between software and hardware.
5. **File management:** Supports the organisation and management of files and directories.
6. **Application support:** Provides services that applications need to operate.
7. **User interaction:** Allows users to interact with the computer through interfaces such as a GUI or CLI.

### Operating Systems and Hardware

The operating system helps applications use hardware resources without requiring every application to control the hardware directly.

For example, when a user performs a calculation in an application:

1. The user enters a number into the application.
2. The application requests the required operation through the operating system.
3. The operating system coordinates access to the resources needed to perform the operation.
4. The result is returned through the operating system to the application.
5. The application displays the result to the user.

This demonstrates how the operating system helps coordinate communication between applications and the computer's resources.

### Resource Allocation

Computers have limited resources, including CPU capacity and memory.

The operating system helps ensure that these resources are allocated to processes that need them.

On Windows, Task Manager is a graphical utility that allows users to monitor running processes and resource usage. It is a tool for viewing and managing system activity, not the operating system itself.

---

## 4. Graphical User Interface (GUI)

A Graphical User Interface (GUI) allows users to interact with a computer through visual elements rather than relying entirely on typed commands.

A GUI makes it possible to perform tasks by clicking icons, selecting menus, and interacting with windows.

### Examples of GUI Components

Common GUI components include:

- Desktop
- Taskbar
- Start menu
- Icons
- Shortcuts
- Windows
- Menus
- Buttons

Hardware components such as a CPU and RAM are not components of a graphical user interface.

### Advantages of a GUI

- It is generally easy for beginners to learn.
- Users can interact with visual elements.
- It reduces the need to memorise commands.
- It makes many everyday tasks straightforward.
- It provides visual feedback when interacting with applications.

### Example

A user can open a folder by clicking its icon in a file manager instead of typing a command.

---

## 5. Command-Line Interface (CLI)

A Command-Line Interface (CLI) allows users to interact with a computer by entering text-based commands.

Instead of clicking icons and menus, users type commands into a terminal or shell.

The CLI is especially useful for system administration, software management, automation, and cybersecurity work.

### Advantages of a CLI

- Commands can perform tasks quickly.
- Repetitive tasks can be automated using scripts.
- It provides direct access to many administrative tools.
- It is useful when managing remote systems.
- It can be more efficient than a GUI for certain technical tasks.
- It is widely used in Linux administration and cybersecurity.

### Example

The following command displays the current working directory:

```bash
pwd
```

The command asks the shell to execute `pwd`, which prints the directory in which the user is currently working.

### GUI vs CLI

| Feature | GUI | CLI |
|---|---|---|
| Interaction | Visual elements | Text-based commands |
| Input | Mouse, keyboard, touch | Primarily typed commands |
| Ease of use | Often easier for beginners | Requires command knowledge |
| Automation | Possible, depending on the tools | Often well suited to scripting |
| Common use | Everyday desktop tasks | Administration, automation, and technical tasks |

Both interfaces are useful. The best choice depends on the task being performed.

### Command History

A command history feature records previously entered commands in the shell environment.

This allows users to review and reuse commands.

Command history can be useful when checking which commands were entered during troubleshooting or administrative work. However, it should not be treated as a complete or tamper-proof audit log.

In cybersecurity, command records may provide useful context when investigating system activity.

---

## 6. Linux Architecture

Linux architecture consists of components that work together to allow users and applications to interact with the computer.

The major components covered in this module include:

1. User
2. Applications
3. Shell
4. Kernel
5. Hardware
6. Filesystem Hierarchy Standard (FHS)

### 6.1 User

The user is the person interacting with the Linux system.

A user can enter commands, run applications, manage files, and perform administrative tasks.

Linux supports multiple user accounts, allowing access and permissions to be managed for different users.

### 6.2 Applications

Applications are programs designed to perform specific tasks.

Examples include:

- Text editors
- Web browsers
- Network analysis tools
- File managers
- Security applications
- Software development tools

Applications use operating system services to access resources such as memory, files, and network interfaces.

### 6.3 Shell

The shell is a command-line interpreter that allows users to interact with the operating system through text-based commands.

It accepts commands, interprets them, and coordinates their execution.

For example:

```bash
echo "Hello, world!"
```

This command displays:

```text
Hello, world!
```

The shell is particularly useful for performing administrative tasks and executing security tools.

### 6.4 Kernel

The kernel is the core component of an operating system.

It manages access to system resources and coordinates interactions between software and hardware.

Its responsibilities include:

- Process management.
- Memory management.
- Hardware interaction.
- Resource allocation.
- Managing access to system services.
- Supporting communication between applications and system resources.

The Linux kernel is the central part of Linux-based operating systems.

### 6.5 Hardware

Hardware refers to the physical components of a computer.

Examples include:

- CPU
- RAM
- Keyboard
- Monitor
- Storage devices
- Network interface cards

#### CPU

The Central Processing Unit (CPU) executes instructions and performs calculations.

#### RAM

Random Access Memory (RAM) provides temporary working memory for running programs and processes.

RAM is volatile memory, meaning its contents are generally lost when power is removed.

#### Network Interface Card

A network interface allows a computer to communicate over a network.

Depending on the device, it may support wired or wireless communication.

### 6.6 Filesystem Hierarchy Standard (FHS)

The Filesystem Hierarchy Standard (FHS) defines a standard structure for organising directories and files on Linux systems.

It helps make file locations more predictable across Linux distributions.

Examples of important Linux directories include:

| Directory | Purpose |
|---|---|
| `/` | The root of the filesystem |
| `/home` | Common location for regular users' home directories |
| `/etc` | System configuration files |
| `/var` | Variable data, including many logs and application data |
| `/tmp` | Temporary files |
| `/usr` | Many user-space programs, libraries, and shared resources |
| `/bin` | Essential command binaries on systems that maintain this directory separately |
| `/sbin` | System administration binaries on systems that maintain this directory separately |

Some modern Linux distributions use symbolic links or merged directory structures, so the exact physical arrangement can vary.

### How the Components Work Together

A simplified view of Linux architecture is:

```text
             User
               |
               v
          Applications
               |
               v
             Shell
               |
               v
             Kernel
               |
               v
            Hardware

     FHS organises filesystem data
```

This diagram is a simplified conceptual representation. Applications can interact with the kernel through operating system interfaces without going through the shell.

**Key takeaway:** The kernel manages system resources, the shell interprets commands, applications perform tasks, hardware executes physical operations, and the FHS defines a standard filesystem organisation.

---

## 7. Understanding the Linux Shell

The shell is an important tool for interacting with Linux through the command line.

It accepts commands, interprets them, and helps execute programs.

A command may produce output, request input, or return an error message.

### Example 1: Display a Message

```bash
echo "Hello, world!"
```

Output:

```text
Hello, world!
```

The `echo` command prints text to standard output.

### Example 2: Display the Current Directory

```bash
pwd
```

The `pwd` command displays the present working directory.

### Example 3: List Files

```bash
ls
```

The `ls` command lists files and directories in the current location.

### Example 4: Display Help Information

```bash
nload -h
```

When Nload is installed, this command displays its help and usage information.

If the command or executable is unavailable, the shell may return an error.

### Shell Errors

When a command cannot be executed successfully, the shell or program may display an error message.

For example, attempting to run a command that is not available may produce a message indicating that the command cannot be found.

Error messages help users understand why a command failed.

---

## 8. Standard Input, Standard Output, and Standard Error

Command-line programs commonly use three standard data streams:

1. Standard input (stdin)
2. Standard output (stdout)
3. Standard error (stderr)

These streams help commands receive information and communicate their results.

### 8.1 Standard Input (stdin)

Standard input is the stream through which a program receives input.

By default, it is commonly connected to the terminal keyboard.

For example, a program may request information from the user through standard input.

### 8.2 Standard Output (stdout)

Standard output is the stream used by a program to return normal results.

For example:

```bash
echo "Linux is useful for cybersecurity"
```

The text is displayed as standard output.

### 8.3 Standard Error (stderr)

Standard error is the stream commonly used for error messages and diagnostic information.

For example, a command that attempts to access a file that does not exist may display an error message.

### Comparison

| Stream | Name | Purpose |
|---|---|---|
| stdin | Standard input | Receives input |
| stdout | Standard output | Returns normal output |
| stderr | Standard error | Returns errors and diagnostic messages |

### Why Are These Streams Important?

Separating normal output from errors makes command-line work more flexible.

For example, a user can redirect normal output to a file while keeping error messages visible in the terminal.

Standard streams are also useful when combining commands in scripts.

**Key takeaway:** Standard input provides information to a program, standard output carries normal results, and standard error carries error messages and diagnostics.

---

## 9. Linux Distributions

A Linux distribution, often called a Linux distro, is a packaged version of a Linux-based operating system.

Distributions combine the Linux kernel with software, utilities, package management tools, and other components to provide a usable operating system.

Different distributions are designed for different purposes.

### Why Are There Different Linux Distributions?

Different users and organisations have different requirements.

Some distributions prioritise ease of use, while others focus on enterprise systems, servers, privacy, or cybersecurity.

### Examples of Linux Distributions

#### Ubuntu

Ubuntu is a widely used Linux distribution based on Debian.

It is known for its accessibility and is commonly used for desktop computing, software development, servers, and cloud environments.

#### Kali Linux

Kali Linux is a Debian-based Linux distribution designed for information security work.

It includes tools that can support:

- Penetration testing.
- Digital forensics.
- Security assessments.
- Network analysis.
- Vulnerability assessment.

Kali Linux is useful for authorised security testing and learning cybersecurity techniques.

#### Parrot

Parrot is a Linux distribution that includes editions and tools focused on security, privacy, and development.

Its security-oriented environment can support penetration testing and digital forensics.

#### Red Hat Enterprise Linux

Red Hat Enterprise Linux is an enterprise-focused Linux distribution used in business and server environments.

It is designed for enterprise computing and supported production environments.

#### CentOS

CentOS is associated with the Red Hat ecosystem.

CentOS Linux was historically a rebuild of Red Hat Enterprise Linux. CentOS Stream is a rolling distribution that tracks ahead of a corresponding Red Hat Enterprise Linux release.

CentOS Stream and the historical CentOS Linux releases should not be treated as identical.

#### SUSE Linux

SUSE Linux distributions are used in desktop, server, and enterprise environments.

SUSE provides Linux solutions for organisations and infrastructure deployments.

### Linux Distributions and Security Tools

Some Linux distributions are designed to provide ready access to security tools.

For example:

- Kali Linux includes many tools used in penetration testing and digital forensics.
- Parrot Security editions include tools for security assessment and privacy-related work.
- Wireshark is a network protocol analyser that can be installed on supported operating systems.

**Important distinction:** Wireshark is an application, not a Linux distribution.

### Comparing Selected Distributions

| Distribution or tool | Category | Common use |
|---|---|---|
| Ubuntu | Linux distribution | Desktop computing, development, and servers |
| Kali Linux | Linux distribution | Penetration testing and digital forensics |
| Parrot | Linux distribution | Security, privacy, and development |
| Red Hat Enterprise Linux | Linux distribution | Enterprise computing |
| CentOS | Linux distribution family | Server and enterprise-related environments |
| SUSE Linux | Linux distribution family | Desktop, server, and enterprise computing |
| Wireshark | Application | Network protocol analysis |

### Key Takeaway

Linux distributions share the Linux kernel lineage but differ in their included software, package management, support models, and intended use cases.

---

## 10. Managing Software with APT

APT stands for **Advanced Package Tool**.

It is a package management tool used by Debian-based Linux distributions, including Ubuntu and Kali Linux.

APT allows users to install, remove, and manage software packages from the command line.

### Common APT Commands

| Command | Purpose |
|---|---|
| `apt` | Displays basic APT usage information |
| `sudo apt install package_name` | Installs a package |
| `sudo apt remove package_name` | Removes a package |
| `apt list --installed` | Lists installed packages |

Replace `package_name` with the name of the package you want to manage.

### Understanding `sudo`

The `sudo` command allows an authorised user to execute a command with elevated privileges.

Installing and removing software commonly requires administrative permissions.

For example:

```bash
sudo apt install tcpdump
```

This requests permission to install the Tcpdump package using APT.

### Installing Software

The general syntax is:

```bash
sudo apt install package_name
```

APT resolves the package and its dependencies and attempts to install the software.

### Removing Software

The general syntax is:

```bash
sudo apt remove package_name
```

This instructs APT to remove the specified package.

The `remove` operation generally leaves system-wide configuration files behind, unlike a full purge operation.

### Listing Installed Packages

```bash
apt list --installed
```

This displays the installed packages known to APT.

It is useful when checking whether a required application is installed.

---

## 11. Hands-On Lab: Manage Software Applications in Linux Using APT

### Lab Overview

In this lab, I practised using APT to install, uninstall, reinstall, and verify software applications in a Debian-based Linux environment.

The lab scenario involved working as a security analyst who needed to manage software tools and verify their installation status.

The applications used were:

- **Nload:** A command-line tool for monitoring network traffic and bandwidth usage.
- **Tcpdump:** A command-line tool for capturing network packets.

**Lab status:** ✅ Completed  
**Result:** All lab tasks passed.

### Learning Objectives

By completing this lab, I learned how to:

- Explore APT from the command line.
- Install software packages.
- Verify that a package is available.
- Remove software packages.
- Identify installed applications.
- Reinstall software.
- Use `sudo` when administrative privileges are required.

### Task 1: Explore APT

I began by running:

```bash
apt
```

This displayed basic usage information for APT.

APT was already available in the Debian-based lab environment.

**What I learned:** APT provides a command-line method for managing software packages.

### Task 2: Install and Remove Nload

#### Step 1: Install Nload

I ran:

```bash
sudo apt install nload
```

When prompted to continue, I pressed Enter to accept the default Yes option.

**Command breakdown:**

- `sudo`: Executes the command with elevated privileges.
- `apt`: Invokes the package management tool.
- `install`: Requests installation of a package.
- `nload`: Specifies the package name.

#### Step 2: Verify Nload

I ran:

```bash
nload -h
```

The command displayed Nload's version and usage information, confirming that the executable was available.

#### Step 3: Remove Nload

I ran:

```bash
sudo apt remove nload
```

This instructed APT to uninstall Nload.

#### Step 4: Verify the Removal

I ran:

```bash
nload -h
```

After removal, the terminal returned an error indicating that `/usr/bin/nload` could not be found.

This confirmed that Nload was no longer available at its previous executable path.

**What I learned:** I can install an application, verify its availability, remove it, and check whether its executable is still accessible.

### Task 3: Install Tcpdump

I installed Tcpdump using:

```bash
sudo apt install tcpdump
```

Tcpdump is a command-line utility used to capture network packets.

**Cybersecurity relevance:** Security analysts can use packet captures to investigate network communications, troubleshoot network problems, and examine potentially suspicious traffic.

Installing Tcpdump does not itself capture traffic. Packet capture requires running the tool with appropriate options and permissions.

### Task 4: List Installed Applications

I ran:

```bash
apt list --installed
```

This displayed the packages installed in the lab environment.

I checked the results and confirmed that:

- Tcpdump was installed.
- Nload was absent after I removed it.

**What I learned:** The installed package list can be used to verify software availability.

### Task 5: Reinstall Nload

I reinstalled Nload by running:

```bash
sudo apt install nload
```

I then checked the installed packages again:

```bash
apt list --installed
```

The final verification confirmed that both Nload and Tcpdump were installed.

### Final Lab Results

| Application | Final status | Purpose |
|---|---|---|
| Nload | Installed | Monitors network traffic and bandwidth usage |
| Tcpdump | Installed | Captures network packets for analysis |

### Commands Used in the Lab

| Command | Action performed |
|---|---|
| `apt` | Displayed basic APT usage information |
| `sudo apt install nload` | Installed Nload |
| `nload -h` | Displayed Nload help and usage information |
| `sudo apt remove nload` | Removed Nload |
| `sudo apt install tcpdump` | Installed Tcpdump |
| `apt list --installed` | Listed installed packages |
| `sudo apt install nload` | Reinstalled Nload |

### What I Learned from the Lab

This lab gave me practical experience managing Linux software from the command line.

I learned that:

1. APT can be used to install and remove applications.
2. `sudo` is commonly required for administrative package-management tasks.
3. Running an application's help command can help verify whether its executable is available.
4. `apt list --installed` helps identify packages installed through APT.
5. Network tools such as Nload and Tcpdump can support network monitoring and investigation.

### Cybersecurity Applications of This Lab

Software management is important in cybersecurity because analysts must ensure that the tools required for an investigation are available.

These skills can be used to:

- Prepare a Linux environment for an investigation.
- Install approved network analysis tools.
- Verify that required packages are installed.
- Remove unnecessary software.
- Check whether tools are available before running them.
- Support troubleshooting and system administration.

**Key takeaway:** This lab demonstrated how to manage software packages in Linux using APT and verify the results through the command line.

---

## 12. Linux and Cybersecurity

Linux is an important platform for cybersecurity professionals because it supports command-line tools, automation, system administration, and security analysis.

### Network Monitoring

Tools such as Nload can help monitor network traffic and bandwidth usage.

This can be useful when troubleshooting connectivity issues or observing network utilisation.

### Packet Capture and Analysis

Tcpdump captures network packets for further analysis.

Packet captures can help analysts investigate:

- Unexpected network connections.
- Suspicious communication patterns.
- Network troubleshooting issues.
- Traffic between systems.
- Potentially malicious activity.

Packet captures may contain sensitive information, so they should be collected and handled in accordance with applicable policies and authorisation.

### Penetration Testing

Security-focused distributions such as Kali Linux provide tools for authorised security testing.

Penetration testing involves assessing systems for vulnerabilities within an approved scope.

### Digital Forensics

Digital forensics involves collecting, preserving, and analysing digital evidence.

Linux tools and security-focused distributions can support forensic workflows.

### System Administration

Security analysts may need to manage software, review system information, and use command-line utilities.

Understanding Linux commands and package management provides a foundation for these tasks.

---

## 13. Key Terms and Definitions

| Term | Definition |
|---|---|
| Operating System (OS) | System software that manages hardware and software resources |
| Linux | An open-source operating system family built around the Linux kernel |
| Open Source | Software whose source code is available under a licence that permits specified forms of use, inspection, modification, and distribution |
| GUI | Graphical User Interface; enables interaction through visual elements |
| CLI | Command-Line Interface; enables interaction through text-based commands |
| Shell | A command interpreter that accepts and executes commands |
| Kernel | The core of an operating system, responsible for managing system resources |
| Hardware | Physical components of a computer |
| CPU | Central Processing Unit; executes instructions |
| RAM | Random Access Memory; provides temporary working memory |
| FHS | Filesystem Hierarchy Standard; defines a standard organisation for Linux directories |
| Linux Distribution | A packaged Linux-based operating system with software and utilities |
| Kali Linux | A Debian-based distribution designed for information security work |
| Parrot | A Linux distribution with security- and privacy-focused editions |
| APT | Advanced Package Tool; manages software packages on Debian-based systems |
| Package | A software component distributed in a format that a package manager can install and manage |
| `sudo` | A command used to execute another command with elevated privileges |
| Nload | A command-line tool for monitoring network traffic and bandwidth usage |
| Tcpdump | A command-line tool for capturing network packets |
| Standard Input (stdin) | The data stream through which a program receives input |
| Standard Output (stdout) | The data stream used for normal program output |
| Standard Error (stderr) | The data stream commonly used for error messages and diagnostics |
| Command History | A record of previously entered commands maintained by the shell environment |

---

## 14. Important Commands to Remember

The following commands are useful starting points for working in a Linux terminal.

| Command | Purpose |
|---|---|
| `pwd` | Displays the current working directory |
| `ls` | Lists files and directories |
| `echo "Hello"` | Prints text to standard output |
| `apt` | Displays basic APT usage information |
| `sudo apt install package_name` | Installs a package |
| `sudo apt remove package_name` | Removes a package |
| `apt list --installed` | Lists installed packages |
| `nload -h` | Displays Nload help information when available |

### Example: Installing a Package

```bash
sudo apt install tcpdump
```

### Example: Listing Installed Packages

```bash
apt list --installed
```

### Example: Displaying Text

```bash
echo "I am learning Linux for cybersecurity"
```

Expected output:

```text
I am learning Linux for cybersecurity
```

**Note:** Commands may behave differently depending on the Linux distribution, installed packages, user permissions, and system configuration.

---

## 15. Key Lessons from Module 2

The most important lessons I took from this module are:

1. Linux is an open-source operating system widely used in technology and cybersecurity.
2. An operating system manages hardware and software resources.
3. The kernel is responsible for core operating system functions, including process and memory management.
4. The shell allows users to interact with Linux through text-based commands.
5. A GUI uses visual elements, while a CLI uses commands.
6. Linux architecture includes the user, applications, shell, kernel, hardware, and filesystem organisation.
7. Linux distributions provide different combinations of software and tools for different use cases.
8. Kali Linux and Parrot have security-focused editions and tools.
9. Wireshark is a network analysis application, not a Linux distribution.
10. Standard input, standard output, and standard error serve different purposes.
11. APT is used to manage software packages on Debian-based Linux systems.
12. `sudo` is commonly used when a command requires elevated privileges.
13. `apt list --installed` can help verify which packages are installed.
14. Nload supports network traffic monitoring, while Tcpdump supports packet capture.
15. Linux command-line skills provide a foundation for security operations and investigations.

---

## 16. Module Reflection

Completing this module improved my understanding of Linux and its role in cybersecurity.

Before this module, I understood that Linux was an operating system, but I needed a clearer understanding of its architecture and how users interact with it.

I learned the roles of the kernel, shell, applications, hardware, and filesystem organisation. I also developed a better understanding of the differences between a GUI and a CLI.

The practical APT lab was particularly useful because it allowed me to apply these concepts by installing, removing, reinstalling, and verifying software packages.

Working with Nload and Tcpdump also introduced me to tools that can support network monitoring and investigation.

### Skills Developed

- Linux fundamentals.
- Understanding operating system architecture.
- Command-line interface fundamentals.
- Linux distribution awareness.
- Software package management using APT.
- Basic software installation verification.
- Understanding network monitoring and packet capture tools.
- Identifying how Linux supports cybersecurity operations.

### Next Steps

To strengthen my Linux skills, I intend to practise:

- Navigating Linux directories.
- Creating, copying, moving, and removing files.
- Understanding file permissions.
- Working with users and groups.
- Searching and filtering command output.
- Reading system logs.
- Using command pipelines and redirection.
- Learning more about network analysis with Tcpdump.
- Building familiarity with Linux security tools in an authorised lab environment.

---

## 17. Module Completion

**Course:** Tools of the Trade: Linux and SQL  
**Module:** Module 2 — Linux  
**Status:** ✅ Completed

This module provided a foundation in Linux architecture, operating system concepts, command-line interaction, Linux distributions, and software package management.

The hands-on APT lab allowed me to practise installing, removing, reinstalling, and verifying applications.

These concepts will support my continued learning in cybersecurity, particularly in Linux administration, network analysis, security operations, and digital investigations.

**Next:** Continue to the next module in the Google Cybersecurity Professional Certificate.
