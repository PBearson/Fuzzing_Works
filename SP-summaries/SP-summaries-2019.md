S. Nagy and M. Hicks, "Full-Speed Fuzzing: Reducing Fuzzing Overhead through Coverage-Guided Tracing," 2019 IEEE Symposium on Security and Privacy (SP), 2019, pp. 787-802, doi: 10.1109/SP.2019.00069.

SUMMARY: Coverage-guided fuzz testing consists of 1) test case generation; 2) code coverage tracing; 3) crash triage. In practice, code coverage tracing incurs a significant portion of the entire fuzzing overhead. Unfortunately, the majority of test cases do not increase fuzz testing, especially over time, and thus the effort required to trace through the code coverage is often highly wasteful. In this paper, the authors propose UnTracer, a strategy for coverage-guided tracing that reduces the overhead of coverage-guided fuzzers. Using static binary instrumentation, the target binary is transformed so that it self-reports when a test case increases coverage. Following the self-report, the binary is traced with the interesting test case in order to determine the code coverage. Since code coverage tracing only occurs for newly discovered code coverage, the overhead is massively improved from previous efforts such as AFL-Clang (36%), AFL-QEMU (612%), and AFL-Dyninst (518%), and UnTracer approaches an overhead of 0% after 24 hours of fuzzing. 

<hr/>

W. You et al., "ProFuzzer: On-the-fly Input Type Probing for Better Zero-Day Vulnerability Discovery," 2019 IEEE Symposium on Security and Privacy (SP), 2019, pp. 769-786, doi: 10.1109/SP.2019.00057.

SUMMARY: Generation-based fuzzing relies on a grammar describing input formats to produce legimite test cases. On the one hand, this reduces the search space for crafting inputs. On the other hand, the grammar must be supplied beforehand or executed from input traces, and vulnerable inputs may not follow the grammar if an implementation ignores certain fields. Meanwhile, mutation-based fuzzing requires seed inputs, requiring no grammar; however, mutation is typically random. In this paper, this authors propose ProFuzzer, which uses a lightweight fuzzing procedure called probing that guides evolution of seed inputs. Specifically, the fuzzer executes in two stages: 1) bytes are sequentially changed one at a time to test the execution path against different values, and data fields are recovered; 2) the fuzzer mutates each field to increase coverage and exploit bad field values. The authors define six application-agnostic field types: 1) assertion (magic byte); 2) raw data (does not affect program execution); 3) enumeration (small set of valid values); 4) loop count (number of times a loop structure executes); 5) offset (locate in the input where the program can access data); 6) size (the size of data to read). ProFuzzer found 42 zero-days among 10 programs, generating 30 CVEs.

<hr/>

D. She, K. Pei, D. Epstein, J. Yang, B. Ray and S. Jana, "NEUZZ: Efficient Fuzzing with Neural Program Smoothing," 2019 IEEE Symposium on Security and Privacy (SP), 2019, pp. 803-817, doi: 10.1109/SP.2019.00052.

TODO.

<hr/>
