J. Wang, B. Chen, L. Wei and Y. Liu, "Skyfire: Data-Driven Seed Generation for Fuzzing," 2017 IEEE Symposium on Security and Privacy (SP), 2017, pp. 579-594, doi: 10.1109/SP.2017.23.

SUMMARY: Programs that accept structured inputs normally operate in 3 stages: 1) parse the syntax of the input; 2) check the syntax of the input; 3) execute the application. Deep bugs are often hidden in the final step. However, mutation-based fuzzing typically fails at step 1, while generation-based fuzzing may fail at step 2. In this paper, the authors propose Skyfire, a data-driven seed generation approach. Skyfire takes a corpus and a grammar as input and generates a probabilistic context-sensitive grammar (PCSG), which specifies syntax features and semantic rules about the inputs. From this, the fuzzer generates seed inputs according to producting rules in the PCSG, with a priority of low-probability production rules over high-priority production rules for producing uncommon inputs.

<hr/>
