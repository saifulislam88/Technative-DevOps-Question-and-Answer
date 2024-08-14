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

##### 📌 Process

**1.** A process is an instance of a running program. It is the basic unit of execution in Linux.\
**2.** Each process has its own memory space, and it can perform tasks independently.

**Example:** Running firefox creates a process for the Firefox web browser.

**Relation to Others:**\
`A process can create multiple threads to perform tasks concurrently. A daemon is a type of process that runs in the background.`

