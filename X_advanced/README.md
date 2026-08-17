Level 3: Advanced Exploration of QM Operators in SymPy
======================================================

The purpose of this lesson is to introduce physical chemistry students to the
cyberinfrastructure skills necessary to explore linear, Hermitian operators
in quantum mechanics using the SymPy library in Python. 

## Lesson Information

> [!IMPORTANT]
> This version of the lesson provides a detailed and mathematical introduction to
> the theory of operators and their properties, including the properties of the
> eigenstates of linear Hermitian operators, however does not assume prior
> familiarity with Dirac notation or the rigorous formulation of quantum
> mechanics in terms of the functional analysis of Hilbert spaces.

### Lesson Learning Outcomes (LOs)

#### Cyberinfrastructure LOs

By the end of this lesson, students will be able to perform the following
cyberinfrastructure (CI) tasks using the SymPy library in Python:

* Construct the SymPy representation of an operator from its mathematical
definition;
* Encode arbitrary operator expressions in SymPy;
* Apply linear and nonlinear operators to definite SymPy `Equation` and
arbitrary SymPy `Function` objects;
* Construct the closed-form representation of a compound operator expression;
* Use the `.collect()`, `.simplify()`, and `.expand()` methods of the SymPy
`Equation` class to identify operator eigenstates and their associated
eigenvalues;
* Construct and evaluate integrals involving operator eigenstates; and
* Normalize the eigenstates of a Hermitian operator.

#### Mathematical LOs

By the end of this lesson, students will be able to use SymPy to perform the
following mathematical tasks:

1. Properties and action of general operators
    * Define and evaluate operator linearity;
    * Define and evaluate operator products and powers of operators;
    * Define and evaluate operator commutativity;
    * Construct the closed-form representation of a compound operator expression;
2. Operator eigenproblems
    * Evaluate whether a given function is an eigenstate of a particular operator
    and to determine its eigenvalue;
    * Define eigenstate degeneracy and apply this property to construct other
    degenerate eigenstates;
    * Determine whether two operators share a set of mutual eigenstates based
    on their commutativity; 
    * Define the realness of the eigenvalues of a Hermitian operator;
    * Normalize the eigenstates of a Hermitian operator

#### Physical Chemistry LOs

By the end of this lesson, students will be able to apply the SymPy and
mathematical skills above to perform the following physical chemistry tasks:

* Evaluate the action of a quantum mechanical operator on a given state
function;
* Normalize the energy eigenstates of a given Hamiltonian operator;
* Determine the average measured value of a classical observable for a quantum
mechanical system described by particular state function by evaluating the
corresponding operator expectation value;
* Determine the variance in the average measured value of a classical observable
for a quantum mechanical system described by a particular state function;
* Evaluate whether the simultaneous uncertainty in the position and momentum of
a particle in a 1-dimensional box obeys the Heisenberg principle;
* Derive the Heisenberg uncertainty relationship for the particle in a
1-dimensional box from the expectation value of their commutator

## Lesson Prerequisites

### Cyberinfrastructure Prereq's

Before beginning this lesson, students are expected to have the following skills
and/or completed the following modules/lessons available on the ACT-CMS Portal:

