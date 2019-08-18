# iOS-XCTest

## Difference between Unit test and Integration test
* `Unit tests`: A single piece of code (usually an object or a function) is tested, isolated from other pieces
* `Integration tests`: Multiple pieces are tested together, for example testing database access code against a test database

## Code Coverage
* Code coverage in Xcode is a testing option supported by LLVM. When you enable code coverage, LLVM instruments the code to gather coverage data based on the frequency that methods and functions are called. The code coverage option can collect data to report on tests of correctness and of performance, whether unit tests or UI tests.
* Code coverage is a tool to measure the value of your tests. It answers the questions
  1. What code is actually being run when you run your tests?
  2. How many tests are enough tests? In other words, have you architected enough tests to ensure that all of your code is being checked for correctness and performance?
  3. What parts of your code are not being tested?
* After a test run is completed, Xcode takes the LLVM coverage data and uses it to create a coverage report in the Reports navigator, seen in the Coverage pane. It shows summary information about the test run, a listing of source files and functions within the files, and coverage percentage for each.

## Other Resources
* [How to Write Unit Tests in Swift](https://www.agnosticdev.com/content/how-write-unit-tests-swift)
