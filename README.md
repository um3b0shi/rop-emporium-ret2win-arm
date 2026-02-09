# rop-emporium-ret2win-arm
A walkthrough of the ROP Emporium ret2win challenge on ARMv5.

If you’re learning binary exploitation, ARM challenges can feel like a big jump from x86. Even simple ret2win-style problems suddenly come with new registers, emulation, and a slightly different debugging setup.
In this post, I walk through the ret2win challenge from ROP Emporium for ARMv5. We’ll identify a stack buffer overflow, find the correct offset, and redirect execution to the `ret2win` function, all while running the binary under QEMU.
The aim here is to keep things straightforward. Rather than diving deep into ARM internals, the focus is on building confidence and showing that the fundamentals of exploitation don’t change just because the architecture does.

