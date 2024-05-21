# Software Reengineering Project: ckjm
## Project Overview
This project involves the reengineering of the ckjm (Chidamber and Kemerer Java Metrics) application. The ckjm tool computes CK metrics for Java-based applications by processing Java bytecode. The goal of this project is to improve the design and maintainability of the ckjm application through a series of refactorings.

## Technology Stack
- Programming Language: Java
- Application: ckjm (https://www.spinellis.gr/sw/ckjm/)
## Deliverables
- Source Code:
  - Re-engineered/refactored source code of the ckjm application.
- Comprehensive Report:
  - Design of Original Source Code:
    - Detailed analysis and documentation of the original design.
  - Summary of Design Defects Observed:
    - Identification and explanation of design flaws and areas for improvement.
  - List of Changes / Refactorings Applied:
    - Documentation of the specific changes and refactorings made to the original code.
  - Improved Design / Class Diagram:
    - Presentation of the enhanced design, including a class diagram and a discussion of the improvements achieved.
## Project Breakdown
#### 1. Design of Original Source Code
The original ckjm application design includes the following key components:

- ClassParser: Responsible for parsing Java class files.
- MetricsCalculator: Computes CK metrics based on the parsed class data.
- OutputHandler: Manages the output of computed metrics.
The original design, while functional, exhibited several design flaws such as tightly coupled components, lack of modularity, and poor readability.

#### 2. Summary of Design Defects Observed
- Tight Coupling: Many classes were highly interdependent, making the system difficult to modify and extend.
- Lack of Modularity: The code lacked clear modular separation, leading to code duplication and reduced maintainability.
- Poor Readability: Inconsistent naming conventions and lack of comments made the code hard to read and understand.
#### 3. List of Changes / Refactorings Applied
The following refactorings were applied to address the design defects:

- Decoupling Components: Introduced interfaces to reduce tight coupling between classes.
- Modularization: Reorganized code into distinct modules to improve separation of concerns.
- Code Cleanup: Improved naming conventions and added comments to enhance readability.
- Optimization: Refactored performance-critical sections to improve efficiency.
#### 4. Improved Design / Class Diagram
The improved design features a modular architecture with clearly defined interfaces and well-separated components. The class diagram below illustrates the enhanced structure:

## Improved Class Diagram
```
+-------------------+     +-------------------+     +-------------------+
|    ClassParser    |<----|   MetricsCalculator   |<----|   OutputHandler   |
+-------------------+     +-------------------+     +-------------------+
| + parseClass()    |     | + calculateMetrics()|     | + handleOutput()   |
|                   |     |                     |     |                   |
+-------------------+     +-------------------+     +-------------------+

```
## Discussion on Improvements Achieved
- Enhanced Modularity: The refactored design promotes modularity, making the system easier to maintain and extend.
- Improved Readability: The codebase is now more readable due to consistent naming conventions and thorough documentation.
- Reduced Coupling: Decoupling components through interfaces has improved flexibility and testability.
- Performance Optimization: Refactoring performance-critical sections has resulted in a more efficient application.
## Conclusion
The reengineering of the ckjm application has resulted in a more maintainable, readable, and efficient system. The refactorings applied have addressed the design flaws of the original code, leading to a significantly improved software design.

## Contact
For any questions or suggestions, please feel free to reach out!
