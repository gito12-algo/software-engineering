Software Engineering

These notes have been prepared mainly from the following book:

Software Engineering
by
K.K. Aggarwal, Yogesh Singh

Kindly refer above book for more details.

## Software Life Cycle Models
### (1) Waterfall Model

This model is generally used when:

- No change in requirement.
- Deliverables expected at every stage.
- We have carried out a similar project earlier.
### Phases and Deliverables of Waterfall Model
| Phase                    | Purpose                                                                 | Deliverables                                                       |
| ------------------------ | ----------------------------------------------------------------------- | ------------------------------------------------------------------ |
| **System Engineering**   | Defining the scope of the project                                       | User Requirements                                                  |
| **Requirement Analysis** | Understanding the functional and non-functional requirements            | (i) SRS <br> (ii) Acceptance Test Plan <br> (iii) System Test Plan |
| **Design**               | Creating the structure of the modules                                   | (i) HLD <br> (ii) DLD <br> (iii) ITP <br> (iv) UTP                 |
| **Coding**               | Building the software and unit testing                                  | Unit tested code                                                   |
| **Testing**              | Ensuring that requirements are met                                      | Integrated and system tested software                              |
| **Deployment**           | Assembling, Installation, End-user testing and sign-off by the customer | User Manual                                                        |

### Pros and Cons of Waterfall Model

Pros:

- Simple and systematic model.
- Follows a disciplined approach.

Cons:

- Not suitable for accommodating any change.
- Potential delay in identifying the risks.
- It does not scale up well to large projects.
## (2) Prototyping Model

This model is generally used when:

- Complete set of requirements is not available.
- Development with an initial set of requirements is started.
- Feel of the product with initial requirements is expected.

### SRS is finalized after the prototype is ready.

Pros:

- Less technical risk.
- Scope for accommodating new requirements.
- A part of the product is visible at an early stage.

Cons:

- Expensive and time consuming.

### (3) Iterative Enhancement Model

This model delivers an operational quality product at each release, but one that satisfies only a subset of the customer's requirements.

The complete product is divided into releases, and the developer delivers the product release by release.

### (4) Evolutionary Development Model

It resembles the Iterative Enhancement Model. This model differs from the Iterative Enhancement Model in the sense that it does not require a workable product at the end of each cycle.

Here requirements are implemented by category rather than by priority.

Example: GUI in first phase, queries in another.

→ Useful for projects using new technology that is not well understood.

### (5) Spiral Model

This model is generally used when:

- Many risks are expected.
- At each stage of development, there are alternatives and we have to make right decisions.
- Budget is not fixed for the project.

Pros:

- Model for other models.
- Captures potential risks at an early stage.
- Iterative and realistic model.

Cons:

- Requires good expertise in risk management and project planning.
Projected cost is revisited and revised every round during planning.
### (6) RAD (Rapid Application Development) Model

This model is generally used when:

- There are tight deadlines.
- High pressure from customer.
- Quick time to market.
- There are many functionalities.
- Users have to be involved throughout.

→ Each major function is addressed by a separate RAD team.

### (7) Agile Methodology
Development team focuses on construction rather than design and documentation.
Intended to deliver software quickly.

### Software Requirements Analysis and Specifications
- Requirements describe the "what" of a system, not the "how".
- The input is the problem statement prepared by the customer.
### Crucial Process Steps
(i) Requirement Elicitation (Gathering)

Requirements are identified with the help of customers and existing system processes.

Use Case Diagrams, which are a combination of text and pictures, are used to improve the understanding of requirements.

- Actor
- Use-Case
- Relationship between Actor & Use-Case
## Types of Requirements
### (i) Functional Requirements

Describe what the software has to do. They are often called product features.

### (ii) Non-Functional Requirements

Describe how well the software does what it has to do.

### (ii) Requirements Analysis

Requirements are analysed in order to identify inconsistencies, defects, and ambiguities.

Produces a structured requirements specification made of graphical notations.

### (a) Data Flow Diagrams (DFDs)

DFDs show the flow of data through a system.

### (b) Entity Relationship Diagrams

It is a detailed logical representation of the data for an organization.

### (c) Data Dictionaries

Data dictionaries are repositories to store information about all data items defined in DFDs.

### (iii) Requirements Documentation

This is the end product of requirement elicitation and analysis. The document is known as Software Requirements Specification (SRS).

## SRS should address the following:
- (a) Functionality

What the software is supposed to do?

- (b) External Interface

How does the software interact with:

- People
- The system's hardware
- Other hardware
- Other software?

## Software Requirements Specification (SRS)
### (c) Performance

What is the speed, availability, response time, recovery time, etc. of various software functions?

### (d) Design Constraints

Constraints imposed on an implementation such as:

Implementation language
Operating environment
etc.
### Characteristics of a Good SRS
- Correct
- Unambiguous
- Complete
- Consistent
- Verifiable
- Modifiable
- Traceable
## Notes
- Acceptance Test Plan and System Test Plan are also generated in the requirements analysis phase.
- SRS should not describe any design or implementation details.
## Software Design
### Design

In this phase, the designer plans how a software system should be developed in order to make it:

- Functional
- Reliable
- Understandable
- Modifiable
- Maintainable

The purpose of the design phase is to produce a solution to a problem given in the SRS document.

### Modularity

Desirable properties of a modular system include:

- Each module is a well-defined subsystem that is potentially useful in other applications.
- Modules can be separately compiled and stored in a library.
### Module Coupling

