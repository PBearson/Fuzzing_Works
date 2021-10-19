J. Choi, K. Kim, D. Lee and S. K. Cha, "NtFuzz: Enabling Type-Aware Kernel Fuzzing on Windows with Static Binary Analysis," 2021 IEEE Symposium on Security and Privacy (SP), 2021, pp. 677-693, doi: 10.1109/SP40001.2021.00114.

SUMMARY: A major strategy in kernel fuzzing research is to utilizes types and dependencies of system calls. This is easily achieved in Linux kernel fuzzers, since Linux is open-source. The same is not true for Windows; system calls in Windows are generally unknown and undocumented. In this paper, the authors propose NtFuzz, a type-aware kernel fuzzing framework. The fuzzer operates in two steps. First, it statically analyzes Windows system binaries (e.g., kernel32.dll, ntdll.dll, etc.) that use documented APIs to call system calls. This can bridge the gap between documented and undocumented interfaces and infer the system call argument types. Second, it uses the inferred types to perform type-aware fuzzing on system calls. This work found 11 new kernel bugs in Windows 10, including 4 CVEs.  

<hr/>

Z. Zhang, W. You, G. Tao, Y. Aafer, X. Liu and X. Zhang, "StochFuzz: Sound and Cost-effective Fuzzing of Stripped Binaries by Incremental and Stochastic Rewriting," 2021 IEEE Symposium on Security and Privacy (SP), 2021, pp. 659-676, doi: 10.1109/SP40001.2021.00109.

SUMMARY: TODO.

<hr/>
