Peng Chen, Jianzhong Liu, and Hao Chen. 2019. Matryoshka: Fuzzing Deeply Nested Branches. In Proceedings of the 2019 ACM SIGSAC Conference on Computer and Communications Security (CCS '19). Association for Computing Machinery, New York, NY, USA, 499–513.

SUMMARY: Greybox fuzzers have trouble solving path constraints with deeply nested conditional statements, such as image and video decoders, network packet analyzers, checksum tools, etc. AFL does not track program state to guide input mutations, so code coverage suffers. Other fuzzers, such as Angora and VUzzer, use dynamic taint tracking to determine whcih input bytes flow into the conditional statement guarding a target branch; however, these fuzzers cannot reliably solve path constraints that involve nested conditional statements. In this paper, the authors propose Matryoshka, a tool for fuzzing deeply nested branches. Matryoshka starts by identifying all control flow dependencies among a conditional statement, i.e., conditional statements before a target statement that may make that target statement unreachable. Then it identifies all taint flow dependencies among a conditional statement, i.e., the subset of control flow dependencies which may change their branch choice as the target conditional statement is mutated. To solve these constraints and reach the target branch, Matryoshka proposes three strategies.

<hr/>

Mingi Cho, Seoyoung Kim, and Taekyoung Kwon. 2019. Intriguer: Field-Level Constraint Solving for Hybrid Fuzzing. In Proceedings of the 2019 ACM SIGSAC Conference on Computer and Communications Security (CCS '19). Association for Computing Machinery, New York, NY, USA, 515–530.

TODO.

<hr/>
