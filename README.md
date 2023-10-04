# Verifier-based-on-relational-Hoare-logic
Implement a verifier based on relational Hoare logic

We are trying to implement a verifier based on relational Hoare logic, a proof system for verifying relational properties of two programs or two runs of the same program. Relational properties include program equivalence, non-interference, information flow, and relative cost. We explain the problem by introducing the syntax and semantics of a simple imperative language and its relational extension, and presenting the proof rules of relational Hoare logic.

The problem we are addressing is currently done by using various techniques such as product programs, probabilistic couplings, and adversaries. These techniques have different strengths and limitations, depending on the type of relational property and the complexity of the programs. For instance, product programs are effective for proving equivalence and non-interference, but not for relative cost or probabilistic properties. Probabilistic couplings are useful for reasoning about probabilistic programs, but not for adversarial computations. Adversaries are powerful for capturing security properties, but require sophisticated reasoning about cryptography.

Some previous works on relational Hoare logic and its applications are:

Benton, N. (2004). Relational semantics for effect-based program transformations. In Proceedings of the 9th ACM SIGPLAN International Conference on Functional Programming (ICFP '04), pp. 93-1041
Barthe, G., D’Argenio, P.R., and Rezk, T. (2004). Secure information flow by self-composition. In Proceedings of the 17th IEEE Computer Security Foundations Workshop (CSFW '04), pp. 100-1142
Barthe, G., Grégoire, B., and Zanella-Béguelin, S. (2011). Formal certification of code-based cryptographic proofs. In Proceedings of the 36th ACM SIGPLAN-SIGACT Symposium on Principles of Programming Languages (POPL '09), pp. 90-1013
What is new in our project is that we aim to implement a verifier that can handle different types of relational properties and programs in a unified framework, using relational Hoare logic as the underlying proof system. We think we will be successful because we have a solid theoretical foundation and a clear design for our verifier. We plan to use an existing verification tool such as Why3 or F* as a backend for our verifier, and leverage their support for automated theorem provers and interactive proof assistants.

There are many security applications of our project, such as verifying confidentiality, integrity, authenticity, and availability of programs that manipulate sensitive data or communicate over insecure channels. For example, we can use our verifier to prove that a program does not leak any information about its secret inputs to an adversary, or that two versions of a program are functionally equivalent and have the same cost.

This project is important because it addresses a fundamental challenge in software verification: how to reason about the relationship between two programs or two runs of the same program. This challenge arises in many scenarios such as program optimization, refactoring, transformation, synthesis, testing, debugging, and comparison. By providing a verifier based on relational Hoare logic, we hope to make it easier and more reliable for programmers and analysts to verify relational properties of their programs.

The main risks of this project are:

The complexity and expressiveness of relational Hoare logic may make it difficult to implement an efficient and user-friendly verifier.
The choice of verification tool as a backend may limit the applicability or scalability of our verifier to certain types of programs or properties.
The soundness and completeness of our verifier may depend on the assumptions and limitations of the underlying proof system and theorem provers.
We plan to mitigate these risks by:

Using modular and incremental design principles to implement our verifier.
Comparing different verification tools and choosing the most suitable one for our purpose.
Providing rigorous proofs and tests for the correctness and performance of our verifier.
