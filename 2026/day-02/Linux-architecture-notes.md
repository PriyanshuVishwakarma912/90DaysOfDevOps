# Understanding the linux fundamentals (Internal working).
## Core components of linux.
  - 1. Kernel :-  Kernel is the main core part of the Linux os. kernel is the heart of the os , without kernel linux is dead. It connects hardware with the software.
          - what it does:
          - Interact or talk with the hardware,
          - Controls cpu,RAM, Disk,
          - Decide which program runs,
          - It protects the whole system
          - kernel runs in kernel mode.
  - 2. Process Management :- It is a part of the kernel that manages the running programs.
          - What is does:
          - Create processes,
          - kill processes,
          - switch CPU between programs.
  - 3. Memory Management :- A kernel component that manages RAM.
          - What it does:
          - Gives memory to program,
          - Take its back,
          - Uses disk as backup(Swap).
  - 4. File System :- In file system linux stores and organizes data. In linux everything is a file.
          - Important directories
          - / → root
          - /home → users
          - /etc → config files
          - /bin → basic commands
          - /var → logs
          - /dev → devices
  - 5. Shell :- Shell is a translator between you and Linux.
          - What it does:
          - Reads your command
          - Finds correct program
          - Executes it
      
  - 6. Init System :- It is a first program which is started by kernel.
    
## How Processes are created and managed in linux?
  - A process in Linux is a running program that the kernel manages by giving it a process ID (PID), CPU time, memory, and other resources.
      - In Linux everything you run is a process.
      - A new process is created using the fork() system call:
          - The parent process makes a copy of itself → child process.
      - To run a different program, the child uses exec():
- This replaces the child’s code with the new program.
👉 Example: When you type ls in the terminal:
- The shell (parent process) uses fork() to create a child.
- The child uses exec() to load and run the ls program.

🔹 Process Management
- Each process has a PID (Process ID).
- The kernel keeps track of all processes.
- Processes can be in states like:
- Running (using CPU),
- Waiting (for input/output),
- Stopped (paused),
- Zombie (finished but not cleaned up).
- The scheduler decides which process runs on the CPU.
- Parent processes can monitor children using wait().

🔹 In Short
- fork() → creates a new process.
- exec() → runs a new program inside it.
- Kernel + scheduler → manage processes.
- PID → unique ID for each process.
  
## What system does and why it matters in linux?
  - systemd is the init system (the first program that runs when Linux boots).
  - It's responsible for:
      - Starting services (like networking, logging, graphical interface).
      - Managing processes (keeping them running, restarting if they fail).
      - Handling dependencies (making sure that services start in the right order).
      - Logging (collecting system messages for troubleshooting).
  - why it matters:-
      - Boot speed
      - Reliability
      - Consistency
      - Control
      - Monitoring


      
