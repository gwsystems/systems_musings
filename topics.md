# List of Potential Topics for Musing

- Understanding [bugs in embedded systems](https://dl.acm.org/doi/10.1145/3597926.3598140)
- [Deep dive on how to think about performance](https://docs.google.com/presentation/d/1wOT5kOWkQybVTHzB7uLXpU39ctYzXpOs2xVyD4zuYXY/edit#slide=id.g809d36a3fc4b213_287 )
- [Zephyr: a modular OS for resource-constrained devices](https://lwn.net/Articles/925924/)
- [Heuristics for software-interrupt processing](https://lwn.net/Articles/925540/)
- [An EEVDF CPU scheduler for Linux](https://lwn.net/Articles/925371/)
- Architecture of modern LLM infrastructures that require singificant context (for example, [this](https://about.sourcegraph.com/blog/cody-is-cheating), and [this](https://about.sourcegraph.com/whitepaper/cody-context-architecture.pdf))
- Hiding memory access latency on [in-order architectures](https://johnnysswlab.com/hiding-memory-latency-with-in-order-cpu-cores-or-how-compilers-optimize-your-code/)
- Understanding processor pipeline [dependencies](https://johnnysswlab.com/when-an-instruction-depends-on-the-previous-instruction-depends-on-the-previous-instructions-long-instruction-dependency-chains-and-performance/), and how to hide memory access latencies [using instruction-level parallelism on out-of-order machines](https://johnnysswlab.com/instruction-level-parallelism-in-practice-speeding-up-memory-bound-programs-with-low-ilp/)
- Parallelism in [javascript](https://webkit.org/blog/7846/concurrent-javascript-it-can-work/)
- User-level synchronization in a [browser, including the popular parking lot mechanisms](https://webkit.org/blog/6161/locking-in-webkit/)
- C [cleanup attributes](https://lwn.net/Articles/934679/) - should we use a non-standard extension?
- [Addressing priority inversion with proxy execution](https://lwn.net/Articles/934114/)
- [Deadline servers as a realtime throttling replacement](https://lwn.net/Articles/934415/)
- [Optimizing single-owner memory](https://lwn.net/Articles/932391/)
- [Mitigating vmap lock contention](https://lwn.net/Articles/932396/) and [Improving page-fault scalability](https://lwn.net/Articles/932298/)
- [Memory passthrough for virtual machines](https://lwn.net/Articles/931933/)
- [1½ Topics: realtime throttling and user-space adaptive spinning](https://lwn.net/Articles/931789/)
- [User-space control of memory management](https://lwn.net/Articles/931662/)
- [Complexities of directed yield](https://lwn.net/Articles/419961/)
- [Latency management in the scheduler (old)](https://lwn.net/Articles/404993/)
- [Core scheduling to avoid SMT/hyperthreading sidechannels](https://lwn.net/Articles/780703/) and [potential uses](https://lwn.net/Articles/799454/)
- Can we find an article on KPI (kernel page-table isolation)?
- Risc-V bootup procedures vs. x86

# Scheduled Discussions

- Elf [relocations](https://intezer.com/blog/malware-analysis/executable-and-linkable-format-101-part-3-relocations/)
- [Async spawn using io_uring](https://lwn.net/Articles/908268/)
- [Open vs. closed workload generators](https://brooker.co.za/blog/2023/05/10/open-closed.html)

# Index of LWN articles

See the great [index](https://lwn.net/Kernel/Index/) of all of the LWN kernel articles. 
Makes it easier to browse through them to find whatever you're interested in.

# Topics we've discussed (but can revisit)

- x86_64 [code optimizations, exception handling, and calling conventions](https://codemachine.com/articles/x64_deep_dive.html)
- [Embedded Linux status](https://static.sched.com/hosted_files/eoss2023/68/Debating-Linux-in-Aerospace%20-VanderLeest-Brink.pdf)
- [Speculation in Javascript](https://webkit.org/blog/10308/speculation-in-javascriptcore/) that also covers JIT compilation
- [x86 boot process/procedure](https://0xax.gitbooks.io/linux-insides/content/Booting/linux-bootstrap-1.html)
- [Position-independent Code/Executables](https://eli.thegreenplace.net/2011/11/11/position-independent-code-pic-in-shared-libraries-on-x64) including the GOT and PLT
- [Thread-Local Storage](https://chao-tic.github.io/blog/2018/12/25/tls), [other examples](https://maskray.me/blog/2021-02-14-all-about-thread-local-storage), [details](https://akkadia.org/drepper/tls.pdf)
- [Zero-copy I/O for ublk, three different ways](https://lwn.net/Articles/926118/)
- Understanding compiler optimizations, and their interactions with link-time optimization.
