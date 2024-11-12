# System Calls
The kernel is the only program that has direct access to hardware. 
* It is responsible for access and sharing the hardware in a secure and fair manner with muliple applications.
* It offers a set of APIs that applications issue which are generally referred to as system calls.

In order to provide application compatibility, system calls are rarely changed.


## User Mode vs. Kernel Mode
* Code that runs in kernel model can fully control the CPU.
* Code that runs in user mode has certain limitations.

## User Space vs. Kernel Space
The kernel spece is the memory area that is reserved to kernel. 
It is accessed protected so that user applications can not access it directly.

The user space is the memory area that is reserved to a particular user process. 
It can be directly accessed from code running in kernel mode.

# System Calls
A system call is an interface between user space and kernel space. 
In order to provide application compatiability, system calls are rarely changed.

Every system call is assigned a unique number, known as the sytem call number.
When a user space program makes a system call, it doesn't directly invoke a kernel function.
Instead, it uses a numerical identifier to reference the desired system call.
In turn, the kernel uses this identifier to determine an appropriate function to execute.
This mechanism maintains a consistent interface, even as the underlying system call implementations evolve. 

