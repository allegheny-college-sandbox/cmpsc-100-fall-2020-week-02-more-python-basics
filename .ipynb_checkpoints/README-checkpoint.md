# CMPSC 100: Fall 2020, Week 02

* Distributed: 14 September, 2020
* Due: 24 September, 2020

## Point values

---

|Type         |Point value |
|-------------|------------|
|Worksheets   |10 pts.     |
|Lab          |20 pts.     |
|Participation|15 pts.     |
|             |            |
|Total        |45 pts.     |
|             |4.5% of course |

## Table of contents

For those who just want to get to work, consult the `Instructional Materials` section. Else, for additional summary or context, read the additional sections included.

* [Accepting the assignment](#Accepting-the-assignment)
* [Overview](#Overview)
  * [Evaluation](#Evaluation)
* [Instructional materials](#Instructional-materials)
  * [Worksheets and activities](#Worksheets-and-activities)
  * [Lab](#Lab)
* [More Python basics](#More-Python-basics)
* [Lab activity:](#Lab-activity:)
* [Wrap-up](#Wrap-up)
  * [GatorGrader](#GatorGrader)
  * [Submitting your work](#Submitting-your-work)
  
## Accepting the assignment

---

- [ ] Log into the `#assignments` channel in our class [Slack](https://cmpsc-100-00-fa-2020.slack.com)
- [ ] Click the link provided for the lab assignment and accept it in GitHub classroom
- [ ] Once the assignment finishes building, click the link to go to your personal repository assignment

## "Cloning" a repository

### Using the correct download link

- [ ] On this repository's page, click the `Clone or download` button in the upper right hand corner
* You may need to scroll up to see it
- [ ] In the upper right corner of the box that appears, click `Use SSH`
- [ ] Copy the link that appears in the textbox below the phrase "Use a password with a protected key."

#### Cloning

* [ ] Type `ls` in your terminal window
* You should be in your `~` directory
- [ ] Once there, "clone" the repository using the link copied above
* If I (the instructor) were to clone my own repository, I'd enter (your link will look different):

```
git clone git@github.com:allegheny-college-cmpsc-100-fall-2020/cmpsc-100-fall-2020-week-02-more-python-basics-dluman
```

## Overview

## Evaluation

### Worksheets

* Responses to all questions or blank cells

### Lab 

* See individual [lab guidelines](lab/Week%2002%20-%20Lab%20-%20The%20Catnap%20Caper.ipynb#Requirements)

# Instructional materials

## Worksheets and activities

* [Week 02, Worksheet 0: Data types (booleans)](worksheets/Week%2002%20-%20Worksheet%200%20-%20Syntax%20-%20Data%20Types%20(booleans).ipynb)
* [Week 02, Worksheet 1: `if` statements](worksheets/Week%2002%20-%20Worksheet%201%20-%20Syntax%20-%20if%20statements%20.ipynb)
* [Week 02, Worksheet 2: Python syntax (while loops)]((worksheets/Week%2002%20-%20Worksheet%201%20-%20Syntax%20-%20while%20loops%20.ipynb))

## Lab

* [G. Wiz and the Catnap Caper](lab/Week%2002%20-%20Lab%20-%20The%20Catnap%20Caper.ipynb)

## More Python basics

We're 100% experts about syntax, right?

Well, not quite yet. There are still a few constructs we haven't seen. Storing items in variables and manipulating memory is fun for a while, but eventually even that strong magic wears off. One question you've probably had at least some awareness of in the dark corner of the night is "what exactly do we do with this stuff?"

This week, we're going to learn _some_ of the things you can do. This is the equivalent of learning a bit about how a car works, then driving one for the first time. There are some rules of the road.

## More on syntax

Our first worksheet invites us to learn about `booleans` (no ghosts here, I promise). This data type allows us to judge the relative "truthiness" of an expression in order to understand its relationship to other values or variables. The `boolean` enables us to do many things, including use the other two constructs we learn about in this week's assignments.

* [Week 02, Worksheet 0: Data types (booleans)](worksheets/Week%2002%20-%20Worksheet%200%20-%20Syntax%20-%20Data%20Types%20(booleans).ipynb)

The `if` statement lives somewhere between philosophy, formal logic, and computer science. Giving us the ability to "branch" our code based on `boolean` skills, we'll use `if` statements to explore what happens when a value is `True` or `False`. In addition, we'll learn a bit about the idea of the "flow of control."

* [Week 02, Worksheet 1: `if` statements](worksheets/Week%2002%20-%20Worksheet%201%20-%20Syntax%20-%20if%20statements%20.ipynb)

In certain cases, if a statement is true, we should continue doing something until either the statement become false or some other information should cause us to stop. Eventually we'll combine our `if` statement and `boolean` skills (along with a new function -- `input`) to make this all worth our `while`.

* [Week 02, Worksheet 2: Python syntax (while loops)]((worksheets/Week%2002%20-%20Worksheet%201%20-%20Syntax%20-%20while%20loops%20.ipynb))

# Lab activity: G. Wiz and the Catnap Caper

* [G. Wiz and the Catnap Caper](lab/Week%2002%20-%20Lab%20-%20The%20Catnap%20Caper.ipynb)

## Wrap-up

---

### GatorGrader

GatorGrader is an Allegheny College-developed, student-written and maintained application that grades your work for you. The long and short of it, before and when you turn in your assignments, you can know what your approximate grade will be.

(It doesn't do _everything_ for us, but it gives us a good starting point for evaluating your work.)

You don't need to do anything to get it -- I will distribute all the files you need with every repository. You realize the following benefits:

* Complete grading transparency
* Grading criteria _never_ changes
* The criteria is very specific; you will know what changes you need to make

This application runs in your terminal tab, and can grade:

* The whole repository
* Just worksheets
* Just the lab

## Checking your work

---

No matter where you are in your repository, the command to start and run GatorGrader is always the same:

```
gradle grade
```

However, you need to be _in the right place_ to get the right result. The following table summarizes the various grading locations.

| Location | Grading             |
|----------|---------------------|
| Root folder | Repository requirements |
| `worksheets/` | Worksheet requirements |
| `lab/`        | Lab requirements |

### Submitting the assignment/saving progress

The GitHub platform is a place to store your work. So, it makes some sense that should be able to _clone_ (download) from it, and push back (upload) to it. Here, we'll learn this second part.

- [ ] `cd` to your `~` folder
- [ ] Locate the `cmpsc-100-fall-2020-week-01-python-basiscs` folder and `cd` to it.

Once in this folder, we need to tell git that there have been changes.

- [ ] Type `git add .` and press `Enter`
* This tells git to look through the _entire_ folder structure for new changes and "stage" them

- [ ] Type `git commit -m "{Commit message}"` to "label" the commit
* This is typically something like `git commit -m "Fixing a typo"` -- the message in quotes should be as descriptive as possible, while still remaining somewhat short

- [ ] To send all changes to the server, type `git push`
- [ ] At the prompt, input the password associated with the `SSH Key` you created earlier in this exercise (yesterday)

Once the process finishes successfully, we're done!

#### A strong warning

<div class="alert alert-block alert-danger">
    <p><strong>While we may use this server to store code, <u>you</u> are responsible for using GitHub as your main backup.</strong></p>
    <p>While I back this server up on a regular basis, I cannot guarantee that I'll have the ability to restore up-to-the-minute data for your work.</p>
    <p>Remember: to err is human; to back up your work is divine.</p>
</div>