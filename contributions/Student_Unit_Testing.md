# Unit Testing

## Introduction

Unit testing is a type of software testing in which the smallest parts of a program, called units, are tested one by one. A unit is usually a single function, method, or module. In Software Engineering, unit testing is done during the implementation phase, usually by the developer who wrote the code, to check that each unit works correctly on its own before it is combined with other parts of the system.

## Example

Consider a Login Module of a college management system. The module takes a username and a password and allows the user to enter the system only if both are correct. Before this module is joined with the rest of the system, it is tested alone using a set of test cases:

| Test Case ID | Input (Username, Password) | Expected Output | Actual Output | Result |
|---|---|---|---|---|
| TC01 | Valid username, valid password | Login successful | Login successful | Pass |
| TC02 | Valid username, wrong password | Error message shown | Error message shown | Pass |
| TC03 | Blank username, blank password | Error message shown | Login successful | Fail |
| TC04 | Username longer than limit | Error message shown | Error message shown | Pass |

Test case TC03 has failed, which tells the developer that the validation for empty fields is missing inside the login unit itself. Since only this one module was being tested, the defect is located and corrected immediately, without having to search the whole system.

## Advantages

- Errors are found early, so the cost of fixing them is much lower.
- Each unit is tested in isolation, so the exact location of a defect is easy to find.
- Code can be changed or improved safely because the tests confirm nothing is broken.
- Test cases act as simple documentation of how a unit is supposed to behave.
- Supports Test Driven Development and makes later integration testing easier.

## Conclusion

Unit testing is an important part of the software development life cycle. It improves the quality and reliability of software by verifying each unit separately before integration. A system built from well tested units is easier to maintain, easier to extend, and less likely to fail after release.
