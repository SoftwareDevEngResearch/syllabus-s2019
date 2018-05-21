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

### Lecture 1: Introduction, Version Control

**Lecture slides:** <https://softwaredevengresearch.github.io/getting-started/>

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
  * **Submission process**: Use the "Create new file" button in the [`proposals` folder via the web interface](https://github.com/SoftwareDevEngResearch/course-projects/tree/master/proposals) to submit your proposal as a pull request. (The "Upload files" button will not work, since you do not have write permissions for this repository.) Alternatively, you can:
    1. Fork the repo into your own account (use the "Fork" button)
    2. Clone a local copy to your computer
    3. Add the file in the proposals folder, and commit this addition
    4. Push the change to your version of the repo (`git push`)
    5. On your repo at GitHub, submit a new pull request back to the original “upstream” repo.
  * Please describe the functionality of your intended software project, including who might use it. This includes what the software will actually do—will it simulate something, process data, or something else?—the overall components you expect to design, and expected inputs/outputs.
  * Most packages should build on some existing methodology, so cite papers as appropriate. Also describe how this builds on any prior work you've done, if relevant. Make it clear how this software package will be different from existing work (yours or otherwise).
  * You should talk about any packages you expect to depend on (if known).
  * It is fine if you plan to develop a graphical user interface for your software package, but that should not be the main or primary contribution.
  * Proposals should be one or two pages long.

### Lecture 2: Remote Version Control, Licensing & Copyright

**Lecture slides:** <https://softwaredevengresearch.github.io/remote-version-control>

1. Introduction to GitHub and remote version control
    * Creating a repo
    * Cloning, pushing, fetching, merging, and pulling
    * Pull Requests and working on projects collaboratively
2. Copyright & Software Licensing
    * Copyright basics (I Am Not A Lawyer)
    * Types of Software Licenses
    * Creative Commons
    * Other Intellectual Property issues

### Lecture 3: Packages and Testing

**Lecture slides:** <https://softwaredevengresearch.github.io/lecture-packaging-testing>

1. Structuring (Python) programs
    * Package directory structure
    * Absolute and relative module imports
    * Useful packages in the Python standard library
    * Useful third-party packages for scientific computing
2. In class activity:
    * create the repo for your project in the class organization, and fork to your account.
    * Clone it locally
    * Brainstorm your necessary modules; create the empty files.
    * Commit and push your work, then submit to the upstream fork.
3. Testing your software
    * Importance of testing
    * What and how to test
    * Types of tests
    * using [`pytest`](https://docs.pytest.org/en/latest/) to automate testing
    * Test-Driven Development

#### Homework

1. Create (at minimum) three functions in your first module (more is fine!)
2. Create edge and interior tests for these functions (make sure they pass!)
3. By Monday, submit your changes as a Pull Request to your upstream repo. I will assign partners to review your PRs.

### Lecture 4: Test Coverage, Continuous Integration, and Documentation

**Lecture slides:** <https://softwaredevengresearch.github.io/lecture-CI-documentation>

1. Test coverage
    * Using `pytest-cov`
2. Continuous integration
    * Using Travis CI
3. Documentation
    * Value of documentation
    * Types of documentation
    * Comments
    * Self-documenting code
    * Docstrings

#### Homework

For Monday 30 April:
1. Set your project up with Travis CI to run the test suite (may have been completed in class)
2. Add comments/docstrings to your code if you haven't already. Revise your code to follow more clear naming practices if needed. Make sure your pull requests pass all your tests!
3. Continue developing your software projects

### Lecture 5: Intro to Julia

Guest lecture from [Prof. Cory Simon](https://simonensemble.github.io).

Introduction to the Julia language, via a live coding demo of a Monte Carlo simulation of Buffon's Needle: https://simonensemble.github.io/2018/04/11/buffon/

### Lecture 6: Intro to Parallel Programming

**Lecture slides:** <https://softwaredevengresearch.github.io/lecture-parallel-computing>

### Lecture 7: Classes and Objects (in Python)

**Lecture slides:** <https://softwaredevengresearch.github.io/lecture-classes-objects/>

### Lecture 8: Packaging and Distributing your Software

**Lecture slides:** <https://softwaredevengresearch.github.io/lecture-packaging-distribution/>

### Lecture 9: Optimizing Numerical Code in Python

Link to video: ["Performance Python: Seven Strategies for Optimizing Your Numerical Code"](https://www.youtube.com/watch?v=zQeYx87mfyw) by [Jake VanderPlas](http://vanderplas.com)

Link to Jupyter notebook: <https://gist.github.com/jakevdp/256c3ad937af9ec7d4c65a29e5b6d454>

### Lecture 10: Files and Command-line Inputs in Python

**Lecture slides:** <https://softwaredevengresearch.github.io/lecture-files-commandline/>

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

* NumPy's [`allclose` function](https://docs.scipy.org/doc/numpy/reference/generated/numpy.allclose.html)
* ["Inside the Cheeseshop: How Python Packaging Works" (video)](https://www.youtube.com/watch?v=AQsZsgJ30AE)
* [Python Packaging Guide](https://packaging.python.org)
* ["Beyond Unit Testing: Taking Your Testing to the Next Level (video)"](https://www.youtube.com/watch?v=MYucYon2-lk)
* ["WHAT IS THIS MESS?" - Writing tests for pre-existing code bases" (video)](https://www.youtube.com/watch?v=LDdUuoI_lIg)
* [Faster Python Programs: Measure, Don't Guess (3-hour video tutorial)](https://www.youtube.com/watch?v=DGrS0uwMuHY)
* [Foundations of Numerical Computing in Python (3-hour video tutorial)](https://www.youtube.com/watch?v=aGGbnMyeZs0)

#### Other Lists

* [Code School](https://www.codeschool.com/paths/python)
* [Teach Yourself to Code](http://teachyourselftocode.com/python)

### Tools

* sharing code snippets: [gist.github.com](https://gist.github.com/)
* asking questions: [Stack Overflow](http://stackoverflow.com/)

#### GitHub

* Git and GitHub
    * [Official GitHub Help](https://help.github.com/)
    * [Recommended resources](http://hackerhours.org/resources.html#github)
* GitHub Pages
    * [Official site](https://pages.github.com/)
    * [Thinkful guide](http://www.thinkful.com/learn/a-guide-to-using-github-pages/)

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
