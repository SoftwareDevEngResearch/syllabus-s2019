---
layout: default
permalink: /
---

# <img src="assets/logo.svg" alt="class logo" class="logo"/> Software Development for Engineering Research syllabus

***If you are a teacher or interested in the design of the course, see the [meta](https://github.com/SoftwareDevEngResearch/syllabus/blob/gh-pages/meta.md) document.***

* **Course:** [ME 599](http://catalog.oregonstate.edu/CourseDetail.aspx?subjectcode=ME&coursenumber=599)
* **Instructor:** Kyle Niemeyer, [kyle.niemeyer@oregonstate.edu](mailto:kyle.niemeyer@oregonstate.edu)
* **Need help?**
    * [![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/SoftwareDevEngResearch/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
        * It sends message digests to people who aren't active in the room, so feel free to ask a question even if no one's around.
    * Look through and create [issues](https://github.com/SoftwareDevEngResearch/syllabus/issues)
   * [Email](mailto:kyle.niemeyer@oregonstate.edu) for 1-on-1 help, or to set up a time to meet using <https://calendly.com/kyle-niemeyer>

## Course Description

This course will advance students' understanding of topics related to computational science and engineering, and advance their skills in applying techniques to solve research problems using high-level programming languages. The course will build on existing abilities in computer programming to cover topics related to computational modeling and scientific software development. Students will gain experience in applying available packages and libraries, as well as developing software to solve problems related to their own research interests. Students will also gain experience in working collaboratively and openly on scientific computing projects.

By the end of this course, you will be able to:

1. use high-level programming language to analyze and/or solve practical research problems;

2. apply principles of modern computational science and engineering, reproducibility, and open science to your research;

3. evaluate, visualize, write about, and publish computational research results; and

4. develop and share an open-source research software package that solves a problem in your research area.

## Prerequisites

* [ME 499/599 "ST/Computer Programming for Mechanical Systems"](http://catalog.oregonstate.edu/CourseDetail.aspx?subjectcode=ME&coursenumber=599) or equivalent
* Basic understanding of Python

These won't be enforced by the instructor, but you will be pretty lost without understanding those concepts. If you need a refresher, take a look at the [Beginner Materials](#beginner-materials).

## Course Overview

We will dive into the nuances of JavaScript, how prototypal inheritance compares to classical inheritance, and how this can be used to build dynamic and complex web applications.  Modern tools like jQuery and BackboneJS will be discussed, but students will learn the building blocks of these frameworks and after this course be able to understand what is happening under the hood.  The focus will be on development for browsers, though most applies to other systems like Node.js, Phonegap, etc.  Topics covered include:

* Structuring programs, modular/functional programming
* Using classes, objects, and arrays
* Storing and manipulating data in files, HDF5
* Version control; working collaboratively & peer code review
* Software testing & continuous integration
* Analysis; plotting & visualization
* Interfacing with other languages
* Introduction to parallel computing
* Measuring and improving performance
* Reproducible research
* Effective software documentation
* Writing & publishing about computational research
* Deploying & sharing software; licenses & copyright

Topics will be demonstrated through live-code examples/slides. Additional exercises will completed in-class.

## Homework/Projects

All assignments will be listed within the [Course Outline](#course-outline).

Approximately three to five short assignments will be given. Working together on assignments is encouraged, but you are expected to submit original work—not to copy work from other students, past students, solution manuals, etc. Any plagiarized, copied assignment problems, or copied electronic files will not be counted for any student involved. **Late assignments will not be accepted without prior approval.**

### Project

In addition to the shorter assignments, the main focus of the course will be a project that involves developing a new software package targeted at your own research area, and ideally something you would use towards your thesis research. All of the concepts discussed in the class, including testing, documentation, and open sharing of the software will be applied to the project.

## Course Outline

### Class 1: Introduction, Version Control

Lecture slides: <https://softwaredevengresearch.github.io/getting-started/>

1. Introduction to course
    * Discuss what the class is going to cover
    * Everyone introduce themselves
        * Name
        * What you "do"
        * What are your goals for the class?
2. Setup: Git
    * How many people are comfortable with Git/GitHub?
    * Install Git or [GitHub Desktop](https://desktop.github.com/)
        * If you are comfortable with Git already, you can skip this.
    * Sign up for GitHub (if you didn't already)
3. Introduction to local version control via Git

#### Homework

* Join [the chat room](https://gitter.im/SoftwareDevEngResearch/Lobby).
* [Set up your GitHub profile.](https://github.com/settings/profile)
* **Due by Friday 13 April:** project proposal. Please submit this via the [`course-projects` repository](https://github.com/SoftwareDevEngResearch/course-projects) in the GitHub organization (you must have accepted the invitation to the organization), in the `proposals` folder. Name your document `LastName-project-proposal.md`; notice the `.md` file extension, which indicates a Markdown file. ([Markdown](https://guides.github.com/features/mastering-markdown/) is a lightweight plaintext format used commonly for things like READMEs.)
  * Please describe the functionality of your intended software project, including who might use it. This includes what the software will actually do—will it simulate something, process data, or something else?—the overall components you expect to design, and expected inputs/outputs.
  * Most packages should build on some existing methodology, so cite papers as appropriate. Also describe how this builds on any prior work you've done, if relevant. Make it clear how this software package will be different from existing work (yours or otherwise).
  * You should talk about any packages you expect to depend on (if known).
  * It is fine if you plan to develop a graphical user interface for your software package, but that should not be the main or primary contribution.
  * Proposals should be one or two pages long.


## Resources

### Required Reading

* *Effective Computation in Physics*, by Scopatz & Huff, O’Reilly. <http://physics.codes>

### Beginner Materials

This class assumes you are confident with this material, but in case you need a brush-up...

* Codecademy – [Python](https://www.codecademy.com/learn/learn-python)
* see also – [Other Lists](#other-lists)

### Recommended Reading

* [Scipy Lecture Notes](http://www.scipy-lectures.org)

#### Specific Topics

*

#### Other Lists

* [Code School](https://www.codeschool.com/paths/python)
* [Teach Yourself to Code](http://teachyourselftocode.com/python)

### Tools

* debugging:
    *
* sharing code snippets: [gist.github.com](https://gist.github.com/)
* asking questions: [Stack Overflow](http://stackoverflow.com/)

#### GitHub

* Git and GitHub
    * [Official GitHub Help](https://help.github.com/)
    * [Recommended resources](http://hackerhours.org/resources.html#github)
* GitHub Pages
    * [Official site](https://pages.github.com/)
    * [Thinkful guide](http://www.thinkful.com/learn/a-guide-to-using-github-pages/)

### Reference

*

### More Examples

*

## Grading

* Assignments – 40%
* Project – 60%

You are expected to discuss issues or concerns with assignment/project grades with me within one week after a grade is returned.

## Statements on Plagiarism

### Oregon State

> **Academic or Scholarly Dishonesty** is defined as an act of deception in which a Student seeks to claim credit for the work or effort of another person, or uses unauthorized materials or fabricated information in any academic work or research, either through the Student's own efforts or the efforts of another.

For more information about academic integrity and relevant University policies/procedures, please refer to the [Student Conduct web site](http://studentlife.oregonstate.edu/studentconduct) and the [section on Academic Regulations](http://catalog.oregonstate.edu/ChapterDetail.aspx?key=75#Section2883) in the OSU Schedule of Classes. If you have any questions or concerns about this policy, **don't hesitate to contact me**.

### Instructor

It is my expectation that any work submitted for this course is a fair and accurate representation of your own abilities and efforts, or in the case of team work, those of the team. Evidence to the contrary will prompt investigation and any dishonest acts will be dealt with accordingly.

From Aidan Feldman's [Advanced Javascript class](https://advanced-js.github.io/syllabus/):
> Reuse and building upon ideas or code are major parts of modern software development. As a professional programmer you will never write anything from scratch. This class is structured such that all solutions are public. You are encouraged to learn from the work of your peers. I won't hunt down people who are simply copying-and-pasting solutions, because without challenging themselves, they are simply wasting their time and money taking this class.
>
> Please respect the terms of use and/or license of any code you find, and if you reimplement or duplicate an algorithm or code from elsewhere, credit the original source with an inline comment.

## Universal Learning

I am committed to the principle of universal learning. This mean that our classroom, virtual spaces, practices, and interactions should be as inclusive as possible. Mutual respect, civility, and the ability to listen and observe others carefully are crucial to universal learning. Students are expected to follow the Code of Student Conduct: <http://studentlife.oregonstate.edu/sites/studentlife.oregonstate.edu/files/code_of_student_conduct.pdf>

For any student with particular needs:
> Accommodations for students with disabilities are determined and approved by Disability Access Services (DAS). If you, as a student, believe you are eligible for accommodations but have not obtained approval please contact DAS immediately at 541-737-4098 or at <http://ds.oregonstate.edu>. DAS notifies students and faculty members of approved academic accommodations and coordinates implementation of those accommodations. While not required, students and faculty members are encouraged to discuss details of the implementation of individual accommodations.

## Credit

This syllabus website and content is based on Aidan Feldman's [Advanced JavaScript class](https://advanced-js.github.io/syllabus/).
