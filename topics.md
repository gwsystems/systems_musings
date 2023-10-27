# Scheduled Discussions

We'll discuss the first time on this list in the next meeting. 
Make sure to scan the articles, and come with questions.

- We need a topic!!!

Add more links.

# List of Potential Topics for Musing

- Performing customizable static analysis on system code with [semgrep](https://semgrep.dev/blog/2021/semgrep-a-static-analysis-journey/) (previously [Coccinelle](https://lwn.net/Articles/698724/), which has long been used in the Linux kernel).
- Making a [micro-Linux distribution](https://popovicu.com/posts/making-a-micro-linux-distro/) (similar to [Linux from Scratch](https://www.linuxfromscratch.org/))
- Latencies and debugging latencies in the [linux scheduler](https://bristot.me/linux-scheduling-latency-debug-and-analysis/)
- Understanding [bugs in embedded systems](https://dl.acm.org/doi/10.1145/3597926.3598140)
- [Zephyr: a modular OS for resource-constrained devices](https://lwn.net/Articles/925924/)
- [Heuristics for software-interrupt processing](https://lwn.net/Articles/925540/)
- [An EEVDF CPU scheduler for Linux](https://lwn.net/Articles/925371/)
- Architecture of modern LLM infrastructures that require singificant context (for example, [this](https://about.sourcegraph.com/blog/cody-is-cheating), and [this](https://about.sourcegraph.com/whitepaper/cody-context-architecture.pdf))
- Hiding memory access latency on [in-order architectures](https://johnnysswlab.com/hiding-memory-latency-with-in-order-cpu-cores-or-how-compilers-optimize-your-code/)
- Parallelism in [javascript](https://webkit.org/blog/7846/concurrent-javascript-it-can-work/)
- User-level synchronization in a [browser, including the popular parking lot mechanisms](https://webkit.org/blog/6161/locking-in-webkit/)
- C [cleanup attributes](https://lwn.net/Articles/934679/) - should we use a non-standard extension?
- [Addressing priority inversion with proxy exechttps://us02web.zoom.us/j/82762395983?pwd=QTQ5bWpaVytaMHFkVXBUV0c5MmVwdz09#successution](https://lwn.net/Articles/934114/)
- [Deadline servers as a realtime throttling replacement](https://lwn.net/Articles/934415/)
- [Optimizing single-owner memory](https://lwn.net/Articles/932391/)
- [Mitigating vmap lock contention](https://lwn.net/Articles/932396/) and [Improving page-fault scalability](https://lwn.net/Articles/932298/)
- [Memory passthrough for virtual machines](https://lwn.net/Articles/931933/)
- [1½ Topics: realtime throttling and user-space adaptive spinning](https://lwn.net/Articles/931789/)
- [User-space control of memory management](https://lwn.net/Articles/931662/)
- [Complexities of directed yield](https://lwn.net/Articles/419961/)
- [Core scheduling to avoid SMT/hyperthreading sidechannels](https://lwn.net/Articles/780703/) and [potential uses](https://lwn.net/Articles/799454/)
- Can we find an article on KPI (kernel page-table isolation)?
- Risc-V bootup procedures vs. x86
- Detailed [architectural summary of Intel's Sandy Bridge](https://chipsandcheese.com/2023/08/04/sandy-bridge-setting-intels-modern-foundation/)
- Attempts to make it so that [bpf can execute unpriv](https://lwn.net/Articles/935195/) code.
- [Scheduling](https://lwn.net/Articles/935180/): pluggable bpf scheduling, priority inheritance through proxy execution, and different timer structures
- Page management and tracking in Linux. [struct page](https://lwn.net/Articles/937839/) (vs. [Composite's](https://github.com/gwsystems/composite/blob/v4/src/kernel/include/resources.h#L10-L17)), generalizing into [folios](https://lwn.net/Articles/849538/), and general page [management](https://lwn.net/Articles/619514/)
- Biased [reference counts](https://dl.acm.org/doi/10.1145/3243176.3243195) used in the new Python [PIP](https://lwn.net/Articles/940290/) to remove the GIL
- Software interrupts, and [where it is all going](https://lwn.net/Articles/939973/) in Linux
- [Mimalloc](https://www.microsoft.com/en-us/research/uploads/prod/2019/06/mimalloc-tr-v1.pdf), [TCmalloc](https://goog-perftools.sourceforge.net/doc/tcmalloc.html), [jemalloc](https://engineering.fb.com/2011/01/03/core-data/scalable-memory-allocation-using-jemalloc/)
- [Linux in mixed-criticality systems](https://lwn.net/Articles/774217/),[A discussion on Linux in space](https://lwn.net/Articles/938779/)
- [Challenges for KernelCI](https://lwn.net/Articles/939538/)
- All things [cgroups](https://lwn.net/Kernel/Index/#Control_groups-LWNs_guide_to)...this would likely take a couple of weeks.
- [How Garbage Collection works in Java? Explained](https://javarevisited.blogspot.com/2011/04/garbage-collection-in-java.html)

# Index of LWN articles

See the great [index](https://lwn.net/Kernel/Index/) of all of the LWN kernel articles. 
Makes it easier to browse through them to find whatever you're interested in.

# Topics we've discussed (but can revisit)

- Understanding processor pipeline [dependencies](https://johnnysswlab.com/when-an-instruction-depends-on-the-previous-instruction-depends-on-the-previous-instructions-long-instruction-dependency-chains-and-performance/), and how to hide memory access latencies [using instruction-level parallelism on out-of-order machines](https://johnnysswlab.com/instruction-level-parallelism-in-practice-speeding-up-memory-bound-programs-with-low-ilp/)
- Zenbleed https://lock.cmpxchg8b.com/zenbleed.html (Please add more links)
- [Latency management in the scheduler (old)](https://lwn.net/Articles/404993/)
- [9/12/2023] Linker scripts in detail. [Link](https://mcyoung.xyz/2021/06/01/linker-script/) The [composite loader](https://github.com/gwsystems/composite/blob/main/src/kernel/include/shared/elf_loader.h), which assumes the [linker script](https://github.com/gwsystems/composite/blob/main/src/components/implementation/comp_x86_64.ld) has generated a two-program-header binary.

- [Open vs. closed workload generators](https://brooker.co.za/blog/2023/05/10/open-closed.html)
- [epoll](https://man7.org/linux/man-pages/man7/epoll.7.html)

  - [Async IO on Linux: select, poll, and epoll](https://jvns.ca/blog/2017/06/03/async-io-on-linux--select--poll--and-epoll/)
  - [Epoll is fundamentally broken part 1/2](https://idea.popcount.org/2017-02-20-epoll-is-fundamentally-broken-12/)
  - [Epoll is fundamentally broken part 2/2](https://idea.popcount.org/2017-03-20-epoll-is-fundamentally-broken-22/)
  - [The method to epoll’s madness](https://copyconstruct.medium.com/the-method-to-epolls-madness-d9d2d6378642)
    
- uioring

  - [Updated pdf documentation](https://kernel.dk/io_uring.pdf)
  - [Ringing in a new asynchronous I/O API](https://lwn.net/Articles/776703/)
  - [Async spawn using io_uring](https://lwn.net/Articles/908268/) (ignore process creation maybe for now, read the following instead?)

- Elf [relocations](https://intezer.com/blog/malware-analysis/executable-and-linkable-format-101-part-3-relocations/)
- x86_64 [code optimizations, exception handling, and calling conventions](https://codemachine.com/articles/x64_deep_dive.html)
- [Embedded Linux status](https://static.sched.com/hosted_files/eoss2023/68/Debating-Linux-in-Aerospace%20-VanderLeest-Brink.pdf)
- [Speculation in Javascript](https://webkit.org/blog/10308/speculation-in-javascriptcore/) that also covers JIT compilation
- [x86 boot process/procedure](https://0xax.gitbooks.io/linux-insides/content/Booting/linux-bootstrap-1.html)
- [Position-independent Code/Executables](https://eli.thegreenplace.net/2011/11/11/position-independent-code-pic-in-shared-libraries-on-x64) including the GOT and PLT
- [Thread-Local Storage](https://chao-tic.github.io/blog/2018/12/25/tls), [other examples](https://maskray.me/blog/2021-02-14-all-about-thread-local-storage), [details](https://akkadia.org/drepper/tls.pdf)
- [Zero-copy I/O for ublk, three different ways](https://lwn.net/Articles/926118/)
- Understanding compiler optimizations, and their interactions with link-time optimization.
- [Deep dive on how to think about performance.](https://docs.google.com/presentation/d/1wOT5kOWkQybVTHzB7uLXpU39ctYzXpOs2xVyD4zuYXY/edit#slide=id.g809d36a3fc4b213_287 ) https://www.infoq.com/presentations/factors-code-performance/
