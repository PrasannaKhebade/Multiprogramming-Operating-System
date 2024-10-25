# Multiprogramming Operating System (MOS) Project

## Overview
This project simulates the working of a multiprogramming operating system (MOS) by managing multiple processes, handling interrupts, and managing memory through paging techniques. The simulation incorporates different phases to demonstrate basic and advanced features of an operating system such as job scheduling, error handling, and interrupt management. 

## Phase 1: Initial Implementation of MOS  
In the first phase, the MOS simulation focuses on executing a single program at a time, ensuring basic process execution with simple control flow and limited error handling. Key aspects include:
- **Job Execution**: Only one job is loaded and executed at a time.
- **Interrupt Handling**: Basic service interrupts (SI) are implemented for:
  1. Input requests (GD)
  2. Output requests (PD)
  3. Program termination (H)
- **Assumptions**: 
  - No physical separation between jobs in memory.
  - Program is loaded at memory location 00.
  - Job outputs are separated by two blank lines in the output file.
  - Programs without errors are assumed for input files.

## Phase 2: Advanced MOS Features  
The second phase adds paging, error handling, and multi-level interrupts to enhance the simulation with real-world complexities. Key improvements include:
- **Memory Management with Paging**: 
  - A page table is stored in real memory, and pages are allocated using a random block generator.
- **Interrupt Handling**: 
  - Program Interrupt (PI) for operation and operand errors.
  - Timer Interrupt (TI) for time-limit exceeded errors.
- **Advanced Error Management**: 
  - Time limit, line limit, and out-of-data errors are introduced.
  - Error messages are coded to indicate specific termination causes (e.g., invalid page faults, operation code errors).
- **Process Control Block (PCB)**: 
  - A data structure is used to manage process details.
- **Queue-based Execution**: 
  - Programs are loaded sequentially, and execution continues with appropriate handling of page faults and timeouts.

This two-phase approach offers a comprehensive understanding of how multiprogramming operating systems function by gradually incorporating memory management, interrupts, and error handling mechanisms.
