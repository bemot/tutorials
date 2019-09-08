Use GitHub to work with MAgPIE
================
Kristine Karstens (<karstens@pik-potsdam.de>)
08 September, 2019

-   [1 Introduction](#introduction)
    -   [Learning objectives](#learning-objectives)
-   [2 GitHub workflow for magpiemodel](#github-workflow-for-magpiemodel)
-   [3 Start to code yourself](#start-to-code-yourself)

1 Introduction
==============

MAgPIE is published as open source software on GitHub. Hence we invite all interested people to understand but also develop the code. Since their are various workflows, how to use GitHub for collaborative software development, we want to give some general remarks on our prefered one. Note the following:

-   **Git** is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency (from: <https://git-scm.com/> - very good help, documentation, tutorial page for git).

-   **GitHub** is an American company (owned by Microsoft) that provides hosting for software development version control using Git. (GitLab, SourceForge and various more are open-source alternatives to GitHub.)

### Learning objectives

The goal of this exercise is to set up MAgPIE for collabrative working. After completion of this exercise, you'll be able to:

1.  Fork and update MAgPIE from/with upstream repository.
2.  Understand the basic workflow including pull requests.
3.  Have heard some very basic git commands and know where to find more help.

2 GitHub workflow for magpiemodel
=================================

<img src="figures/github_workflow.png" width="100%" style="display: block; margin: auto;" />

Every code development (even bugfixes) will be merged into our main repository under <https://github.com/magpiemodel/magpie> with the help of so called pull requests. Pull request gives us control over the changes entering our branches. To create a pull request, we use personal or institutional forks. They have to be kept up-to-date with our upstream repository (the original magpiemodel fork).

> **Exercise**: Visit us on <https://github.com/magpiemodel/magpie> and create your own fork by clicking at 'fork' (at the upper right).

It is basically possible to change the code just using the GitHub interface, but since you want to test and run your code locally you have to clone the repository from your fork anyway. This can be done using the 'https' or 'ssh' adresse of your fork together with the `git clone` command (cmd/bash/GUI) at your machine. We recommand to upload a ssh-key and use ssh to connect to GitHub.

> **Exercise**: Visit your fork and clone the repository at your machine.

To keep your fork up-to-date with the upstream repository you can use the GitHub interface. Via `Compare` you are able to look, if the upstream is some commits ahead and if so merge this new changes into your fork. If you feel familiar with git, you also can do this merging procedure by adding both your fork and the upstream repository as so called 'remotes' to your local repository.

> **Exercise**: Check, if there is anything to merge from the upstream repository into your fork. If so, merge it into your fork.

3 Start to code yourself
========================

When you start making your first changes to the code at your local copy, we strongly recommend to do a tutorial to get familiar with the basic commands in git. You can also have a look on 'git cheat sheets' like <https://about.gitlab.com/images/press/git-cheat-sheet.pdf>.

Here we just want to draw your attention to the various working areas of the git workflow.

<img src="figures/git_basics.png" width="100%" style="display: block; margin: auto;" />

Git wil help you not only to push changes to your remote repositories to version control them, you will also locally controll your development steps:

-   When you introduce changes at your working directory, you can mark your changes by `git add`-ing them to your 'staging area'.

-   After you have collected all your changes for your next commit, you will `git commit` them to your local version history.

-   When you `git push` your changes to your remote repository, you will see them finally at your forks GitHub-page.

-   Now you can do a `pull request`.
