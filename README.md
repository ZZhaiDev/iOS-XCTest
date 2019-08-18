# iOS-XCTest


## What Is Continuous Integration (CI)
Continuous Integration (CI) is an automated way for you to test code and push builds for testing and App Store deployment. 

## Why we use Continuous Integration (CI)
* `Automated tests` are run by a central server before every build is pushed. Writing and maintaining a test suite for your app may feel tedious, but in the long run you will have more confidence that your code won’t contain bugs. You can also push more regularly due to a lower reliance on manual testing, which can be very time consuming.
* We can guard against `malicious code injection`. This is important if you are working in a team environment and a developer may have something to gain by injecting code that, for example, logs a user’s private keys. A good CI process can ensure that every commit is peer reviewed before it is merged. Because only the CI server has access to the certificates needed to push to the app store, only code that has been merged through peer review will be compiled and pushed to the store.
* It gives us `verifiable code`. By using automated tagging, we can ensure our GitHub repo is tagged correctly for every build and that the exact commit hash of the build is embedded into our app. This gives us 100% confidence in our ability to identify what code is running where.
* It `saves time`. Pushing builds out constantly can become very time consuming. A good CI will take care of all this for you. Automated testing also reduces the need for time consuming manual testing.

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
* [This guide will help you set up a server to test, build, and deploy your iOS apps automatically.](https://blog.keys.casa/ios-continuous-integration-guide/)
* [Easy CI with fastlane: How we automated everything iOS from running tests to distributing a build](https://medium.com/aaptiv-engineering/easy-ci-with-fastlane-how-we-automated-everything-ios-from-running-tests-to-distributing-a-build-5ecbb817fba0)
* [fastlane is the easiest way to automate beta deployments and releases for your iOS and Android apps](https://docs.fastlane.tools/)
* [How to Write Unit Tests in Swift](https://www.agnosticdev.com/content/how-write-unit-tests-swift)
