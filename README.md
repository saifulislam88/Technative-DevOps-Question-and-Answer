- [System Administration](#System-Administration)
  - [Difference between Linux & Windows](#Difference-Between-Linux-and-Windows)
  - [A concise explanation of Process, Thread, Daemon, and Service](#process-thread-daemon-service)
  - [](#)
  - [](#)
  - [](#)
  - [](#)
  - [](#)
  - [](#)
  - [](#)






## System Administration🚀

## [Difference between Linux and Windows]()

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


## [Process-Thread-Daemon-Service]()

Here's a concise explanation of `processes`, `threads`, `daemons`, and `services` in Linux, along with examples and their relationships:

### 📌[Process]()

- A process is an instance of a running program. It is the basic unit of execution in Linux.\
- Each process has its own memory space, and it can perform tasks independently.\
- A process can creates other processes which are known as Child Processes.

🔄**Example:** Running firefox creates a process for the Firefox web browser. When you run **`ls -la`**, it creates a temporary process that executes the command and produces output. 

⏰**Relation to threads & daemon:**\
**`A process can create multiple threads to perform tasks concurrently. A daemon is a type of process that runs in the background.`**

------------------------------------------------------------------------------------------------------------------------------

### 📌[Thread]()                                                                                                     

- A thread is the smallest unit of a process that can be scheduled by the operating system.\
- Threads share the same memory space and resources of the parent process but run independently.\
- A thread have 3 states: running, ready, and blocked

🔄**Example:** In a web server like Apache, each request might be handled by a separate thread within the same process.

⏰**Relation to process:**\
**`Threads exist within a process and share its resources. Multiple threads can run simultaneously within the same process.`**

------------------------------------------------------------------------------------------------------------------------------

### 📌[Daemon]()

- A daemon is a background process that runs continuously and is usually started at boot time.
- Daemons typically provide system or network services.

🔄**Example:** **`cron`** is a daemon that executes scheduled tasks & **`httpd`** handles incoming HTTP requests and serves web pages.

⏰**Relation to process:**\
**`A daemon is a type of process, but it runs in the background and is detached from any terminal session.`**

------------------------------------------------------------------------------------------------------------------------------

### 📌[Service]()

- A service is a specific function or set of functions provided by the operating system, usually managed by a daemon.
- Services are typically started at boot and managed by service managers like systemd.

🔄**Example:** `nginx` as a web server service that is managed by the `nginx` daemon.

⏰**Relation to daemon:**\
**`A service is provided by a daemon process. Services can involve multiple processes and threads to perform their tasks.`**

------------------------------------------------------------------------------------------------------------------------------

### 📌[Relationships]()

- A process is an independent program, while threads are the sub-units of a process, sharing its resources.
- All daemons are processes, but not all processes are daemons. Daemons run in the background and provide services.
- A service is typically provided by a daemon. The daemon manages the process(es) that provide the service.




