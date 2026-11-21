Software Maintenance, Reengineering, and AI in Software Engineering
Student & Case Study Details
 * Name: Kanishk Ashok Reddy
 * USN: NB25CSE165
 * Case Study: Question 5 — Software Maintenance, Reengineering, and AI in Software Engineering

1. Introduction
Software maintenance is the process of modifying and updating a software system after delivery to correct faults, improve performance, adapt to changing environments, or enhance functionality over its operational lifecycle. When a legacy system ages, routine maintenance alone may not be enough, making software reengineering (examining, restructuring, and rebuilding a system into a newer form without changing its core business purpose) and AI-assisted software engineering (using intelligent tools for code analysis, bug detection, refactoring, and test generation) essential for sustainable modernization.

2. Problem Analysis
The college's existing Student Management System has been in operation for several years and exhibits three core problems:
 * Poor Performance (Slow Execution): The system has become slow, indicating bottlenecks such as unoptimized database queries, legacy code structures, or insufficient resource handling as student and academic records scale.
 * Outdated Features: The application contains outdated features that no longer align with modern academic workflows, user expectations, or current institutional standards.
 * Frequent Errors and Reliability Issues: The software frequently produces errors, pointing to technical debt, brittle modules, or inadequate error handling and testing coverage.

3. Proposed Solution
A. Suitable Types of Software Maintenance
A balanced combination of maintenance categories is needed to stabilize and evolve the Student Management System:
 * Corrective Maintenance: Fixes runtime bugs, crashes, and data-handling defects that cause frequent errors in the existing system.
 * Adaptive Maintenance: Updates the software to run smoothly on current operating systems, databases, frameworks, and cloud/campus infrastructure.
 * Perfective Maintenance: Refactors slow modules, optimizes queries, and adds modern features or improved user interfaces to address performance and usability gaps.
 * Preventive Maintenance: Cleans up technical debt, improves code modularity, and strengthens logging and validation so future failures are minimized.
B. Steps Involved in Software Reengineering
To modernize the system systematically without losing institutional data or core workflows:
 * Inventory Analysis: Catalog existing modules, database schemas, dependencies, and integrations to establish a modernization baseline.
 * Document Restructuring: Update outdated system documentation and architectural diagrams to match actual runtime behavior.
 * Reverse Engineering: Analyze legacy source code and database structures to extract business rules, data flows, and system design.
 * Code and Data Restructuring: Refactor messy or tightly coupled code and normalize/clean database tables to improve readability and speed.
 * Forward Engineering: Rebuild or upgrade modules using modern architectures, frameworks, and security practices based on the recovered design.
C. Two Applications of AI in Software Engineering
 * AI-Assisted Code Analysis, Refactoring, and Bug Detection: AI coding and static-analysis assistants can flag error-prone code paths, suggest performance optimizations for slow loops or queries, and assist developers in refactoring legacy modules safely.
 * AI-Driven Automated Test Generation: AI tools can generate unit tests, regression test cases, and edge-case scenarios to catch regressions early and reduce recurring system errors.
D. Modernization Workflow Diagram
+-----------------------------------+
|   Legacy Student Management       |
|   System (Slow, Outdated, Buggy)  |
+-----------------+-----------------+
                  |
                  v
+-----------------------------------+
|   Software Maintenance            |
|   (Corrective, Adaptive,          |
|    Perfective, Preventive)        |
+-----------------+-----------------+
                  |
                  v
+-----------------------------------+
|   Software Reengineering          |
|   Inventory -> Reverse Eng. ->    |
|   Restructuring -> Forward Eng.   |
+-----------------+-----------------+
                  |
        +---------+---------+
        |                   |
        v                   v
+---------------+   +---------------+
| AI Code & Bug |   | AI Test Gen.  |
| Assistance    |   | & QA          |
+-------+-------+   +-------+-------+
        |                   |
        +---------+---------+
                  |
                  v
+-----------------------------------+
|   Modernized, Reliable & Fast     |
|   Student Management System       |
+-----------------------------------+

4. Benefits and Challenges
Three Expected Improvements
 * Faster System Responsiveness: Query tuning, restructured logic, and modernized components reduce page load and transaction processing times.
 * Higher Reliability and Fewer Errors: Fixing root defects, refactoring fragile code, and expanding automated test coverage lower the frequency of runtime errors.
 * Upgraded Features and Maintainability: Replacing outdated features with modern workflows makes the system easier for staff, students, and developers to use and maintain.
Additional Benefits and Challenges
 * Benefits: Lower long-term support costs, stronger maintainability for future academic updates, and improved data integrity across student records.
 * Challenges & Limitations: Potential data migration risks during reengineering, initial training overhead for staff and IT teams, and the need to human-verify AI-generated code or tests to avoid subtle logic flaws.

5. Conclusion
Modernizing the college's aging Student Management System requires pairing targeted software maintenance (corrective, adaptive, perfective, and preventive) with structured software reengineering and AI-assisted software engineering. By diagnosing performance bottlenecks, outdated features, and recurring errors upfront—and applying disciplined reengineering alongside AI-supported refactoring and testing—the institution can achieve a faster, more reliable, and future-ready platform while managing migration risks carefully.

