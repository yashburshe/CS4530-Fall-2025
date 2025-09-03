---
layout: page
title: Test-Driven Development
nav_exclude: true
---

## Activity: Test-Driven Development

This activity is intended to supplement the CS4530 lecture on test-driven development.

Start by downloading and unpacking the [starter Code]({{ site.baseurl }}{% link Activities/module-02-tdd-transcript-activity.zip %})

### Steps
The slides for module 2 list a number of decisions that were made in the negotiations with the client. However, the tests in `transcriptService.test.ts` do not check all of those decisions.

1. Review the decisions listed on the slides for this lecture, and identify at least 3 decisions that are not addressed by `transcriptService.test.ts`, or are themselves ambiguous and require further negotiation. Also identify at least two tests that are included in `transcriptService.test.ts` that make assumptions about the system that are not justified by the decisions listed on the slides.
2. Write tests to check each of the conditions you have identified. Put these tests, along with the conditions they are supposed to check. 
3. Run your tests in this repository, and identify which of the conditions are not satisfied by the existing code. (Your tests need not be exhaustive, and you need not attempt to fix the bugs you uncover.)
4. Create a file named `module02.test.ts` containing the conditions you identified, the tests you wrote, and the results.

When you are done, submit your work as required by your instructor (check the Canvas asssignment for details, if assigned). This may vary from section to section.

### Grading Rubric:

Grading will be done via "specification grading". 

There are only two non-zero grades: Satisfactory (10 points), and Minimal (5 points).

To obtain a grade of Satisfactory, you must deliver all of the requirements listed in the instructions.

To obtain a grade of Minimal, you must:
* Identify at least one decision that is not addressed by the tests in transcriptService.test.ts.
* Write a condition that resolves that decision
* Write a Jest test  or tests to check that decision
* Run the tests in the repository, and identify whether the repository meets the condition you have identified.

Submit a file named module02.test.ts with your answers.

Grading will be manual; the TAs will look at your solution; they may or may not run them.