* Basic skills in Python programming and syntax
    - [Introduction to Programming for Molecular Scientists](https://act-cms.molssi.org/portal/lessons/foundational-intro-python/)
* Symbolic mathematics in Python with SymPy
    - [Foundations of Symbolic Mathematics in Python](https://act-cms.molssi.org/portal/lessons/foundational-symbolic-math/)
    - TODO: Link specific algebra and calculus lessons

### Mathematical Prereq's

Before beginning this lesson, students are expected to be familiar with the
following mathematical topics:

* Calculus of a single variable (Calculus 1 & 2)
* Partial derivatives & multiple integrals in Cartesian coordinates (Calculus 3)
* Some familiarity with linear algebra and/or discrete mathematics
    > [!IMPORTANT] _Author Recommendation_
    > While no prior experience with linear algebra or discrete mathematics is
    > explicitly necessary for students to access the content of this lesson, this is
    > recommended as a "maturity prereq" to ensure students will not balk at the
    > conceptual complexity of the mathematical treatment of operators in this
    > lesson.

### Physical Chemistry Prereq's

This lesson does not assume a prior level of student background familiarity
with physical chemistry concepts, as the applications of operator theory to
quantum mechanics are introduced in this lesson as a natural extension of
operators themselves.  Depending on their students' level of comfort with
pure mathematics, however, the adopting instructor should determine the most
appropriate timing for this lesson to ensure its conceptual rigor is proximal.

For all but the most thoroughly mathematically prepared students, the most
appropriate timing of this version of the lesson is immediately following the
discussion of the particle in a 1-dimensional infinite square well, and before
discussing the extension of this model system to the multidimensional case.

### Resources

Additional resources to support students completing this lesson include

#### Cyberinfrastructure Resources
* [MolSSI Workshop: Python Scripting for Computational Molecular Sciences](https://education.molssi.org/python_scripting_cms/)
* [MolSSI CMS Python Workshop: Introduction](https://education.molssi.org/python_scripting_cms/01-introduction/index.html)
* [Algebra with SymPy Documentation](https://gutow.github.io/Algebra_with_Sympy/algebra_with_sympy.html)
* [Demonstrations of `algebra_with_sympy` functionality with the `Equation` class](https://gutow.github.io/Algebra_with_Sympy/Demonstration%20of%20equation%20class.html)

#### Mathematical Resources
* [OpenStax Calculus Volume 1](https://openstax.org/details/books/calculus-volume-1)
* [OpenStax Calculus Volume 2](https://openstax.org/details/books/calculus-volume-2)
* [OpenStax Calculus Volume 3](https://openstax.org/details/books/calculus-volume-3)
* [Schilling, Nachtergaele, & Lankham's _Linear Algebra_](https://math.libretexts.org/Bookshelves/Linear_Algebra/Book%3A_Linear_Algebra_(Schilling_Nachtergaele_and_Lankham))
* [Levitus' _Mathematical Methods in Chemistry_](https://chem.libretexts.org/Bookshelves/Physical_and_Theoretical_Chemistry_Textbook_Maps/Mathematical_Methods_in_Chemistry_(Levitus))

#### Physical Chemistry Resources
* [McQuarrie & Simon's _Physical Chemistry: A Molecular Approach_](https://chem.libretexts.org/Bookshelves/Physical_and_Theoretical_Chemistry_Textbook_Maps/Physical_Chemistry_(LibreTexts))
* [OpenStax University Physics Volume 3](https://openstax.org/details/books/university-physics-volume-3)

### References

Portions of this lesson were inspired by or adapted from:
* D. A. McQuarrie and J. D. Simon, _Physical Chemistry: A Molecular Approach_, 2nd Ed. University
Science Books, 1997.
* D. A. McQuarrie, _Quantum Chemistry_, 2nd Ed. University Science Books, 2008.
* R. Shankar, _Principles of Quantum Mechanics_, 2nd Ed. Plenum, 1994.

## Lesson Versions & Intended Modalities

Three versions of this lesson are provided, each with a different intended
modality of instruction and associated implementation strategies.

| Modality     | Pedagogy                | Role of Instructor                                                       | Lesson Version            |
|--------------|-------------------------|---------------------------------------------------------------------------|--------------------------|
| Asynchronous | Guided Inquiry Learning | N/A (independent student learning)                                       | `student-async.ipynb`     |
| Synchronous  | Guided Inquiry Learning | Facilitate student process, answer questions, ensure nobody falls behind | `student-sync-gil.ipynb`  |
| Synchronous  | LiveCoding              | Demonstrate & narrate process, control pacing, etc.                      | `student-sync-live.ipynb` |

Also provided to support adopting instructors are
- `instructor-key.ipynb`: Instructor "key" notebook with completed code cells and full instructor commentary in Markdown cells
- `instructor-notes.ipynb`: Author notes for adopting instructors, including implementation strategies, common issues & workarounds, piloting notes, etc.

See the `instructor-notes.ipynb` For more information about implementation
strategies from the lesson author.



