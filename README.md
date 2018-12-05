# Reusability and reproducibility for bioinformatics analyses

<img align="right" src=../../../20181003_Intro_git_GitHub/blob/master/images/github_icon.png width="225">

## Introduction to version control using GitHub

- Date and time: 7th December 2018, 14:00 - 15:30
- Location: [Bioinformatics Training Facility](http://map.cam.ac.uk/Craik-Marshall+Building), University of Cambridge, UK
- [Programme](https://e.issuu.com/anonymous-embed.html?u=bioinfocambs&d=bioinformaticsforbiologists_dec2018)
- Trainers: [Sergio](https://github.com/semacu) and [Mark](https://github.com/mfernandes61)


## Overview

Have you ever wondered how to keep automatic control of the different versions of your research documents, computer scripts and data sets? In this session we will learn the basics of Git and GitHub so that you can then develop version control for your own research projects.

- [Background and motivation](README.md#background-and-motivation)
- [What is version control? What is Git? What is GitHub?](README.md#what-is-version-control-what-is-git-what-is-github)
- [How can you use Git and GitHub? How can they be useful for you?](README.md#how-can-you-use-git-and-github-how-can-they-be-useful-for-you)
- [Practical session: working with Git and GitHub](README.md#practical-session-working-with-git-and-github)


## Background and motivation

- When reproducing someone's previous work (or your own past work), researchers very often benefit greatly from having access to detailed documention of the methods used e.g. how were the experiments done? How were the computational analyses performed?

- In many cases you don't only want to see a single static version of the project but may want to have access / keep track of the different versions of the project e.g. how did the project looked like 1 year ago?

- Some of the existing manual approaches to version control have **clear limitations**:

<p align="center">
<img src=../../../20171024_GitHub_Chemistry_Cambridge/blob/master/images/finaldoc.gif width="600">
</p>

<p align="right">
(http://phdcomics.com/comics/archive_print.php?comicid=1531)
</p>

- In the context of bioinformatics scripts and software, the scientific community is beginning to consider the value of peer reviewing computer code - see Nature Methods August 2018 editorial [**Easing the burden of code review**](https://www.nature.com/articles/s41592-018-0137-5):

*An increasing share of modern research relies on analytical code and software. In turn, a good deal of irreproducible research can be attributed to computational tools that are difficult to decipher, use or recreate. Through the concerted efforts of computational researchers and stricter guidelines from publishers, the culture of scientific software is now more open and geared toward dissemination than ever [...]*

- Git and GitHub are some of best-known tools for releasing / sharing / version control the scripts and computer code developed as part of a project or manuscript.


## What is version control? What is Git? What is GitHub?

[**Version control**](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control) is the management of *changes* (a.k.a. *revisions*) to any types of information
  - In its simplest form, creating copies and changing the scripts' file names, e.g. v1.0, v1.1, v2.0
  - Using tools that (to some extent) incorporate version control functionality, e.g. Google Drive and Dropbox
  - Using dedicated version control tools, e.g. Git

The first version control systems were created by groups writing software and code - see development of the Linux operating system. Fortunately they can now be used not only by computer scientist for developing computer code but by anyone for any file type :smile:

There are two types of version control systems:

<p align="center">
<img src=../../../20171024_GitHub_Chemistry_Cambridge/blob/master/images/vcs.png width="800">
</p>

<p align="right">
(adapted from http://lhzuigao.com/309note.html)
</p>

Advantages of *distributed* (right) over *centralised* (left) version control systems include:

  - If the central repository (server) crashes, it could be recovered / backed up from any of the local repositories created e.g. by the researcher, collaborator or group leader.
  - Each person can make changes to their local repositories *offline*. Then integrate their individual changes in the central repository (server) when connected *online*.


[**Git**](https://git-scm.com) is a *distributed* version control system to keep track and compare the history of *changes* made to your scripts and files. It allows groups of people to work on the same documents at the same time, and without stepping on each other's toes. It was created by Linus Torvalds in 2005 for the development of the Linux project. It is **free** and **open source** and helps you with:
  - Creating repositories to host your projects using the [command-line](https://en.wikipedia.org/wiki/Command-line_interface)
  - Tracking changes to the files and folders within your repositories


[**GitHub**](https://github.com/) is a platform to share and showcase your work online with collaborators and the wider audience. A tool to help you build projects that are collaborative, well documented, and version-controlled. It provides you with:
  - A place to host and backup your repositories online
  - A nice web interface to your repositories
  - A strategy to collaborate with colleagues

Versions in Git and GitHub are identified by a *revision number*, e.g. 60363b1, also known as *commit*. Each revision is associated with a *timestamp* and the *person* making the change. Revisions can be **compared**, **restored**, and with some types of files, **merged**.

There are other softwares for version control similar to Git, e.g. [svn](https://en.wikipedia.org/wiki/Apache_Subversion). Similarly, there are other online platforms similar to GitHub to share and collaborate code, e.g. [GitLab](https://about.gitlab.com/).


