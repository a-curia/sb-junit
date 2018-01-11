Unit Testing, Test-Driven Development(TDD) and Behavior-Driven Development(BDD)
-------------------------------------------------------------------------------

 

Ok... so what are these? Where can and should use them?

 

**Unit testing**

-   focus on single “unit of code”, usually a function in an object or module

-   test is specific to a single function, so the test should be simple, quick
    to write and quick to run

-   very useful when you change your code and want to check you don’t break
    other parts

-   should be isolated from dependencies(no network access and no database
    access)

-   you can replace these dependencies with tools that fake the dependency

-   conclusion: individual tests, which test one thing, and they are isolated
    from each other

-   Three of the most common types of automated tests:

    -   **Unit tests**: A single piece of code (usually an object or a function)
        is tested, isolated from other pieces

    -   **Integration tests**: Multiple pieces are tested together, for example
        testing database access code against a test database

    -   **Acceptance tests (also called Functional tests)**: Automatic testing
        of the entire application, for example using a tool like Selenium to
        automatically run a browser.

 

TDD

-   TDD works great with unit tests, but you can apply it to other testing
    methods as well.

-   It also does not require any specific tool or syntax.

-   difficult for developers is the fact that you have to write the tests before
    writing code

TDD process consists of the following steps:

1.  Start by writing a test

    1.  Run the test and any other tests. At this point, your newly added test
        should fail. If it doesn’t fail here, it might not be testing the right
        thing and thus has a bug in it.

    2.  Write the minimum amount of code required to make the test pass

    3.  Run the tests to check the new test passes

    4.  Optionally refactor your code

    5.  Repeat from 1

 

BDD

-   applied to automation, BDD is a set of best practices for writing great
    tests

-   can and should be used together with TDD and Unit Testing methods

-   one of the key things BDD addresses is implementation detail in unit tests

-   Unit tests rely too much on how the tested function is implemented; this
    means if you update the function, even without changing the inputs and
    outputs, you must also update the test; this makes doing changes tedious, so
    it is a problem

-   you should not test implementation, but instead behaviour

 

Unit testing gives you WHAT

TDD gives you WHEN

BDD gives you HOW
