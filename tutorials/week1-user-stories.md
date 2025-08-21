---
layout: page
title: Requirments Engineering -- VSD, User Stories, and Conditions of Satisfaction
permalink: /tutorials/week1-user-stories
parent: Tutorials
nav_order: 3
---
This tutorial provides a description of Value Sensitive Design (VSD) and the process of applying it to define 
user stories. Further, it provides examples for user stories, conditions of satisfaction and how a minimum viable product can be defined. The process description and the examples will help understand the process of collecting requirements
as user stories and how to document them in a systematic way.

Contents:

* [What is VSD?](#what-is-vsd)
* [User Stories and Conditions of Satisfaction](#user-stories-and-conditions-of-satisfaction)
* [User Stories and Project Planning](#user-stories-and-project-planning)
* [User Stories and Test-Driven Development](#user-stories-and-test-driven-development)
* [Examples](#examples)

# What is VSD?

Like any technology, software reflects and affects human values. Ignoring values during the requirements collection and definition phase is irresponsible as it leads to software whose impact on communities that use it may be unintentional at best or actively harmful at worst. 

Value sensitive design (VSD) is a framework to systematically reason about values in software design. This involves the following:

- Combine empirical, value, and technical investigations
- Recognize the stakeholders involved and consider their values.
- Consider diverse perspectives.

The three types of investigation -- empirical, value, and technical into a value often require collaboration with experts in different fields ranging from sociology to philosophy to computer science. While this is difficult to practice without
access to a diverse team, this tutorial, through a few examples, will help you appreciate how the process can be applied to requirements gathering.

Before proceeding it is helpful to note what VSD is not! VSD does not prescribe a system of ethics or specific values, rather it incorporates value reflections in the requirements choosing process. 

## Informed Consent Online Example

Web applications today are pervasive. They have access to huge amounts of personal information to enable important
services to banking, education, entertainment, etc. Often such information is collected surreptiously, without the user's
consent. One way to address this problem is to encrypt personal data and prevent unauthorized access. However, solutions like encryption place the burden on automated technical mechanisms, with the software engineer as adjudicator. Another way is through informed consent, in which direct and indirect stakeholders, based on how the application works, choose whether to provide their personal data or not. 

To understand informed consent, we need to investigate how the concept works in the real-world (empircal) and reflect on how the concept may manifest in different ways (value investigation). The idea hinges on two concepts -- informed and consent. Informed encompasses *disclosure* and *comprehension*. Disclosure refers to providing accurate information about
the pros and cons of taking an action. If the action involves collecting personal information then the following should be made explicit: (1) what is being collected, (2) who will have access to it, (3) how long will it be stored, (4) what will it be used for, and (5) whether the data will be anonymized. Comprehension is complex in a digital or virtual environment due to the lack of face-to-face interactions. Hence as designers, we will need to analyze the interventions that need to be
created to ensure that the users understand the disclosures (e.g., a quiz). 

The second construct of *consent* encompasses *voluntariness*, *competence*, and *agreement*. *Voluntariness* simply means to ensure that the action was not coerced or manipulated. For e.g., the decision to accept or reject disclosure will affect essential usage. *Competence* refers to the mental and physical capabilities needed to give consent. For e.g., web applications meant for children will need to be mindful of this component. Finally, *agreement* refers to a clear opportunity to accept or decline participation. For e.g., in this context, the ability accept or reject must be visible and
accessbile and not obscured in layers.  

Once we have completed the emprical and value investigation of informed consent, we can think about how to implement it
given our technical constraints. This is where we translate our observations into user stories and conditions of satisfaction (see Examples section). Before we see how to do this let's take a detour and understand the structural constraints of defining user stories and conditions of satisfactions. 

# User Stories and Conditions of Satisfaction

A user story is an informal, general explanation of a software feature written from the perspective of the **end user or customer**. A user story is always of the following form:

As a <code>&lt;role&gt;</code> I can <code>&lt;perform action&gt;</code> so that I can <code>&lt;receive benefit&gt;</code>

User stories represent something the user/customer might want. There will be many ways to give the user/customer the benefit that they want.

We need to refine these in order to determine what to build. We call these refinements “conditions of satisfaction” (COS)

A COS should be a specific capability or behavior that the user expects, in the user’s terms.  It should be visible to and verifiable by the user.

The COS is a guide to the implementation team. It should be specific enough so that the implementation team has a clear idea of what they are building.
There still may be many ways to implement a COS. For example, a COS probably would not specify any of the graphic or layout details; these would likely be left to the implementation team.


# User Stories and Project Planning

In planning a project, need to assign priorities to each user story and Condition of Satisfaction. Priorities tell us the order in which COS and their associated engineering tasks should be addressed, and how much effort should be devoted to each of them.
There are many ways to describe priorities. For example, a user story might be described as Essential, Desirable, or Extension:

* **Essential** means the project is useless without it.
* **Desirable** means the project is less usable without it, but is still usable.
* **Extension** describes a User story or COS that is desirable, but may not be achievable within the scope of the project.

## Minimum Viable Product (MVP)

An MVP is a product that consists of all essential user stories. Developers should prioritize those above others.

# VSD, User Stories and Test-Driven Development

We model the development process as a cycle of refinements:

1. VSD analysis to gather requirements
2. User Stories to dcoument gathered requirements
2. Conditions of Satisfaction
3. Testable behaviors
4. Executable Tests
5. Engineering Tasks (Code)

As we proceed down these refinements, we will likely go back and revisit design decisions that we made at earlier stages. This is the topic of Module 02.

# Examples

## User Stories Without VSD

### User Story #1

As a user of stack overflow, I want to be able to reply to questions with answers so that I can help others with my knowledge. (Essential)

### User Story #2

As a user of stack overflow, I want to be list my replies and how often they are upvoted so that I can see how well people react to my answers.  (Desirable)

### User Story #3

As a user of stack overflow, I want to be able to play the codel (like the wordle but for code) so that I can enjoy my time on the site. (Extension)

## Informed Consent User Story (Using VSD)

As a user of stack overflow, I want to understand what personal information is collected so that
I can make an informed decision about my privacy when using the website. (Essential)

## Conditions of Satisfaction

### For User Story #1

* There should be a place on questions to post my reply with an answer (Essential)
* Replies should be visible to anyone who views the question (Essential)
* I should be able to format my reply with syntax highlighting. (Desirable)
* Replies should pop up in real-time without needing to reload the page (Extension)

### For User Story #2

* I should be able to view a list of my replies and how many upvotes they have each received. (Essential)
* I should be able to click on a reply from the list and it links me to the appropriate page. (Desirable)
* Other users should be able to see my replies and total number of upvotes (Desirable)
* I should be able to compare my total number of upvotes with all the other users on the site. (Extension)

### For User Story #3

* I should be able to play the codel and use my knowledge of programming languages and practices to solve puzzles. (Essential)
* Everyday the puzzle should change to something new. (Essential)
* I should be able to share how well I did on the codel without spoiling the answer. (Desirable)
* Puzzles should generate randomly so there is always a new puzzle. (Extension)

### For Informed Consent User Story

* The system shall clearly state that cookies are being used to collect login tokens, voting history, and search queries. (Essential) (relates to disclosure)
* Only admins will have access to the information collected in the cookies (Essential) (relates to disclosure)
* The data in cookies will expire in a week (Essentail) (relates to disclosure)
* The data collected in cookies will be encrypted to prevent unauthorized access (Essential) (relates to disclosure)
* The system shall make a clear distinction between essential and non-essential cookies (Essential) (relates to voluntariness)
* The system shall allow users to read all posts and make their own posts even if they reject non-essential cookies (Essential) (relates to voluntariness)
* The cookie consent interface shall provide equally prominent "Accept" and "Reject" buttons (Essential) (relates to agreement)
* The system shall explain what the data collected in cookies will be used for (Desirable) (relates to comprehension)
* The system shall provide interactive examples or tooltips explaining technical terms (Desirable) (relates to comprehension)
* The system shall remember user preferences and not repeatedly prompt for consent (Extension) (relates to agreement)
* Cookie settings shall be accessible via keyboard navigation and screen readers (Extension) (relates to competence)

Note in addition to the planning labels, how the labels in the informed consent COS can be used to track if the COS
meets the analysis laid out in the VSD process. Further, following a VSD process allowed us to defined more detailed
COS as opposed to not using VSD in the user stories 1-3. 

[User Stories](https://www.simplilearn.com/tutorials/agile-scrum-tutorial/user-stories#how_to_write_user_stories)
[VSD](https://vsd.ccs.neu.edu/introduction/what-is-vsd/)