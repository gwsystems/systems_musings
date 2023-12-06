# Scheduled Discussions

We'll discuss the first time on this list in the next meeting. 
Make sure to scan the articles, and come with questions.

- Virtualization hardware details in [Extended Page-Tables (EPT)](https://revers.engineering/mmu-ept-technical-details/) and implementation [details](https://revers.engineering/mmu-virtualization-impl-p1/)

Add more links.

# List of Potential Topics for Musing

- tracing tools [overview](https://thume.ca/2023/12/02/tracing-methods/)
- ELF [core dump](https://lief-project.github.io/doc/latest/tutorials/12_elf_coredump.html) format and parsing.
- Survey of [IPC mechanisms](https://beej.us/guide/bgipc/html/) in UNIX
- BPF-defined [network devices](https://lwn.net/Articles/949960/)
- [Deferred scheduling](https://lwn.net/Articles/948870/) of threads holding user-level spinlocks...we want something like this!
- A light read about the [software-defined vehicle](https://spectrum.ieee.org/software-eating-car), but with many relevant research implications.
- How are virtual drivers implemented using virtio? Interesting series of articles on virtio:

    - virtio [devices](https://www.redhat.com/en/blog/virtio-devices-and-drivers-overview-headjack-and-phone)
    - [queues](https://www.redhat.com/en/blog/virtqueues-and-virtio-ring-how-data-travels)
    - [optimizations](https://www.redhat.com/en/blog/packed-virtqueue-how-reduce-overhead-virtio)

- Linux kernel [preemption](https://lwn.net/Articles/831678/) [mode](https://lwn.net/Articles/944686/) [information](https://lwn.net/Articles/945422/) (and a current push to [unify](https://lore.kernel.org/lkml/20231107215742.363031-1-ankur.a.arora@oracle.com/))
- [Maple Trees](https://lwn.net/Articles/845507/) to track virtual address ranges including some background on how these ranges are tracked.
- [GraalOS](https://blogs.oracle.com/java/post/introducing-graalos) - a high performance serverless Java-based application deployment technology by Oracle. More [here](https://blogs.oracle.com/cloud-infrastructure/post/ultrafast-serverless-functions-powered-by-graalos). See [graal.cloud/graalos/](https://graal.cloud/graalos/).
- Similarly, KIM VMM [wiser](https://github.com/flouthoc/wiser)
- Yet antoher attempt to add [security to BPF](https://lwn.net/Articles/947173/) -- fundamental issues here around how to add security to a large surface API
- Progress on removing the [GIL in Python](https://lwn.net/Articles/947138/) -- the interesting part here is the [concurrency/synchronization](https://peps.python.org/pep-0703/#reference-counting)
- Adaptive, user-level spinlocks and [restartable sequences](https://lwn.net/Articles/944895/) for user-kernel communication (we used to have these in Composite!, and there is potential research here)

    - More on [ras here](https://lwn.net/Articles/946870/) and [here](https://lwn.net/Articles/697979/)
      
- Updates and complexities in [Linux kernel preemption](https://lwn.net/Articles/944686/) -- or why there is cooperative yielding in the kernel
- [pidfd](https://lwn.net/Articles/794707/) and [race-free process creation](https://lwn.net/Articles/943022/)
- [io_ring vulnerability and VM attestation](https://lwn.net/Articles/943239/)
- Performing customizable static analysis on system code with [semgrep](https://semgrep.dev/blog/2021/semgrep-a-static-analysis-journey/) (previously [Coccinelle](https://lwn.net/Articles/698724/), which has long been used in the Linux kernel).
- Making a [micro-Linux distribution](https://popovicu.com/posts/making-a-micro-linux-distro/) (similar to [Linux from Scratch](https://www.linuxfromscratch.org/))
- Latencies and debugging latencies in the [linux scheduler](https://bristot.me/linux-scheduling-latency-debug-and-analysis/)
- Understanding [bugs in embedded systems](https://dl.acm.org/doi/10.1145/3597926.3598140)
- [Heuristics for software-interrupt processing](https://lwn.net/Articles/925540/)
- [An EEVDF CPU scheduler for Linux](https://lwn.net/Articles/925371/)
- [Zephyr: a modular OS for resource-constrained devices](https://lwn.net/Articles/925924/)
- Architecture of modern LLM infrastructures that require singificant context (for example, [this](https://about.sourcegraph.com/blog/cody-is-cheating), and [this](https://about.sourcegraph.com/whitepaper/cody-context-architecture.pdf))
- Hiding memory access latency on [in-order architectures](https://johnnysswlab.com/hiding-memory-latency-with-in-order-cpu-cores-or-how-compilers-optimize-your-code/)
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
- Can we find an article on KPI (kernel page-table isolation)?
- Risc-V bootup procedures vs. x86
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

- KVM [hello world](https://github.com/dpw/kvm-hello-world) (I haven't read the article but maybe we can combine these two into one?)
- KVM simple [host](https://github.com/sysprog21/kvm-host) 
- [11/7/23] [Core scheduling to avoid SMT/hyperthreading sidechannels](https://lwn.net/Articles/780703/), current [status and code](https://lwn.net/Articles/861251/) and [potential uses](https://lwn.net/Articles/799454/)
- [10/31/2023] Detailed [architectural summary of Intel's Sandy Bridge](https://chipsandcheese.com/2023/08/04/sandy-bridge-setting-intels-modern-foundation/)
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
