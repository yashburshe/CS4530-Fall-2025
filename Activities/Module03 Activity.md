---
layout: page
title: Test Adequacy
nav_exclude: true
---
## Test Adequacy Activity
We will gain experience improving test suites using two adequacy criteria: line coverage and mutation coverage. The instructions refer to line numbers in `transcriptManager.ts`. Do *not* change that file while you are following along, or else you may find that the line referenced do not match what you see.

### Test Coverage

As usual, download the [starter code]({{ site.baseurl }}{% link Activities/module03-test-adequacy.zip %}) and run `npm install`. Run the tests with `npm test` and observe that all tests pass.

Please write tests so that lines 91 and 110 are covered. (1 point each)

Create a file called `newTests.test.ts`. Add tests to that file to cover those lines. You can run `npm test` to see if your tests are passing.

### Mutation Testing

Then run Stryker to perform mutation testing by running `npm run stryker`. You should find that there are 12 surviving mutants. for each of the surviving mutants, determine whether the mutant is
1. Equivalent (i.e., the system with the mutant is functionally identical to the original code)
2. The mutant is not functionally identical, but the mutant is not a real bug.
3. The mutant is a real bug that should be fixed.

 For each surviving mutant in categories 1 and 2, write a short justification of why you believe the mutant is equivalent or not a real bug. Write your justifications as comments in `newTests.test.ts`.

For each surviving mutant that represents a real bug, write a test that will kill the mutant. Put all your new tests in `newTests.test.ts`. 

When you are done, submit that file only.

Grading: 1 point for each surviving mutant that is correctly classified and killed if applicable.  

Maximum of 10 points (that is, full credit if you get 10 or more points according to the grading rubrics above).

Be sure to review the canvas assignment for submission and other related details.


