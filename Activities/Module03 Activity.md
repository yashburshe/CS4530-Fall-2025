---
layout: page
title: Test Adequacy
nav_exclude: true
---
## Test Adequacy Activity
We will gain experience improving test suites using two adequacy criteria: line coverage and mutation coverage. The instructions refer to line numbers in `transcriptManager.ts`. Do *not* change that file while you are following along, or else you may find that the line referenced do not match what you see.

### Test Coverage

As usual, download the [starter code]({{ site.baseurl }}{% link Activities/module03-test-adequacy.zip %}) and run `npm install`.

Then run the tests, using `npm test`. You should see that all tests pass, but lines 91 and 110 are not covered. Write tests to cover those lines. Put your new tests in a file `newTests.test.ts`.

Then run `npm run stryker` to see the mutation report. You should see that 12 mutants survived.  Classify the surviving mutants into innocuous (didn't introduce a bug) and non-innocuous (did introduce a bug).

In the file `newTests.test.ts`, write tests that will kill the non-innocuous mutants. For each mutant that you classified as innocuous, write a comment explaining why you think it is innocuous.

Grading: 
* +1 point for covering each of the two uncovered lines
* +1 point for each mutant correctly classified as innocuous or non-innocuous and killed if non-innocuous (up to 12 points). 
* Total grade is the sum of the two parts, up to 10 points.

Be sure to review the canvas assignment for submission and other related details (if assigned).