 BYTE Cybersecurity Recruitment - Task 03: Binary Exploitation

This repository contains the solution and exploit script for **Task 03 (Binary Exploitation)** from the [BYTE Cybersecurity Recruitment Portal](https://bytesoc.dev/tasks/cybersecurity/)[cite: 2].

 Challenge Overview
Type: Binary Exploitation (Buffer Overflow).
Remote Endpoint: `nc cybersub.bytesoc.dev 9999`.
Objective:Exploit an insecure memory buffer to reach the section of the program containing the flag in the `BYTE{...}` format[cite: 2].



Steps to Run and Solve

A. Local Setup:
   1) Download the challenge archive from the [portal](https://bytesoc.dev/tasks/cybersecurity/).
   2) Extract all files (`chall.sh`, dummy binary `chall`) into the `task03_pwn/` folder.
   3) Run the local script to test behavior:
     bash
     ./chall.sh
     
B. Analysis:
   1) Disassemble the dummy binary using Ghidra or GDB to find the vulnerable input buffer and determine the required offset for the instruction pointer overwrite. *(Note: The local dummy binary contains a fake flag; the real flag is fetched remotely).

C. Execution:
    Install dependencies and run the exploit script against the remote target service:
     bash
     pip install pwntools
     python3 task03_pwn/exploit.py
     
