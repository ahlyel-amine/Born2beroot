# Born2beroot

**How a VM work**

VM simply is a software that simulate the hardware of a physical computer wich he allows to run multiple OS's on a single machine, isolating them from each other (host machine included).

- A virtual machine (VM) works by using a piece of software called a hypervisor, which runs on the host computer and creates a virtual environment for the guest operating system to run in. When you start a VM, the hypervisor creates a virtual version of the hardware components that the guest OS needs to run, such as a virtual CPU, memory, and storage. The guest OS then runs on top of this virtual hardware, just as it would on a physical computer.

**Basic difference between centos and debian**

CentOS and Debian are two different Linux distributions. Both are open source and free to use. Here are a few key differences between the two:

- Package management: CentOS uses the yum package manager, while Debian uses apt.
- Release cycle: CentOS releases are less frequent and are more stable and conservative, while Debian releases are more frequent and include newer software.
- Target audience: CentOS is often used by businesses and organizations because of its stability, while Debian is more popular among individuals and developers.

Overall, the choice between CentOS and Debian will depend on your specific needs and preferences. Both distributions have their own strengths and can be used effectively in different situations.

**The purpuse of virtual machine**

- Testing and development: You can use a virtual machine to test new software or make changes to an operating system without affecting your main computer.

- Isolation and security: By running a separate operating system in a virtual machine, you can isolate it from your main system and prevent any potential security risks or vulnerabilities from affecting your main computer.

- Compatibility: You can use a virtual machine to run an older operating system or applications that are not compatible with your current system.
- Resource management: You can use multiple virtual machines to run different applications or operating systems on the same physical machine, allowing you to efficiently use your hardware resources.

Overall, virtual machines offer a convenient and flexible way to run multiple operating systems and applications on a single computer.

**Difference between apt and aptitude**

`apt` and `aptitude` are both package management tools for Debian and Debian-based Linux distributions. Both tools are used to install, remove, and manage packages on the system.

- `apt` is a command-line tool that is used to manage packages through the use of various subcommands, such as install, remove, and upgrade. `aptitude` is also a command-line tool, but it has a more user-friendly interface and allows you to perform package management tasks through an interactive menu.

- `apt` uses the dpkg package manager under the hood to manage packages, while aptitude uses its own package manager.

- `aptitude` has additional features that are not available in apt, such as the ability to resolve dependencies automatically and the ability to mark packages as "automatically installed" so that they can be automatically removed when they are no longer needed.

Overall, both `apt` and `aptitude` are useful tools for package management on Debian-based systems. You can choose the tool that best fits your needs and preferences.

**AppArmor**

`AppArmor` (Application Armor) is a Linux security module that allows system administrators to restrict the actions that programs can perform on a system. It is similar to other mandatory access control systems, like SELinux, but is more lightweight and easier to use. With AppArmor, administrators can specify rules that determine what system resources (such as files, network sockets, and interprocess communication mechanisms) a program is allowed to access. If a program tries to access a resource that is not allowed by its AppArmor profile, the access is denied and an alert is generated. AppArmor is often used to improve the security of system services and third-party applications by limiting their potential attack surface.

**What is LVM and how it works**

Logical Volume Manager `LVM` is a system for managing disk storage in Linux. It allows you to create logical volumes, which are abstractions of physical storage devices, and to manage them as a single entity.

Here's how `LVM` works at a high level:

- Physical storage devices, such as hard drives or partitions, are grouped together into volume groups `VGs`.

- Each `VG` is divided into logical volumes `LVs`.

- The `LVs` can be treated as normal block devices, such as hard drives or partitions. They can be formatted with a filesystem and mounted like any other storage device.

- The `LVs` can be resized or moved to different `VGs` without the need to reformat or move data. This allows for greater flexibility in allocating storage and making use of available space.

- `LVM` also provides features for snapshotting and mirroring LVs, which can be useful for backup and disaster recovery purposes.

`LVM` is useful for managing large amounts of storage, particularly in enterprise environments. It allows administrators to easily allocate and manage storage resources without the need to worry about the underlying physical devices.

**What is FireWall**

A firewall is a security system that controls incoming and outgoing network traffic based on predetermined security rules. A firewall can be implemented as hardware, software, or a combination of both.

- Firewalls are used to protect private networks from external threats, such as hackers and malware. They do this by examining each incoming and outgoing network connection and allowing or blocking the connection based on a set of rules. These rules are typically defined by the system administrator, and they can be based on a variety of criteria, such as the source and destination IP addresses, the protocol being used, and the port number.

- Firewalls can be configured to allow all traffic, block all traffic, or allow only certain types of traffic. They can also be configured to log connections, alert the administrator to suspicious activity, and take other actions as needed.

- Firewalls are an important part of a secure network. They can help to prevent unauthorized access and protect against external threats.

**What is UFW**

Uncomplicated Firewall (UFW) is a firewall software program for Linux systems. It is designed to be easy to use and to provide a basic level of security for a system.

- UFW operates by defining a set of rules that specify which network connections are allowed or denied. These rules are stored in a firewall policy, and UFW enforces the policy by modifying the system's firewall settings.

**What is SSH**

Secure Shell (SSH) is a network protocol used to securely connect to a remote computer. It is often used to log into a server, execute commands, and transfer files.

SSH uses encryption to secure the connection between the client and the server. It authenticates the client and the server using public keys and a trusted third party, and it allows the client and the server to authenticate each other using a shared secret.

SSH is commonly used to access servers over a network. It is often used as an alternative to Telnet, which transmits data in plaintext and is susceptible to interception and tampering. SSH is also used to remotely administer servers, configure network devices, and automate tasks.

SSH is available for a wide range of operating systems, including Linux, Unix, macOS, and Windows. It is an important tool for system administrators and other IT professionals who need to securely access and manage remote systems.

**What is cron**

Cron is a time-based job scheduler in Linux and Unix-like operating systems. It allows users to schedule tasks to be executed automatically at a specified time or interval.

Cron is typically used to perform routine maintenance tasks, such as backing up files or cleaning up temporary directories. It can also be used to run custom scripts or programs on a regular basis.

In Cron, tasks are defined using crontab files. A crontab file is a text file that contains a list of commands, one command per line. Each line in a crontab file has a specific format that specifies when the command should be executed and what command should be run.

Crontab files are stored in the `/etc/crontab` directory, and each user can also have their own crontab file in the `/var/spool/cron` directory. The system administrator can use the crontab command to manage the crontab files for the system and for individual users.

Cron is a useful tool for automating tasks and maintaining a system. It is often used by system administrators and other IT professionals to automate routine tasks and to ensure that systems are running smoothly.
