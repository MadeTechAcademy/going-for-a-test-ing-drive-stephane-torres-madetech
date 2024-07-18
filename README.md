[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/ycVsfoVh)
# test-ing--drive

In bootcamp you explored the principles of TDD (what is a test, writing a test before code, red-green-refactor, etc.). Before we meet up again to go deeper into testing, I'd like you to explore how testing works on your projects.

To submit your answers, you must first create a branch of this repository, then edit this README file.

1. Describe the approach to TDD on your delivery. In general, how strict are people writing tests before code? (This is not a judgement, just an observation of what you are noticing). What makes it difficult to start with tests? What might make it easier?

From the pieces of work I've shadowed and paired on, I've noticed that we've rarely written tests before writing solutions, but tests are definitely present and used to verify that the code is doing what it's expected to do. I think part of the difficulty of writing tests first could be the need to mock different AWS services and the different interactions between these and previously existing code and how everything will/is meant to work together.

2. What testing frameworks are in use? Is the same framework used for everything, or do you have a framework for testing code, and one for testing a website or service?

Cypress, Jest => Front-end, Cypress E2E, and Pytest => backend. Don't know what we use to test Terraform, is there a way?
Cypress is pretty cool and used to test the website and different workflows, you're able to define a workflow touching different aspects and pages of the code, assert what is expected to be present on the page or what page you're meant to be on depending what response you get back from queries, clicks are made etc



3. Looking at the language(s) used, list at least 5 other testing frameworks. What do they have in common, and what's their unique proposition?

TS - Mocha, Jasmine, Bun, => All claim to be simpple, work with pretty much any framework or library.
Bun - All in one JS runtime, with included test runner, can also do TS, claims to be super rapid and lightweight.
Jasmine - Super simple, doesn't require a DOM...? doesn't depend on anything else, no external dependencies, can do both browser and NodeJS testing, "Behaviour driven".
Mocha - Not sure what the unique propositon is here, doesn't come with it's own assertion or mocking library but easily integrates with others, used often with Chai.

Python - PyUnit or UnitTest, Selenium
pyunit - build into python already so no need for other packages, however meant to be more verbose than PyTest, using classes and methods to define test cases rather than simple function definitions.
Selenium - Useful for testing web based apps opens up a browser and tests elements

4. Using a coverage tool, what is the test coverage on the project (If there's more than one project, choose one). What might that result suggest? In what area would you discuss adding more tests?

Coverage for the project is around 85% for the frontend and 95% for the backend. Suggests it might be slightly more awkward to test the front-end code, interestingly we also use SonarCloud, which also runs a coverage tool and reports whether tests are missing for conditional branches.


6. Looking at the tests written, how confident would you say they:
    - describe what is happening
    - correctly document what the code should be doing
    - drive development of the code (because of this test this feature *and only this feature* was made)
  

Looking at the tests I feel like they generally describe what is happening very well, it has taken some time to understand them, especially when it comes to what's being mocked and why, still getting the hang of it. Fixtures, mocker and mocking still confuse me a bit.
Naming of test, functions and variables, both within the tests and features, definitely aid in documenting what the code should be doing.

In terms of driving development, testing and sandboxing features of features definitely flags bugs and drives the fixing of these only for features being worked, but is not the only drive for development of the feature being worked on.  


<!-- Over that past few weeks, having been more involved in some of the development of certain features, I've definitely become more confident in undertanding what is happening in the tests, and being able to describe them. I do still find the idea of mocking and setting up what needs to be mocked and what doesn't quite confusing. This also depends on what is being tested/complexity of feature or problem. For example; features like testing React is navigating to the correct places/pages with the correct props/elements I feel is still beyond me, possibly because not taking the time to deep dive and play with Navigate() in React. Or to what extend to test a feature, Abid and I worked on a toggle button, to make simple assertions meant a lot of mocked/forced re-renders of a component in our tests adding a lot of bloat, whether this sort of testing is necessary to write or if sandboxing and QA testing is more appropriate.  -->









