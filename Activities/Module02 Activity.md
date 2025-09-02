---
layout: page
title: Test-Driven Development
nav_exclude: true
---

## Test-Driven Development

This activity is intended to supplement the CS4530 lecture on test-driven development.

Start by downloading and unpacking the [starter Code]({{ site.baseurl }}{% link Activities/module-02-tdd-transcript-activity.zip %})

## Steps
The slides for module 2 list a number of decisions that were made in the negotiations with the client. However, the tests in `transcriptService.test.ts` do not check all of those decisions.

1. Review the decisions listed on the slides for this lecture, and identify at least 3 decisions that are not addressed by `transcriptService.test.ts`, or are themselves ambiguous and require further negotiation. Also identify at least two tests that are included in `transcriptService.test.ts` that make assumptions about the system that are not justified by the decisions listed on the slides.
2. Write tests to check each of the conditions you have identified. Put these tests, along with the conditions they are supposed to check. 
3. Run your tests in this repository, and identify which of the conditions are not satisfied by the existing code. (Your tests need not be exhaustive, and you need not attempt to fix the bugs you uncover.)
4. Create a file named `module02.test.ts` containing the conditions you identified, the tests you wrote, and the results.

When you are done, submit your work as required by your instructor (check the Canvas asssignment for details, if assigned). This may vary from section to section.