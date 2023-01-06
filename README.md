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
