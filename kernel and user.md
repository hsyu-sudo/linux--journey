The kernel is the only program that has direct access to hardware. 
* It is responsible for access and sharing the hardware in a secure and fair manner with muliple applications.
* It offers a set of APIs that applications issue which are generally referred to as system calls.
  * In order to provide application compatibility, system calls are rarely changed.

## User Mode vs. Kernel Mode
* Code that runs in kernel model can fully control the CPU.
* Code that runs in user mode has certain limitations.

## User Space vs. Kernel Space
* The kernel spece is the memory area that is reserved to kernel. It is accessed protected so that user applications can not access it directly.
* The user space is the memory area that is reserved to a particular user process. It can be directly accessed from code running in kernel mode.
