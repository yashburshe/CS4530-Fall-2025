---
layout: page
title: Requirement Engineering Using Value Sensitive Design
nav_exclude: true
---
## Activity: Requirement Engineering Using Value Sensitive Design

### Introduction

This activity will give you practice with requirements analysis using an ethical framework such as value sensitive design. Additonally, you will document the requirements gathered during the analysis using user stories with conditions of satisfaction. 

Before you start, be sure to review the Reddit case study discussed in the lecture slides and the tutorial "Requirement Engineering using VSD" on the course website.

### The Reddit Case Study

Reddit uses human moderators to regulate posts and ensure that their community guidelines for speech are not violated. However, this is cumbersome and time consuming. They want to develop a classifier model that will replace the role of humans in the moderating process. This algorithm will classify new posts, determining whether or not they’re appropriate for Reddit. Those that are flagged inappropriate will be removed.

#### Empirical Investigation - Development of the Model 

The training data for the classifier model has two primary elements:

1. Posts that Reddit users have flagged previously
2. A dataset of English words that would be flagged as inappropriate

During this investigation we want to reflect on the sources of data. To this end we should think about the following questions:

- Is the dataset representative of the language we want removed?
- Are there any sources of biases or disparities that in this data that we should be considering?

Further, we also want to think about the complications that may arise from using such a model. Specificall, given the contextual nature of offensive speech, what complications or problems can arise from this model?

#### Value Investigation – Who are the Stakeholders? 

During this analysis we will reflect on thee following questions:

- Relative to the issue of content moderation, who or what are the stakeholders? (i.e. individuals or groups whose interests stand to be impacted by this algorithm?)
- Relative to the issue of content moderation, what are the interests or values of the different stakeholders?
- Are there any conflicts of interests or values?
- Overall, given the different stakeholders, interests and values, do any of them stand out to you as ones we should prioritize? Why?
- Why do you think some people might be concerned with Reddit removing user’s posts? What if the posts have misinformation or hate speech?
- How are users harmed if posts are mistakenly removed by Reddit?
- How can bias in the moderation algorithms potentially harm users?
- Given the debate on free speech vs. content moderation what do you think are the strengths and weaknesses of the proposed requirement?

#### Technical Investigations

Suppose as a result of the value investigations we came up with two high-level requirements:

1. The flagging feature gives an explanation to the user as to why the system flagged and removed their content. If, after reading the explanation, the user thought the flagging was in error, they can submit the flag for further review. 

2. The system prompts the user to reconsider if their post is potentially offensive, but does not prevent it from being posted.

Which requirement would you prefer based on the technical feasibility and the values that you think are important?


### Requirements for this activity

1. Choose one of the two high-level requirements (in technocal investigations) using the VSD process. Briefly explain your reasoning. In your explanation be sure to identify at least 3 stakeholders (e.g., consumer) and 3 values (e.g., informed consent).
   
2. Define a user story for each stakeholder.  These should be of the form
   
    As a <code>&lt;stakeholder&gt;</code> I want <code>&lt;some capability&gt;</code> so that I can <code>&lt;get some benefit&gt;</code>

3. For **each** user story, write 3 conditions of satisfaction with appropriate priorities. (Essential = user story is not satisfied without it)

Please submit a total of:

* 1 high-level requirement with your analysis
* 3 user stories
* 9 conditions of satisfaction with priorities

When you are done, submit your work as required by your instructor (check the Canvas asssignment for details, if assigned). This may vary from section to section.

### Grading Criteria: 10pts

* High Level Requirement Chosen and Analysis (4 pts) 
* 3 user stories (3 pts) 
* 9 conditions of satisfaction with appropriate priorities (3 pts)