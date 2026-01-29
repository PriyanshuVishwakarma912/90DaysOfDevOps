# Understandidng the linux fundamentals (Internal working).
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
  - 5. Device Drivers :- Drivers are translators between kernel and hardware. It is needed because, Hardware understands signals, not commands.
          - Devices like -> Keyboard , mouse ,printer.
  - 6. Shell :- Shell is a translator between you and Linux.
          - What it does:
          - Reads your command
          - Finds correct program
          - Executes it
      
  - 7. Init System :- It is a first program which is started by kernel.
       
