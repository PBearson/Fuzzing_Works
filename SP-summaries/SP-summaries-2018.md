W. Xu, H. Moon, S. Kashyap, P. Tseng and T. Kim, "Fuzzing File Systems via Two-Dimensional Input Space Exploration," 2019 IEEE Symposium on Security and Privacy (SP), 2019, pp. 818-834, doi: 10.1109/SP.2019.00035.

SUMMARY: File systems are one of the most basic services of an OS. Most conventional file systems run in the kernel, and hence can lead to devastating errors when bugs are found. However, file systems are large and complex, and coventional stress-testing frameworks either do not scale well (i.e., model checking) or only consider file system regression. Fuzz testing of file systems is gaining traction, but file systems present unique challenges that differ from typical binary fuzzing. Namely, fuzzing a file system consists of mutating a mounted disk image and a program that makes file operations on that image. In this paper, the authors propose Janus, an evolutionary feedback-driven file system fuzzer. When mutating a seed disk image, Janus only mutates the metadata blocks of the image, which reduces the search space of the input. When mutating the file ops program, Janus uses an image-directed syscall fuzzing technique, i.e., it stores generated system calls on file objects and tracks their runtime status after each system call is executed. Moreover, Janus utilizes a libOS executor, i.e., Linux Kernel Library, as opposed to a VM for mounting an image and executing the program; this improves performance and enhances bug reproducibility. Janus found 90 bugs, including 32 CVEs, across 8 popular Linux file systems.

<hr/>

H. Peng, Y. Shoshitaishvili and M. Payer, "T-Fuzz: Fuzzing by Program Transformation," 2018 IEEE Symposium on Security and Privacy (SP), 2018, pp. 697-710, doi: 10.1109/SP.2018.00056.

SUMMARY: TODO

<hr/>

W. You et al., "ProFuzzer: On-the-fly Input Type Probing for Better Zero-Day Vulnerability Discovery," 2019 IEEE Symposium on Security and Privacy (SP), 2019, pp. 769-786, doi: 10.1109/SP.2019.00057.

SUMMARY: TODO

<hr/>

S. Gan et al., "CollAFL: Path Sensitive Fuzzing," 2018 IEEE Symposium on Security and Privacy (SP), 2018, pp. 679-696, doi: 10.1109/SP.2018.00040.

SUMMARY: TODO

<hr/>
