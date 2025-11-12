# Low-Level Systems Simulators

Collection of low-level system simulators, including a cycle-accurate CPU (E20 Processor) and configurable L1/L2 caches (E20 Cache), written in C++. Provides detailed execution and memory logging for studying processor behavior, instruction execution, and cache performance. The E20 assembly language used by this simulator was originally developed by NYU Tandon for educational purposes.

## Features

- **E20 Processor Simulation**  
  - Implements arithmetic, logic, branching, memory, and jump instructions.  
  - Maintains program counter, general-purpose registers, and memory state.  

- **Cache Simulation**  
  - Supports configurable L1 and optional L2 caches.  
  - Configurable associativity, block sizes, and replacement policies (LRU).  
  - Logs cache hits, misses, and store operations for analysis.  

- **Flexible Configuration**  
  - Load programs from machine code files.  
  - Command-line arguments to configure cache size, associativity, and block size.  

## Usage

```bash
./simulator [--cache SIZE,ASSOC,BLOCK[,SIZE,ASSOC,BLOCK]] program.bin
