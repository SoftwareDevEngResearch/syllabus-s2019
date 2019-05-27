---
layout: default
permalink: /
---

# <img src="assets/logo.svg" alt="class logo" class="logo"/> Software Development for Engineering Research syllabus

***If you are a teacher or interested in the design of the course, see the [meta](https://github.com/SoftwareDevEngResearch/syllabus-s2019/blob/gh-pages/meta.md) document.***

* **Course:** ME 599, CRN 57683
* **Instructor:** Kyle Niemeyer, [kyle.niemeyer@oregonstate.edu](mailto:kyle.niemeyer@oregonstate.edu)
* **Need help?**
    * We will use Slack for most communication in the class; log in to the `class-me599-003-sp19` workspace at https://oregonstate.enterprise.slack.com.
    * Look through and create [issues](https://github.com/SoftwareDevEngResearch/syllabus-s2019/issues)
    * [Email](mailto:kyle.niemeyer@oregonstate.edu) for 1-on-1 help, or to set up a time to meet using <https://calendly.com/kyle-niemeyer>. However, messaging through Slack is your best bet.

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

We will dive into topics related to developing research software packages, primarily using Python, following best practices. You will each develop a new package over the course of the term that supports research in your particular area of expertise. Topics covered include:

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
* Introduction to high-performance computing (HPC)

Topics will be demonstrated through live-code examples/slides. Additional exercises will completed in-class.

## Homework/Projects

### Project

The main focus of the course will be a project that involves developing a new software package targeted at your own research area, and ideally something you would use towards your thesis research. All of the concepts discussed in the class, including testing, documentation, and open sharing of the software will be applied to the project.

All assignments will relate to this project in some way, and will be listed here.

#### Project presentation and report

The majority of your grade in this course will be based on your project, and assessed through
a final project presentation given on **June 5** and a final project report due **June 12**.

**Presentation:** The presentations will be ~10 minutes each, with up to 5 minutes for questions and switching to the next person.
The presentation should include motivation for your project, any relevant background/theory, some discussion of
the software design (functionality, modules, dependencies, etc.), results (which may be preliminary),
and conclusions/future work/how this fits into your research.

It doesn't matter to me how you make your presentations---Keynote, PowerPoint, Beamer, reveal.js
(what I've been using for most lectures), whatever. You can use your own laptop, or you can
send me your presentation ahead of time and use mine. I encourage you to treat this like a
(relatively short) conference presentation on your work. Feel free to develop your own presentation
format/style, or use your research group's (if that exists).

**Report:** The report should follow the guidelines described in the [`REPORT_INFO.md`](https://github.com/SoftwareDevEngResearch/course-projects-s2019/blob/master/REPORT-INFO.md) file in the [`course-projects-2019` repo](https://github.com/SoftwareDevEngResearch/course-projects-s2019);
reports should be submitted as PDFs in the `reports` directory there by June 12.

**Project expectations:** By the time of your final report submission, I expect that your projects will
follow the best practices we've discussed in class, including having sufficient tests, using continuous
integration, being shared under an open-source license (unless we've discussed an exception),
being installable as a package by pip and/or conda, having a sane command-line or module interface,
and having some documentation.

### Assignments

Working together on assignments is encouraged, but you are expected to submit original work—not to copy work from other students, past students, solution manuals, etc. Any plagiarized, copied assignment problems, or copied electronic files will not be counted for any student involved. **Late assignments will not be accepted without prior approval.**

#### Week 1:

* Join the [Slack chat room](https://oregonstate.enterprise.slack.com): workspace `class-me599-003-sp19`.
* Sign up for GitHub and [set up your profile.](https://github.com/settings/profile)
* **Due by Friday 12 April:** project proposal. Please submit this via the [`course-projects` repository](https://github.com/SoftwareDevEngResearch/course-projects-s2019) in the GitHub organization (you must have accepted the invitation to the organization), in the `proposals` folder. Name your document `LastName-project-proposal.md`; notice the `.md` file extension, which indicates a Markdown file. ([Markdown](https://guides.github.com/features/mastering-markdown/) is a lightweight plaintext format used commonly for things like READMEs.)
  * **Submission process**: Use the "Create new file" button in the [`proposals` folder via the web interface](https://github.com/SoftwareDevEngResearch/course-projects-s2019/tree/master/proposals) to submit your proposal as a pull request. (The "Upload files" button will not work, since you do not have write permissions for this repository.) Alternatively, you can:
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

#### Weeks 2-3:

Complete by **Wednesday 24 April**:

* Create your project repo
  1. Name your software package, create the repo for your project in the class organization, and fork to your account.
  2. Clone your fork locally
  3. Brainstorm your necessary modules; create the empty files.
  4. Commit and push your work to your fork, then submit to the upstream repo via a pull request.
  5. Notify your code review partner
* Begin writing code and testing it
  1. Create (at minimum) three functions in your first module (more is fine!)
  2. Create edge and interior tests for these functions (make sure they pass!)
  3. Submit your changes as a Pull Request to your upstream repo. I will assign partners to review your PRs.
* Set up continuous integration
  1. Set your project up with Travis CI to run the test suite.
  2. Add comments/docstrings to your code if you haven't already. Revise your code to follow more clear naming practices if needed. Make sure your pull requests pass all your tests!

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

#### Extra reading:

 - [Blog post about relicensing yt from GPL to BSD](https://blog.yt-project.org/post/Relicensing/)

### Lecture 3: Packages and Testing

**Lecture slides:** <https://softwaredevengresearch.github.io/lecture-packaging-testing>

1. Testing your software
    * Importance of testing
    * What and how to test
    * Types of tests
    * using [`pytest`](https://docs.pytest.org/en/latest/) to automate testing
    * Test-Driven Development
2. Structuring (Python) programs
    * Package directory structure
    * Absolute and relative module imports
    * Useful packages in the Python standard library
    * Useful third-party packages for scientific computing

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

### Lecture 5: Classes and Objects (in Python)

**Lecture slides:** <https://softwaredevengresearch.github.io/lecture-classes-objects/>

1. Object oriented programming
2. Objects
3. Classes
  * Instance variables
  * Methods
  * Subclasses and inheritance

### Lecture 6: Files and Command-line Inputs in Python

**Lecture slides:** <https://softwaredevengresearch.github.io/lecture-files-commandline/>

1. Files in Python
  * File handle methods
  * `with` context manager
2. HDF5
  * PyTables
  * Nodes, arrays, tables
3. Command-line interface
  * `argparse`

### Lecture 7: Packaging and Distributing your Software

1. Clarification inheritance of class constructors
2. Brief explanation of `main()` and `__main__`
3. Packaging for pip and PyPI
  * `setup.py`
  * `_version.py`, `CHANGELOG`, and semantic versioning
4. Packaging with conda
5. Advanced deploying with Travis CI

**Lecture slides:** <https://softwaredevengresearch.github.io/lecture-packaging-distribution/>

### Lecture 8: Intro to Parallel Programming

**Lecture slides:** <https://softwaredevengresearch.github.io/lecture-parallel-computing>

1. Basic concepts of parallelism
2. Scale and scalability
3. Parallelism with Python
  * `threading`
  * `multithreading`
4. Brief intro to MPI

### Lecture 9: Optimizing Numerical Code in Python

**Link to video:** ["Performance Python: Seven Strategies for Optimizing Your Numerical Code"](https://www.youtube.com/watch?v=zQeYx87mfyw) by [Jake VanderPlas](http://vanderplas.com)

**Link to notebook:** <https://gist.github.com/jakevdp/256c3ad937af9ec7d4c65a29e5b6d454>

Strategies for optimizing numerical code:

1. Line profiling
2. NumPy
3. Specialized data structures
4. Cython
5. Numba
6. Dask
7. Find an existing implementation

<!---

### Lecture 5: Intro to Julia

Guest lecture from [Prof. Cory Simon](https://simonensemble.github.io).

Introduction to the Julia language, via a live coding demo of a Monte Carlo simulation of Buffon's Needle: https://simonensemble.github.io/2018/04/11/buffon/


### Lecture 11: Open Science, Software Citation, and Reproducibility Best Practices

**Lecture slides:** <https://github.com/SoftwareDevEngResearch/syllabus/blob/gh-pages/lecture-open-citation-repro.pdf>

--->

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

* [Defining main functions in Python](https://realpython.com/python-main-function/)
* NumPy's [`allclose` function](https://docs.scipy.org/doc/numpy/reference/generated/numpy.allclose.html)
* ["Inside the Cheeseshop: How Python Packaging Works" (video)](https://www.youtube.com/watch?v=AQsZsgJ30AE)
* [Python Packaging Guide](https://packaging.python.org)
* ["Beyond Unit Testing: Taking Your Testing to the Next Level (video)"](https://www.youtube.com/watch?v=MYucYon2-lk)
* ["WHAT IS THIS MESS?" - Writing tests for pre-existing code bases" (video)](https://www.youtube.com/watch?v=LDdUuoI_lIg)
* [Faster Python Programs: Measure, Don't Guess (3-hour video tutorial)](https://www.youtube.com/watch?v=DGrS0uwMuHY)
* [Foundations of Numerical Computing in Python (3-hour video tutorial)](https://www.youtube.com/watch?v=aGGbnMyeZs0)

#### Other Lists

* [Code Academy: Python 3](https://www.codecademy.com/learn/learn-python-3)
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

## Academic Honesty

It is my expectation that any work submitted for this course is a fair and accurate representation of your own abilities and efforts, or in the case of team work, those of the team. Evidence to the contrary will prompt investigation and any dishonest acts will be dealt with accordingly.

> **Academic or Scholarly Dishonesty** is defined as an act of deception in which a Student seeks to claim credit for the work or effort of another person, or uses unauthorized materials or fabricated information in any academic work or research, either through the Student's own efforts or the efforts of another.

For more information about academic integrity and relevant University policies/procedures, please refer to the [Student Conduct web site](http://studentlife.oregonstate.edu/studentconduct) and the [section on Academic Regulations](http://catalog.oregonstate.edu/ChapterDetail.aspx?key=75#Section2883) in the OSU Schedule of Classes. If you have any questions or concerns about this policy, **don't hesitate to contact me**.

### More info:

From Aidan Feldman's [Advanced Javascript class](https://advanced-js.github.io/syllabus/):
> Reuse and building upon ideas or code are major parts of modern software development. As a professional programmer you will never write anything from scratch. This class is structured such that all solutions are public. You are encouraged to learn from the work of your peers. I won't hunt down people who are simply copying-and-pasting solutions, because without challenging themselves, they are simply wasting their time and money taking this class.
>
> Please respect the terms of use and/or license of any code you find, and if you reimplement or duplicate an algorithm or code from elsewhere, credit the original source with an inline comment.

## Universal Learning

I am committed to the principle of universal learning. This mean that our classroom, virtual spaces, practices, and interactions should be as inclusive as possible. Mutual respect, civility, and the ability to listen and observe others carefully are crucial to universal learning. Students are expected to follow the Code of Student Conduct: <http://studentlife.oregonstate.edu/sites/studentlife.oregonstate.edu/files/code_of_student_conduct.pdf>

For any student with particular needs:
> Accommodations for students with disabilities are determined and approved by Disability Access Services (DAS). If you, as a student, believe you are eligible for accommodations but have not obtained approval please contact DAS immediately at 541-737-4098 or at <http://ds.oregonstate.edu>. DAS notifies students and faculty members of approved academic accommodations and coordinates implementation of those accommodations. While not required, students and faculty members are encouraged to discuss details of the implementation of individual accommodations.

**Culture of respect:** I believe in the creation and maintenance of a more inclusive, welcoming university that is safe for all students, faculty, and staff. I will provide care and support to community members who may be negatively affected by bias incidents through our Bias Incident Response Process, which is supported by the [OSU Office of Institutional Diversity (OID)](https://diversity.oregonstate.edu/bias-incident-response).

**Basic needs:** Any student who has difficulty affording groceries or accessing sufficient food to eat every day, or who lacks a safe and stable place to live, and believes this may affect their performance in the course, is urged to contact the [OSU Human Services Resource Center (HSRC)](https://studentlife.oregonstate.edu/hsrc/other-resources/osu-basic-needs-statement) for support (541-737-3747, <hsrc@oregonstate.edu>).

**Mental health:** Diminished mental health, including significant stress, mood changes, excessive worry, or problems with eating and/or sleeping can interfere with optimal academic performance. The source of symptoms might be strictly related to your course work; if so, please speak with me. However, problems with relationships, family worries, loss, or a personal struggle or crisis can also contribute to decreased academic performance. [OSU Counseling and Psychological Services (CAPS)](https://counseling.oregonstate.edu) offers free, confidential psychological services to help you manage personal challenges that may threaten your well-being.

## Credit

This syllabus website and content is based on Aidan Feldman's [Advanced JavaScript class](https://advanced-js.github.io/syllabus/).