Coupling is the measure of the degree of interdependence between modules.

Loosely Coupled Systems: Made up of modules that are relatively independent.
Highly Coupled Systems: Share a great deal of dependence between modules.
Uncoupled Modules: Have no interconnections at all.
## Important Point

A good design will have low coupling. Therefore, interfaces should be carefully specified in order to keep the value of coupling low.

## Types of Coupling

### (i) Data Coupling:
Module A and B communicate by only passing of data.

### (ii) Stamp Coupling:
Module A and B communicate by passing complete data structure.

### (iii) Control Coupling:
Module A and B communicate by passing of control information, i.e. flags.

### (iv) External Coupling:
A module has a dependency to other module, external to the software being developed.

### (v) Common Coupling:
Module A and B have shared data.

### (vi) Content Coupling:
When control is passed from one module to the middle of another.

### Coupling Ranking:

- Data Coupling — Best (Low)
- Stamp Coupling
- Control Coupling
- External Coupling
- Common Coupling
- Content Coupling — Worst (High)
### Module Cohesion

Cohesion is a measure of the degree to which the elements of a module are functionally related.

An important design objective is to maximize the module cohesion and minimize the module coupling.

## Types of Cohesion

Given a procedure that carries out operations X and Y, we can describe various forms of cohesion between X and Y:

### (i) Functional Cohesion

X and Y are part of a single functional task.

### (ii) Sequential Cohesion

X outputs some data which forms the input to Y.

### (iii) Communicational Cohesion

X and Y both operate on the same input data or contribute towards the same output data.

### (iv) Procedural Cohesion

It occurs in modules whose instructions, although accomplishing different tasks, have been combined because there is a specific order in which the tasks are to be completed.

### (v) Temporal Cohesion
- X and Y both must perform around the same time
### (vi) Logical Cohesion
- X and Y perform logically similar operations
### (vii) Coincidental Cohesion
- X and Y have no conceptual relationship other than shared code.
## Cohesion Ranking(Best to Worst)
- Functional Cohesion(Best/High)
- Sequential Cohesion 
- Communicational Cohesion
- Procedural Cohesion
- Temporal Cohesion
- Logical Cohesion
- Concidental Cohesion(Worst/Low)

## Structure Chart
The Structure Chart is ojne of the most commonly used methods for system design .It partitions a system into block boxes. A block box means that the functionality is known for the user without the knowledge of the internal design.

The block boxes are arranged in a hierarchical format, as shown in the digarm below.

[Main   Module]
[Module 1] [Module 2] [Module 3]

## Software Project Planning
Software planning begins before technical work starts, continues as the software evolves, and culminates only when the software is retired.

The project planning must incorporate the following major issues:
- Size and Cost Estimation
- Scheduling
- Project Monitoring
- Resource Requirement
- Risk Management
## Size Estimation
### (1) Lines of Code (LOC)
A line of code is any line of program text that is not a comment or blank line, regardless of the number of statements or fragments of statements on the line. This specifically includes all lines containing program headers, declarations, and executable and non-executable statements.
### (2) Function Count
It measures functionality from the user's point of view, i.e., on the basis of what the user requests and receives in return from the system.
It is independent of the language and tools used for implementation.
```
Formula:
FP = UFP × CAF
Where:
FP = Function Point
UFP = Unadjusted Function Point
CAF = Complexity Adjustment Factor
```
## Cost Estimation
Constructive Cost Model (COCOMO)
```
Formulas:
E = a(KLOC)^b
D = c(E)^d
Where:
E = Effort (Person-Months)
D = Development Time (Months)
```
Additional formulas:
```
Average Staff Size = E / D (Persons)
```
```
Productivity = KLOC / E (KLOC per Person-Month)
```
## Risk Estimation
Question: Consider a project that has a 0.5% probability of an undetected fault that would cost the company Rs. 1,00,000 in fines. What would be the risk exposure?
Solution:
Risk Exposure = 1,00,000 × (0.5 / 100)
= Rs. 500
Availability Example

Question: In a software system, Mean Time To Failure (MTTF) is equal to Mean Time To Repair (MTTR). Find the availability.
Formula:
Availability = MTTF / (MTTF + MTTR) × 100%
Since MTTF = MTTR,
Availability = x / (x + x) × 100%
= 50%

Error Seeding Example
Question: 10 errors were seeded into the software. During testing, 4 seeded errors and 100 non-seeded errors were detected. Estimate the number of undetected errors.
Solution:
Total estimated errors = 100 × (10 / 4) = 250
Undetected errors = 250 − 100 = 150
```
Important Formula
MTBF (Mean Time Between Failures)
MTBF = MTTF + MTTR
Availability = MTTF / MTBF = MTTF / (MTTF + MTTR)
```
## Software testing

Testing is the process of executing a program with the intent of finding errors.
In the software life cycle the earlier the errors are discovered and removed, the lower is the cost of their removal.
Complete or exhaustive testing is just not possible.

### Verification and Validation:
(i) Verification:-
Checking the software with respect to specifications.

### (ii) Validation:-
- Checking the software with respect to customer’s expectations.
### Acceptance Testing:-
- Used when the software is developed for a specific customer.
- Testing is conducted by the customer to validate all requirements.
### Alpha and Beta Testing:-

- Used when the software is developed as a product for anonymous customers.
- The alpha test are conducted at the developer’s site by a customer.
- The beta test are conducted by the customer at their site.

