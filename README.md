0x06. Python - Classes and Objects
==================================

-   By Guillaume

#### In a nutshell...

Concepts
------------------
*For this project, students are expected to look at these concepts:*

-   [Source code management](https://intranet.hbtn.io/concepts/22)
-   [Git and Github cheat sheet - Everything in less than 30 seconds](https://intranet.hbtn.io/concepts/57)
-   [The Framework](https://intranet.hbtn.io/concepts/75)
-   [Approaching a Project](https://intranet.hbtn.io/concepts/350)

Resources
---------

**Read or watch**:
-   [Resources to learn Git](https://intranet.hbtn.io/rltoken/rOOPwBFp4ezRunQ0G0YHYQ)
-   [About READMEs](https://intranet.hbtn.io/rltoken/4CwCa3MmQvJfXu5poTRVQw)
-   [How to write a Git commit message](https://intranet.hbtn.io/rltoken/zkdCE4WEr9H91WlOpfNlGA)
**Resources for advanced tasks**(Read only after finishing the mandatory tasks):
-   [Learning branching](https://intranet.hbtn.io/rltoken/514Jj2WL9uL6wOyOYWejdA)
-   [Effective pull requests and other good practices for teams using GitHub](https://intranet.hbtn.io/rltoken/ZUE0eoAWDKadJd4QCQkzQg)

Learning Objectives
-------------------

At the end of this project, you are expected to be able to [explain to anyone](https://alx-intranet.hbtn.io/rltoken/Hca4-cCJg_1lKwC4ij6Z0g "explain to anyone"), **without the help of Google**:

### General

-   What is source code management
-   What is Git
-   What is GitHub
-   What is the difference between Git and GitHub
-   How to create a repository
-   What is a README
-   How to write good READMEs
-   How to commit
-   How to write helpful commit messages
-   How to push code
-   How to pull updates
-   How to create a branch
-   How to merge branches
-   How to work as collaborators on a project
-   Which files should and which files should not appear in your repo

Requirements
------------

### General

-   A `README.md` file at the root of the repo, containing a description of the repository
-   A `README.md` file, at the root of the folder of *this* project (i.e. `0x03-git`), describing what this project is about
-   **Do not use GitHub's web UI**, but the command line to perform the exercise (except for operations that can not possibly be done any other way than through the web UI). You won't be able to perform many of the task requirements on the web UI, and you should start getting used to the command line for simple tasks because many complex tasks can only be done via the command line.
-   Your answer files should only contain the command, and nothing else

More Info
---------

### Install `git`

If `git` is not already installed on your terminal:

```
$ sudo apt-get update
$ sudo apt-get upgrade
$ sudo apt-get install git

```

### Basic usage

At the end of this project you should be able to reproduce and understand these command lines:

```
$ git clone <repo>
$ touch test
$ git add test
$ git commit -m "Initial commit"
$ git push origin main

```
### 0\. Create and setup your Git and GitHub account
mandatory

You will need Git for this project, you might have to [install it](https://alx-intranet.hbtn.io/rltoken/7kPsched1VMPOY2bdvZvGQ "install it") on your computer if it's not done yet.

-   Configure your basic info (name, email) on your local machine -- they will be part of your commits. [Tips](https://alx-intranet.hbtn.io/rltoken/oAAqmPJ1ftZZhUjaw7FvjA "Tips")

On [GitHub.com](https://alx-intranet.hbtn.io/rltoken/4vp5Qze3WATHKtytzT2_UA "GitHub.com"):

-   Using the graphic interface on the website, create the repository (if it's not done yet)
    -   Description: `This is my first repository as a full-stack engineer`
    -   Public repo: `zero_day`
    -   No `README`, `.gitignore`, or license

On your computer, open a terminal and do the following:

-   Navigate to your home directory. [Tips](https://alx-intranet.hbtn.io/rltoken/YeOwsN-vhfSCbNjgE01Gag "Tips")
-   Create a directory `zero_day`. [Tips](https://alx-intranet.hbtn.io/rltoken/hWrqqlilEv8L6yqpyt1TTA "Tips")
-   Navigate to this new directory. [Tips](https://alx-intranet.hbtn.io/rltoken/za58mq537U6U775osQ8bfQ "Tips")
-   Initialize git and add the remote origin
-   Create a file `README.md` with Emacs (or other command line editors) and write a small [Markdown](https://alx-intranet.hbtn.io/rltoken/VV79mKOEf5mXVbKpH4i63Q "Markdown") text to present this project. **This file is mandatory in projects**
-   Add this new file to git, commit the change with this message "My first commit" and push to the remote server / origin (Note: You will probably need to set your login/password to push to the remote server)

Good job!

You pushed your first file in your **first repository** of the **first task** of your **first School project**.

**Repo:**

-   GitHub repository: `zero_day`
-   File: `README.md`

### 1\. Repo-session
mandatory

-   Create a new directory called `0x03-git` in your `zero_day` repo.

Make sure you include a not empty `README.md` in your directory:

-   at the root of your repository `zero_day`
-   AND in the directory `0x03-git`

And important part: **Make sure your commit and push your code to Github - otherwise the Checker will always fail.**

**Repo:**

-   GitHub repository: `zero_day`

For the moment we have an empty project directory containing only a README.md. It’s time to code!

### 2\. Coding fury road
mandatory

-   Create these directories at the root of your project: `bash`, `c`, `js`
-   Create these empty files:
`c/c_is_fun.c`
`js/main.js`
`js/index.js`
-   Create a file `bash/best` with these two lines inside: `#!/bin/bash` and `echo "Best"`
-   Create a file `bash/school` with these two lines inside: `#!/bin/bash` and `echo "School"`
-   Add all these new files to git
-   Commit your changes (message: “Starting to code today, so cool”) and push to the remote server

**Repo:**

-   GitHub repository: `zero_day`
-   Directory: `0x03-git`
-   File: `bash/best`, `bash/school`, `c/c_is_fun.c`, `js/main.js`, `js/index.js`

### 3\. Collaboration is the base of a company
mandatory

A branch is like a copy of your project. It’s used mainly for:

-   adding a feature in development
-   collaborating on the same project with other developers
-   not breaking your entire repository
-   not upsetting your co-workers
The purpose of a branch is to isolate your work from the main code base of your project and/or from your co-workers’ work.

For this project, create a branch `update_script` and in this branch:

-   Create an empty file named `bash/98`
-   Update `bash/best` by replacing `echo "Best"` with `echo "Best School"`
-   Update `bash/school` by replacing `echo "School"` with `echo "The school is open!"`
-   Add and commit these changes (message: “My personal work”)
-   Push this new branch [Tips](https://intranet.hbtn.io/rltoken/w-vaOsoyqzITnQQ2NoSf6g)
Perfect! You did an amazing update in your project and it’s isolated correctly from the **main** branch.

Ho wait, your manager needs a quick fix in your project and it needs to be deployed now:

-   Change branch to `main`
-   Update the file `bash/best` by replacing `echo "Best"` with `echo "This -   School is so cool!"`
-   Delete the directory `js`
-   Commit your changes (message: “Hot fix”) and push to the origin
Ouf, hot fix is done!

**Repo:**

-   GitHub repository: `zero_day`
-   Directory: `0x03-git`
-   File: `bash/best`, `bash/school`, `bash/98`

### 4\. Collaboration: be up to date
mandatory

Of course, you can also work on the same branch as your co-workers and it’s best if you keep up to date with their changes.

For this task – **and only for this task** – please update your file `README.md` in the main branch from GitHub.com. It’s the **only time** you are allowed to update and commit from GitHub interface.

After you have done that, in your terminal:

-   Get all changes of the main branch locally (i.e. your `README.md` file will be updated)
-   Create a new `file up_to_date` at the root of your directory and in it, write the git command line used
-   Add `up_to_date` to git, commit (message: “How to be up to date in git”), and push to the origin

**Repo:**

-   GitHub repository: `zero_day`
-   Directory: `0x03-git`
-   File: `README.md`, `up_to_date`

### 5\. HAAA what did you do???
mandatory

Collaboration is cool, but not really when you update the same file at the same time…

To illustrate that, please merge the branch `update_script` to `main`: “Cool, all my changes will be now part of the main branch, ready to be deployed!”

**HHHHHHHAAAAAAAA***

```
CONFLICT (content): Merge conflict in bash/best
```
As you can see, you have conflicts between two branches on the same file.

Your goal now is to resolve conflicts by using the version of the branch `update_script`, and push the result to the origin.

At the end, you should have all your work from the branch `update_script` (new file and two updated files) and all latest `main` commits (new files, delete folder, etc.), without conflicts.

**Repo:**

-   GitHub repository: `zero_day`
-   Directory: `0x03-git`

### 6\. Never push too much
mandatory

Create a `.gitignore` file and define a rule to never push `~` files (generated by Emacs). [Tips](https://intranet.hbtn.io/rltoken/0ANsyvhObT_TYAToY8-lbA)

**Repo:**

-   GitHub repository: `zero_day`
-   Directory: `0x03-git`
-   File: `.gitignore`
