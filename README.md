[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/ycVsfoVh)
# test-ing--drive

In bootcamp you explored the principles of TDD (what is a test, writing a test before code, red-green-refactor, etc.). Before we meet up again to go deeper into testing, I'd like you to explore how testing works on your projects.

To submit your answers, you must first create a branch of this repository, then edit this README file.

1. Describe the approach to TDD on your delivery. In general, how strict are people writing tests before code? (This is not a judgement, just an observation of what you are noticing). What makes it difficult to start with tests? What might make it easier?

- The team typically writes tests after the code is completed. This appears to be due to the significant amount of time required to create the necessary mocks for testing.

2. What testing frameworks are in use? Is the same framework used for everything, or do you have a framework for testing code, and one for testing a website or service?

- Jest for the React frontend
- PyTest for the backend Lambdas
- Cypress for frontend end-to-end testing

3. Looking at the language(s) used, list at least 5 other testing frameworks. What do they have in common, and what's their unique proposition?

| Alternative | Alternative To | Comman Factors | Unique Propositions |
|----------|----------|----------|----------|
| Mocha | Jest | JavaScript Support, Asynchronous Testing, Integration with CI/CD, Community and Documentation, Assertions | It doesn’t impose any particular structure, allowing developers to choose their own libraries for assertions, mocking, etc. |
| Chai | Jest | JavaScript Support, Asynchronous Testing, Integration with CI/CD, Community and Documentation, Assertions | It offers a variety of assertion styles (should, expect, assert) to match the developer's preference. It supports a wide range of plugins that extend its functionality, allowing for more expressive tests.|
| Enzyme | Jest | JavaScript Support, Asynchronous Testing, Integration with CI/CD, Community and Documentation, Assertions | Enzyme is specifically designed for testing react components. So it has utilities to simulate user interactions, traverse component trees and assert component states. It allows shadow redering which is the ability to render components without their children. This makes unit tests easier and faster. |
| unittest | PyTest | | It comes with Python's standard library, making it readily available without any additional installations. It encourages a more object-oriented approach to testing, with test cases defined as classes. |
| nose2 | PyTest | Both have a rich plugin ecosystem although pytest's might be broader. Both use python assert statements.| Allows fine-grained control over test execution and reporting. |
| doctest | PyTest | Used for testing python code | doctest is specialized for ensuring that code examples in documentation are correct and functional |

4. Using a coverage tool, what is the test coverage on the project (If there's more than one project, choose one). What might that result suggest? In what area would you discuss adding more tests?

- The team standard for test covearge is: 80%
- For the python backend test coverage is: 95%
- For the react front end, test coverage is: 85%

5. Looking at the tests written, how confident would you say they:
    - describe what is happening
    - correctly document what the code should be doing
    - drive development of the code (because of this test this feature *and only this feature* was made)
| Criteria                      | Confidence Level                              |
|------------------------------|-----------------------------------------|
| **describe what is happening**      | 70% |
| **correctly document what the code should be doing**           | 75% |
| **drive development of the code (because of this test this feature *and only this feature* was made)**                 | 30% |

