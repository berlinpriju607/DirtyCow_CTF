# DirtyCow_CTF
Dirty COW is a privilege escalation vulnerability in the Linux kernel's memory subsystem, specifically in the Copy-On-Write (COW) mechanism.

And here, Dirty COW (CVE-2016-5195) is a well-known privilege escalation vulnerability affecting the Linux kernel’s 
copy-on-write (COW) mechanism. It occurs due to a race condition that allows an unprivileged local user to 
write to read-only memory mappings. By exploiting this flaw, an attacker can overwrite critical system files—
often /etc/passwd—to gain root access. The exploit is stable, widely documented, and works reliably on 
older kernels like 3.13.0-32. In this challenge, the vulnerability provided a viable method to escalate 
privileges to root on the JEELLY target machine. 



