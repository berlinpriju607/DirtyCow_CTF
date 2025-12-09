# DirtyCow_CTF
Dirty COW is a privilege escalation vulnerability in the Linux kernel's memory subsystem, specifically in the Copy-On-Write (COW) mechanism. This flaw makes it possible to write to memory-mapped files that are supposed to be read-only, such as /etc/passwd, enabling attackers to escalate their privileges. Dirty COW affected almost every Linux kernel version released over the previous nine years and was widely used in real attacks especially on older kernels. The vulnerability was patched in October 2016 by fixing how the kernel handles copy-on-write memory operations.
## DirtyCow_Exploit

♦ Verified that the machine’s kernel version was vulnerable to the Dirty COW (CVE-2016-5195) 
privilege escalation flaw. 

♦ Downloaded a publicly available proof-of-concept exploit for educational and CTF purposes. 
[Dirty COW Official Website](https://dirtycow.ninja/)

♦ Compiled the exploit using `gcc -pthread dirtycow.c -o` dirty to create an executable 
payload. 

♦ Ran the exploit, which successfully abused the kernel race condition to overwrite protected 
system files. 

♦ Gained full root access on the JEELLY CTF target, allowing complete control over the system. 

♦ Retrieved the final flag after achieving root-level privileges. 



