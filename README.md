# SMT-based Static Type Inference for Python 3
### Bachelor Thesis

Author: Mostafa Abdullah

Supervisors: 
- Dr. Caterina Urban
- Marco Eilers
- Prof. Peter Müller

### Abstract
Static types are useful in many programming languages. They can contribute to the type safety of the language by catching type errors in an early stage and contribute to the documentation of the programs written in it. Python is a dynamically typed language in which types are assigned to variables at runtime. Python is very popular nowadays and is used in different fields especially data science. This justifies the increasing attention towards performing static analysis for Python programs.
The aim of this thesis is to provide a static type inference for Python 3. We make use of SMT solving to perform the type inference by encoding the type system of the language in an SMT problem, collecting constraints from the given program and using Z3 SMT solver to provide a types model. We do whole program type inference such that the types model given by the SMT solution includes the types for all the variables that appear in the whole program.
We present a static type system for Python which is essential for defining the static type inference rules. We provide an encoding for this type system in the SMT solver Z3 and present a complete implementation of the type inference algorithm based on this encoding. The type inference currently supports many complicated features in Python like multiple inheritance and operator overloading. The proposed type inference is sound, but there remains some Python features which we do not support. The type inference proved to perform well on several programs and an open source project which uses different Python features.

Based on [TUM thesis latex template](https://github.com/fwalch/tum-thesis-latex)
