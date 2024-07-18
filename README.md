[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/ycVsfoVh)
# test-ing--drive

In bootcamp you explored the principles of TDD (what is a test, writing a test before code, red-green-refactor, etc.). Before we meet up again to go deeper into testing, I'd like you to explore how testing works on your projects.

To submit your answers, you must first create a branch of this repository, then edit this README file.

1. Describe the approach to TDD on your delivery. In general, how strict are people writing tests before code? (This is not a judgement, just an observation of what you are noticing). What makes it difficult to start with tests? What might make it easier?

From the pieces of work I've shadowed and paired on, I've notices that we've rarely written tests before writing solutions

2. What testing frameworks are in use? Is the same framework used for everything, or do you have a framework for testing code, and one for testing a website or service?

Cypress, Jest => Front-end, cypress E2E and Pytest => backend. Don't know what we use to test Terraform, is there a way?

3. Looking at the language(s) used, list at least 5 other testing frameworks. What do they have in common, and what's their unique proposition?

TS - Mocha, Jasmine, Bun,
Bun - All in one JS runtime, with included test runner, can also do TS, claims to be super rapid and lightweight.
Python - PyUnit or UnitTest, pyunit build into python already so no need for other packages, however meant to be more verbose than PyTest for example.

4. Using a coverage tool, what is the test coverage on the project (If there's more than one project, choose one). What might that result suggest? In what area would you discuss adding more tests?

Coverage for the project is around 85% for the end and 95% for the backend. Suggests it might be slightly more awkward to test the front-end, interestingly we also use SonarCloud, which also runs a coverage tool and reports whether tests are missing for conditional branches.


6. Looking at the tests written, how confident would you say they:
    - describe what is happening
    - correctly document what the code should be doing
    - drive development of the code (because of this test this feature *and only this feature* was made)



