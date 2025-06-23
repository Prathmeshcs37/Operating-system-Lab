# Operating-system-Lab

A set of xv6 operating system extensions developed as part of CS3500: Operating Systems.

## Labs Overview

### Lab 2: System Calls
- Added custom syscalls: `echo_simple`, `echo_kernel`, `trace`, `get_process_info`
- Enabled syscall argument tracing

### Lab 3: Memory Management
- Implemented `vmprint` to display page tables
- Disabled memory allocation in `sbrk()`
- Added lazy allocation on page faults

### Lab 4: Kernel Stack & Context
- Used `qemu-gdb` to analyze RISC-V assembly
- Implemented `backtrace()` using frame pointers
- Introduced `pcbread` syscall to inspect PCB and trapframe state

### Lab 5: Signals
- Added `sigalarm()` to trigger user-defined handlers after n ticks
- Implemented `sigreturn()` to resume execution
- Passed correctness tests via `alarmtest` and `usertests`

### Lab 6: Copy-On-Write (COW)
- Optimized `fork()` using shared read-only pages
- Handled write faults with on-demand copying
- Implemented reference counting and COW-aware `copyout()`

