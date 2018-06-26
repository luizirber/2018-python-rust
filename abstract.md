# Oxidizing Python: writing extensions in Rust

Python has a mature ecosystem for extensions using C/C++,
with Cython being part of the standard toolset for scientific programming.
Even so,  C/C++ still have many drawbacks,
ranging from smaller annoyances (like library packaging, versioning and build systems)
to serious one like buffer overflows and undefined behavior leading to security issues.

Rust is a system programming language trying to avoid many of the C/C++ pitfalls,
on top of providing a good development workflow and memory safety guarantees.

This work presents a way to write extensions in Rust and use them in Python,
using sourmash as an example.
