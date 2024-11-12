# What is a linux kernel？
A linux kernel is the only program that has direct access to hardware. 
* It is responsible for access and sharing the hardware in a secure and fair manner with muliple applications.
* It offers a set of APIs that applications issue which are generally referred to as system calls.

## User Mode vs. Kernel Mode
* Code that runs in kernel model can fully control the CPU.
* Code that runs in user mode has certain limitations.

## User Space vs. Kernel Space
The kernel spece is the memory area that is reserved to kernel. 
It is accessed protected so that user applications can not access it directly.

The user space is the memory area that is reserved to a particular user process. 
It can be directly accessed from code running in kernel mode.

# How does a linux kernel work?
A linux kernel is made up of six distinct layers, or subystems that enables its core functions:
## System Call Implementation
   This layer carries the functionality that allows the kernel to execute system calls from user space into the kernel space.
* process management
* memory management
* virtual memory
* network stack
* device drivers





# System Calls
A system call is an interface between user space and kernel space. 
In order to provide application compatiability, system calls are rarely changed.


Every system call is assigned a system call number.
When a user space program makes a system call, it doesn't directly invoke a kernel function.
Instead, it uses a system call number to reference desired system call.
This mechanism maintains a consistent interface, even as underlying system call implementations evolve. 

# System Call Wrappers


