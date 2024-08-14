- [System Administration](#System-Administration)
  - [Difference Between Linux & Windows](#Difference-Between-Linux-and-Windows)
  - [A concise explanation of process, thread, daemon, and service](#Process-Thread-Daemon-Service)
  - [](#)
  - [](#)
  - [](#)
  - [](#)
  - [](#)
  - [](#)
  - [](#)






### System Administration

#### 🚀 Difference Between Linux and Windows

| **Key Diff**               | **Linux OS**                                                                                     | **Windows**                                                |
|----------------------------|--------------------------------------------------------------------------------------------------|------------------------------------------------------------|
| **Licensing**              | Open Source                                                                                      | Closed Source                                              |
| **Customizable**           | Can modify & redistribute                                                                        | Can’t modify & redistribute                                |
| **User Comfort**           | Less user-friendly                                                                               | Almost user-friendly                                       |
| **Kernel Type**            | Monolithic                                                                                       | Hybrid                                                     |
| **Manufacturer**           | Developed by the community (overseen by Linus Torvalds)                                          | Microsoft                                                  |
| **File System**            | ext2, ext3, ext4, NTFS, FAT, XFS                                                                 | NTFS, FAT                                                  |
| **Programm**               | C                                                                                                | Assembly, C, C++                                           |
| **Boot Time**              | Faster (drivers loaded dynamically)                                                              | Slower (all drivers loaded at boot)                        |
| **Security**               | High                                                                                             | Lower compared to Linux                                    |
| **License**                | GNU Public License                                                                               | Proprietary                                                |
| **Preceded by**            | Basic Terminal (CLI)                                                                             | MS-DOS                                                     |
| **Usage**                  | Installable on a wide range of hardware (phones, tablets, consoles, mainframes, supercomputers)  | Mainly on PCs, desktops, laptops, servers                  |
| **OS Family**              | GNU                                                                                              | DOS                                                        |


#### 🚀 Process-Thread-Daemon-Service

##### 📌 [Process]()

- A process is an instance of a running program. It is the basic unit of execution in Linux.
- Each process has its own memory space, and it can perform tasks independently.
- A process can creates other processes which are known as Child Processes.

**Example:** Running firefox creates a process for the Firefox web browser. When you run **`ls -la`**, it creates a temporary process that executes the command and produces output. 

**Relation to threads & daemon:**\
`A process can create multiple threads to perform tasks concurrently. A daemon is a type of process that runs in the background.`

##### 📌 [Thread]()

- A thread is the smallest unit of a process that can be scheduled by the operating system.
- Threads share the same memory space and resources of the parent process but run independently.
- A thread have 3 states: running, ready, and blocked

**Example:** In a web server like Apache, each request might be handled by a separate thread within the same process.

**Relation to process:**
Threads exist within a process and share its resources. Multiple threads can run simultaneously within the same process.



