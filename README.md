# Oxidizing Python: writing extensions in Rust

[Luiz Carlos Irber Júnior](https://github.com/luizirber)

- Department of Population Health and Reproduction, University of California, Davis, USA

[![DOI](https://img.shields.io/badge/DOI-10.7490%2Ff1000research.1115726.1-orange.svg)](https://dx.doi.org/10.7490/f1000research.1115726.1)

Poster presented at [GCCBOSC 2018][1].

## Abstract

Python has a mature ecosystem for extensions using C/C++,
with Cython being part of the standard toolset for scientific programming.
Even so,  C/C++ still have many drawbacks,
ranging from smaller annoyances (like library packaging, versioning and build systems)
to serious one like buffer overflows and undefined behavior leading to security issues.

Rust is a system programming language trying to avoid many of the C/C++ pitfalls,
on top of providing a good development workflow and memory safety guarantees.

This work presents a way to write extensions in Rust and use them in Python,
using sourmash as an example.

## Table of Contents

- [Introduction](01.intro.md)
- [Why Rust?](02.why.md)
- [Current implementation](03.current_impl.md)
- [Rust implementation](04.rust_impl.md)
- [Future work](05.future.md)
- [References](#references)
- Appendices
  - [Submitted abstract](abstract.md)
  - [The final poster](poster/poster.pdf)

## References

- Broder, Andrei Z. 1997. “On the Resemblance and Containment of Documents.” - In Compression and Complexity of Sequences 1997. Proceedings, 21–29. IEEE. http://ieeexplore.ieee.org/abstract/document/666900/.
- Ondov, Brian D., Todd J. Treangen, Páll Melsted, Adam B. Mallonee, Nicholas H. Bergman, Sergey Koren, and Adam M. Phillippy. 2016. “Mash: Fast Genome and Metagenome Distance Estimation Using MinHash.” Genome Biology 17: 132. https://dx.doi.org/10.1186/s13059-016-0997-x
- Bovee, Roderick, and Nick Greenfield. 2018. “Finch: A Tool Adding Dynamic Abundance Filtering to Genomic MinHashing.” The Journal of Open Source Software. doi: https://dx.doi.org/10.21105/joss.00505
- Titus Brown, C., and Luiz Irber. 2016. “sourmash: A Library for MinHash Sketching of DNA.” The Journal of Open Source Software 1 (5). https://dx.doi.org/10.21105/joss.00027


[1]: https://gccbosc2018.sched.com/
