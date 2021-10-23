Lee, G., Shim, W., & Lee, B. (2021). Constraint-guided Directed Greybox Fuzzing. In 30th _USENIX_ Security Symposium (_USENIX_ Security 21).

SUMMARY: Directed greybox fuzzing (DGF) uses directedness from crash reproduction and proof-of-concept generation to driving the fuzzing process. However, DGF does not consider the order of target sites in the code or the data dependencies to reach those sites. For example, use-after-free bugs should execute the "free" code before executing the "use" code. In this paper, the authors propose Constraint-guided DGF (CDGF) that resolves these limitations. CDGF automatically generates a sequence of constraints from information sources such as crash dumps (using memory error detectors) and changelogs from patches. CDGF then attempts to reach the target site, while solving the constraints in the specified order. Seeds that satisfy more constraints are given higher priority. CDGF is implemented as a proof-of-concept called CAFL, which based on AFL. CAFL outperforms AFLGO by 2.88x in reproducing 47 real world crashes.

<hr/>

Tychalas, D., Benkraouda, H., & Maniatakos, M. (2021). ICSFuzz: Manipulating I/Os and Repurposing Binary Code to Enable Instrumented Fuzzing in {ICS} Control Applications. In 30th _USENIX_ Security Symposium (_USENIX_ Security 21).

TODO.

<hr/>

Nagy, S., Nguyen-Tuong, A., Hiser, J. D., Davidson, J. W., & Hicks, M. (2021). Breaking Through Binaries: Compiler-quality Instrumentation for Better Binary-only Fuzzing. In 30th _USENIX_ Security Symposium (_USENIX_ Security 21).

TODO.

<hr/>
