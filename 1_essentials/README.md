Level 1: Essentials of QM Operators in SymPy
============================================

The purpose of this lesson is to introduce physical chemistry students to the
cyberinfrastructure skills necessary to explore quantum mechanical operators
using the SymPy library in Python. 

## Lesson Information

> [!IMPORTANT]
> This version of the lesson is written to provide students with a practical
> introduction to the essential cyberinfrastructure skills necessary to encode,
> manipulate, and apply quantum mechanical operators to solve physical chemistry
> problems using SymPy.

### Lesson Learning Outcomes (LOs)

#### Cyberinfrastructure LOs

By the end of this lesson, students will be able to perform the following
cyberinfrastructure (CI) tasks using the SymPy library in Python:

* Construct the SymPy representation of an operator from its mathematical
definition;
* Encode simple operator expressions in SymPy;
* Apply linear operators to definite SymPy `Equation` objects;
* Use the `.collect()`, `.simplify()`, and `.expand()` methods of the SymPy
`Equation` class to identify operator eigenstates and their associated
eigenvalues;
* Construct and evaluate integrals involving operator eigenstates; and
* Normalize the eigenstates of a Hermitian operator.

#### Content LOs

By the end of this lesson, students will be able to use the SymPy library to
perform the following tasks within the context of the particle-in-a-box model
system:

* Evaluate the action of a quantum mechanical operator on a given state
function;
* Normalize the energy eigenstates of a given Hamiltonian operator; and
* Determine the expected value and variance for the measurement of a classical
observable, both when the system is in an eigenstate and for a given, arbitrary
state function.

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

### Physical Chemistry Prereq's

This lesson is written to introduce the basic properties of quantum mechanical
operators within the context of the 1-dimensional particle-in-a-box, however it
is not meant to serve as the first introduction to the quantum mechanics of
1-dimensional model systems.  Before beginning this lesson, students are
therefore expected to be familiar with the 1-dimensional particle-in-a-box
model system and the general form & properties of the wavefunctions which solve
the corresponding time-independent wave equation.

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

#### Physical Chemistry Resources
* [Libretexts _Physical Chemistry_](https://chem.libretexts.org/Bookshelves/Physical_and_Theoretical_Chemistry_Textbook_Maps/Physical_Chemistry_(LibreTexts))
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



