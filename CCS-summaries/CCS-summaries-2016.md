Marcel Böhme, Van-Thuan Pham, and Abhik Roychoudhury. 2016. Coverage-based Greybox Fuzzing as Markov Chain. In Proceedings of the 2016 ACM SIGSAC Conference on Computer and Communications Security (CCS '16). Association for Computing Machinery, New York, NY, USA, 1032–1043.

SUMMARY: Coverage-based greybox fuzzing (CGF) requires no program analysis, but most tests tend to exercise the same few "high-frequency" paths. A CGF uses a power schedule to determine how often a chosen seed will be fuzzed (its "energy"), while it uses a search strategy to determine the order in which seeds are chosen. For example, AFL assigns consant energy to inputs and selects inputs in the order in which they are discovered. In this paper, the authors propose AFLFast, a fork of AFL that modifies its power schedules and search strategies. AFLFast implements a power schedule that assigns low energy to seeds executing high-energy paths and high energy to seeds executing low-energy paths (i.e., the inverse of the density of the stationary distribution, as modeled by a Markov Model). AFLFast modifies the search strategy by prioritizing seeds with lower-frequency paths and that have been chosen less often. AFLFast discovered 9 new CVEs, 3 of which could not be found by AFL within 24 hours.

<hr/>

Juraj Somorovsky. 2016. Systematic Fuzzing and Testing of TLS Libraries. In Proceedings of the 2016 ACM SIGSAC Conference on Computer and Communications Security (CCS '16). Association for Computing Machinery, New York, NY, USA, 1492–1504.

TODO.

<hr/>
