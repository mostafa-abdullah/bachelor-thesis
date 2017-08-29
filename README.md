# SMT-based Static Type Inference for Python 3
### Bachelor Thesis

Author: Mostafa Abdullah

Supervisors: 
- Dr. Caterina Urban
- Marco Eilers
- Prof. Peter Müller

### Abstract
Static types are useful in many programming languages. They can contribute to the
type safety of the language, its expressiveness and the documentation of the programs
written in it. Python is a dynamically typed language in which types are assigned to
variables at runtime.
The aim of this thesis is to provide a static type inference for Python 3. We make
use of SMT solving to provide a types model which is sound in terms of static type
checking. We do whole program type inference such that the types model given by the
SMT solution includes the types for all the variables that appear in the whole program.
We present a static type system for Python which is essential for defining the static
type inference rules. We provide an encoding for this type system in the SMT solver Z3
and present a complete implementation of the type inference algorithm based on this
encoding. The type inference currently supports many complicated features in Python
like multiple inheritance and operator overloading. The proposed type inference is
sound, but there remains many Python features which we do not support. However,
the type inference proved to perform well on several open source projects which use
different Python features.

Based on [TUM thesis latex template](https://github.com/fwalch/tum-thesis-latex)
