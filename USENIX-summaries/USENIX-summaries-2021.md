Schumilo, S., Aschermann, C., Abbasi, A., Wörner, S., & Holz, T. (2021). Nyx: Greybox hypervisor fuzzing using fast snapshots and affine types. In 30th {USENIX} Security Symposium ({USENIX} Security 21).

SUMMARY: TODO.

<hr/>

Lee, G., Shim, W., & Lee, B. (2021). Constraint-guided Directed Greybox Fuzzing. In 30th _USENIX_ Security Symposium (_USENIX_ Security 21).

SUMMARY: Directed greybox fuzzing (DGF) uses directedness from crash reproduction and proof-of-concept generation to driving the fuzzing process. However, DGF does not consider the order of target sites in the code or the data dependencies to reach those sites. For example, use-after-free bugs should execute the "free" code before executing the "use" code. In this paper, the authors propose Constraint-guided DGF (CDGF) that resolves these limitations. CDGF automatically generates a sequence of constraints from information sources such as crash dumps (using memory error detectors) and changelogs from patches. CDGF then attempts to reach the target site, while solving the constraints in the specified order. Seeds that satisfy more constraints are given higher priority. CDGF is implemented as a proof-of-concept called CAFL, which based on AFL. CAFL outperforms AFLGO by 2.88x in reproducing 47 real world crashes.

<hr/>

Tychalas, D., Benkraouda, H., & Maniatakos, M. (2021). ICSFuzz: Manipulating I/Os and Repurposing Binary Code to Enable Instrumented Fuzzing in {ICS} Control Applications. In 30th _USENIX_ Security Symposium (_USENIX_ Security 21).

SUMMARY: Industrial control systems (ICS) are responsible for moderating a wide range of industrial sectors and critical infrastructures. Disruption of ICS operation may cause severe complications and even human casualties. In this paper, the authors propose ICSFuzz, a novel approach for security evaluation of PLC control applications through fuzzing. The authors have performed a manual research step to evaluate the different languages of IEC 61131-3, the standard in which many control applications are initially written in. Following this framework, the auhots have developed a fuzzing framework to discover vulnerabilities in programmable logic controller (PLC) applications and their host software, such as Codesys.

<hr/>

Nagy, S., Nguyen-Tuong, A., Hiser, J. D., Davidson, J. W., & Hicks, M. (2021). Breaking Through Binaries: Compiler-quality Instrumentation for Better Binary-only Fuzzing. In 30th _USENIX_ Security Symposium (_USENIX_ Security 21).

SUMMARY: Instrumentation is a valuable tool for coverage-guided fuzzing. However, binary-only instrumentation still lags far behind compiler instrumentation due to performance overhead and semantic limitations. For example, hardware-assisted tracers (e.g., Intel PT) cannot modify programs, and static binary rewriters (e.g., Dyninst) do not scale well to stripped binaries. In this paper, the authors present ZAFL, a platform for applying fuzzing-enhancing program transformations to binary-only targets. ZAFL makes five transformations to binaries prior to fuzzing: 1) single successor-based pruning (do not instrument basic blocks which are the single successor to their parent block); 2) deminator tree instrumentation pruning (only instrument dominator tree leaves, i.e., A dominates B if every path to B contains A); 3) edge instrumentation downgrading (implement CollAFL-style edge instrumentation, which uses fewer instrumentation instructions for blocks with a single predecessor); 4) sub-instruction profiling (break down conditional constraints into nested single-byte comparisons); 5) context-sensitive coverage (implement calling contexts for finer-grained coverage, i.e., each function is instrumented with a random variable that is XOR's to a global value during function entry/exit that is used during edge hashing). On the LAVA-M dataset and real-world targets, ZAFL found up to 96% more crashes than AFL-Dyninst and up to 131% more crashes than AFL-QEMU.

<hr/>
