# List of Potential Topics for Musing

- [Embedded Linux status](https://static.sched.com/hosted_files/eoss2023/68/Debating-Linux-in-Aerospace%20-VanderLeest-Brink.pdf)
- [Async spawn using io_uring](https://lwn.net/Articles/908268/)
- [Open vs. closed workload generators](https://brooker.co.za/blog/2023/05/10/open-closed.html)
- [Deep dive on how to think about performance](https://docs.google.com/presentation/d/1wOT5kOWkQybVTHzB7uLXpU39ctYzXpOs2xVyD4zuYXY/edit#slide=id.g809d36a3fc4b213_287 )
- [Zephyr: a modular OS for resource-constrained devices](https://lwn.net/Articles/925924/)
- [Heuristics for software-interrupt processing](https://lwn.net/Articles/925540/)
- [An EEVDF CPU scheduler for Linux](https://lwn.net/Articles/925371/)
- Architecture of modern LLM infrastructures that require singificant context (for example, [this](https://about.sourcegraph.com/blog/cody-is-cheating), and [this](https://about.sourcegraph.com/whitepaper/cody-context-architecture.pdf))
- x86_64 [code optimizations, exception handling, and calling conventions](https://codemachine.com/articles/x64_deep_dive.html)
- Hiding memory access latency on [in-order architectures](https://johnnysswlab.com/hiding-memory-latency-with-in-order-cpu-cores-or-how-compilers-optimize-your-code/)
- Understanding processor pipeline [dependencies](https://johnnysswlab.com/when-an-instruction-depends-on-the-previous-instruction-depends-on-the-previous-instructions-long-instruction-dependency-chains-and-performance/), and how to hide memory access latencies [using instruction-level parallelism on out-of-order machines](https://johnnysswlab.com/instruction-level-parallelism-in-practice-speeding-up-memory-bound-programs-with-low-ilp/)

# Topics we've discussed (but can revisit)

- [Position-independent Code/Executables](https://eli.thegreenplace.net/2011/11/11/position-independent-code-pic-in-shared-libraries-on-x64) including the GOT and PLT
- [Thread-Local Storage](https://chao-tic.github.io/blog/2018/12/25/tls), [other examples](https://maskray.me/blog/2021-02-14-all-about-thread-local-storage), [details](https://akkadia.org/drepper/tls.pdf)
- [Zero-copy I/O for ublk, three different ways](https://lwn.net/Articles/926118/)
- Understanding compiler optimizations, and their interactions with link-time optimization.
