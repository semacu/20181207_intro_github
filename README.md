# Reusability and reproducibility for bioinformatics analyses

<img align="right" src=../../../20181003_Intro_git_GitHub/blob/master/images/github_icon.png width="225">

## Introduction to version control using GitHub

- Date and time: 7th December 2018, 14:00 - 15:30
- Location: [Bioinformatics Training Facility](http://map.cam.ac.uk/Craik-Marshall+Building), University of Cambridge, UK
- [Programme](https://e.issuu.com/anonymous-embed.html?u=bioinfocambs&d=bioinformaticsforbiologists_dec2018)
- Trainers: [Sergio](https://github.com/semacu) and [Mark](https://github.com/mfernandes61)
- Short url: https://tinyurl.com/2018gitbio



## Overview

Have you ever wondered how to keep automatic control of the different versions of your research documents, computer scripts and data sets? In this session we will learn the basics of Git and GitHub so that you can then develop version control for your own research projects.

- [Background and motivation](README.md#background-and-motivation)
- [What is version control? What is Git? What is GitHub?](README.md#what-is-version-control-what-is-git-what-is-github)
- [How can you use Git and GitHub? How can they be useful for you?](README.md#how-can-you-use-git-and-github-how-can-they-be-useful-for-you)
- [Practical session: working with Git and GitHub](README.md#practical-session-working-with-git-and-github)



## Background and motivation

- When reproducing someone's previous work (or your own past work), researchers very often benefit greatly from having access to detailed documention of the methods used e.g. *how were the experiments done? How were the computational analyses performed?*

- In many cases you may not only want to see a single static version of your project but have access / keep track of the different versions during its development e.g. *at which stage was the project 1 year ago?*

- Some of the existing manual approaches to version control have **some clear limitations**:

<p align="center">
<img src=../../../20171024_GitHub_Chemistry_Cambridge/blob/master/images/finaldoc.gif width="400">
</p>

<p align="right">
(http://phdcomics.com/comics/archive_print.php?comicid=1531)
</p>

- In the context of bioinformatics scripts and software, the scientific community is beginning to consider the value of peer reviewing computer code - see Nature Methods August 2018 editorial [**Easing the burden of code review**](https://www.nature.com/articles/s41592-018-0137-5):

*An increasing share of modern research relies on analytical code and software. In turn, a good deal of irreproducible research can be attributed to computational tools that are difficult to decipher, use or recreate. Through the concerted efforts of computational researchers and stricter guidelines from publishers, the culture of scientific software is now more open and geared toward dissemination than ever [...]*

- Git and GitHub are some of the best-known tools for releasing / sharing / version control the scripts and computer code developed as part of a project or manuscript.



## What is version control? What is Git? What is GitHub?

[**Version control**](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control) is the management of *changes* (a.k.a. *revisions*) to any types of information
  - In its simplest form, creating copies and changing the scripts' file names, e.g. v1.0, v1.1, v2.0
  - Using tools that (to some extent) incorporate version control functionality, e.g. Google Drive and Dropbox
  - Using dedicated version control tools, e.g. Git

The first version control systems were created by groups writing software and code. Fortunately, they can now be used not only by computer scientists (for developing computer code) but by anyone (for any type of file) :smile:

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



## How can you use Git and GitHub? How can they be useful for you?

The interfaces to Git and GitHub are:

- Via the command-line using *git*

<p align="center">
<img src=../../../20171024_GitHub_Chemistry_Cambridge/blob/master/images/git_commandline.png width="600">
</p>

- Directly [online](http://github.com/)

<p align="center">
<img src=../../../20171024_GitHub_Chemistry_Cambridge/blob/master/images/github_online.png width="800">
</p>

- Github [Desktop](https://desktop.github.com/) (available for Mac and Windows)

<p align="center">
<img src=../../../20171024_GitHub_Chemistry_Cambridge/blob/master/images/github_desktop.png width="800">
</p>

<p align="right">
(https://programminghistorian.org/lessons/getting-started-with-github-desktop)
</p>

For this workshop, we will use git commands and GitHub's online interface.


### Examples

- To host and share your research outputs and software
  - Laboratories sharing own research e.g. the [Jefferis](https://github.com/jefferislab) or [Balasubramanian](https://github.com/sblab-bioinformatics) groups
  - Software source codes e.g. [BWA](https://github.com/lh3/bwa), an aligner of DNA sequences to reference genomes, and [PIDGIN](https://github.com/lhm30/PIDGINv2), and algorithm to predict protein targets for drug-like molecules
  - Or even to share slides - see Bérénice Batut [work](https://bebatut-slides.github.io/backofen_lab_retreat_04_17/#/) and Stephen J. Eglen [slides](https://github.com/sje30/2018-12-07-rmd)

- To create websites using [GitHub pages]((https://pages.github.com/))
  - Personal research websites, e.g. [Mike Love site](http://mikelove.github.io/)
  - Courses and activities, e.g.
    - [A Friendly Introduction to GitHub](https://kirstiejane.github.io/friendly-github-intro/)
    - [Statistics course in the University of British Columbia](http://stat545.com/index.html)

- To share the contents of a book, e.g. [Bioinformatics Data Skills](https://github.com/vsbuffalo/bds-files) or [Happy Git and GitHub for the R user](http://happygitwithr.com/)

- To write a PhD thesis, e.g. [A reasoning framework for C4 photosynthesis research based on high-throughput analysis](http://rik.smith-unna.com/phd/thesis.html)

- To change the [law](https://arstechnica.com/tech-policy/2018/11/how-i-changed-the-law-with-a-github-pull-request/?utm_source=The+Week+in+Data+mailing+list&utm_campaign=b629363b0d-TheWeekinData16Feb2018_COPY_01&utm_medium=email&utm_term=0_3391a19d97-b629363b0d-101334857&mc_cid=b629363b0d&mc_eid=56501d149f)


### In the context of our research group

- Communication is key as most projects have both experimental and computational leaders
- Building from the classical ways of sharing - conversations/meetings, email, Dropbox, shared folders ... we want to build an environment where:
  - Computational colleagues can share code, figures and tables. Review others work and get credit from their collaborative work
  - Experimental colleagues can follow computational developments, access results and learn methods of data analysis

- And ideally avoiding situations like ...

<p align="center">
<img src=../../../20171024_GitHub_Chemistry_Cambridge/blob/master/images/reproducibility.gif width="800">
</p>

<p align="right">
(http://phdcomics.com/comics.php?f=1689)
</p>

- Parhaps a happier lifetime for a research project:

<p align="center">
<img src=../../../20171024_GitHub_Chemistry_Cambridge/blob/master/images/project_timeline.png width="800">
</p>

<p align="right">
(https://github.com/semacu/20170703_GitHubintheLab_CRUK-CI)
</p>


### Public (free) and private repositories

If you want to start creating repositories in GitHub, your first need to open an account:

- Public repositories are free, and can be browsed and downloaded by anyone
- Private repositories have associated costs - see [pricing of plans](https://github.com/pricing). The developer plan costs $7/month but it is free if you are [a student or an academic](https://education.github.com/pack)

Alternatively, [GitLab](https://about.gitlab.com/) uses a different business strategy with free private repositories and cost plans for public ones. There are other alternatives e.g. [Bitbucket](https://bitbucket.org/).


### Markdown

- GitHub uses Markdown for text edition, a language with plain text formatting syntax (bold, italics, checkboxes, lists, etc.), to render pages online (like HTML but easier). You can use this syntax in text files (.md), commit messages, issues, blog posts, and more.

- Markdown is important because GitHub automatically renders anything written in Markdown. This can be specific files (eg: README), or your comments and issues.

- Some examples of Markdown syntax are available [here](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet).



## Practical session: working with Git and GitHub

We have four possible tutorials:

- [Create a GitHub account](README.md#create-a-github-account) (+)
- [Create your first repository](README.md#create-your-first-repository) (+)
- [Explore your first repository and GitHub account](README.md#explore-your-first-repository-and-github-account) (++)
- [Making changes using Git in the command-line](README.md#making-changes-using-git-in-the-command-line) (+++)
- ... and some [extras](README.md#extras)


### Create a GitHub account

If you don't have a GitHub account already:

- Go to https://github.com
- Fill in your **Username**, **Email** and **Password**. Then click on the green button "Sign up for GitHub".

<p align="center">
<img src=../../../20171024_GitHub_Chemistry_Cambridge/blob/master/images/p1_1.png width="800">
</p>

- Choose your personal plan page. Select "Free plan" and then click on "Continue".

<p align="center">
<img src=../../../20171024_GitHub_Chemistry_Cambridge/blob/master/images/p1_2.png width="800">
</p>

- Tailor your experience page. Choose the boxes that apply to you and click on "Submit". Otherwise, just go to "skip this step".

<p align="center">
<img src=../../../20171024_GitHub_Chemistry_Cambridge/blob/master/images/p1_3.png width="800">
</p>

- You have created a GitHub account! :smile:



### Create your first repository

- If you are not already signed in, sign in to GitHub using the **Username/Email** and **Password** created before.
- Click on the top-right "avatar icon" and select "Your profile". Have a quick browse through your page.

<p align="center">
<img src=../../../20171024_GitHub_Chemistry_Cambridge/blob/master/images/p2_1.png width="800">
</p>

- Click on the top-right "+" icon and select "New repository". **Verify your email address**. You should have just received an email from GitHub in the address provided before. Find this email and click on "Verify email address".

<p align="center">
<img src=../../../20171024_GitHub_Chemistry_Cambridge/blob/master/images/p2_2.png width="400"> <img src=../../../20171024_GitHub_Chemistry_Cambridge/blob/master/images/p2_3.png width="400">
</p>

- Create a new repository page. Fill in a "Repository name", e.g. "my_first_repository" or "my_analysis_script". Write a short description of your repository e.g. "This is a test repository". For now choose "Public" and select the box to initialize this repository with a README. Finally, click on "Create repository".

<p align="center">
<img src=../../../20171024_GitHub_Chemistry_Cambridge/blob/master/images/p2_4.png width="800">
</p>

- You created your first repository! :rocket:



### Explore your first repository and GitHub account

#### Your first repository

- Click on **README.md** and go to the right pencil "Edit this file". Type anything to change the file, e.g. "GitHub is fun!".

<p align="center">
<img src=../../../20171024_GitHub_Chemistry_Cambridge/blob/master/images/p3_1.png width="800">
</p>

<p align="center">
<img src=../../../20171024_GitHub_Chemistry_Cambridge/blob/master/images/p3_2.png width="800">
</p>

- Scroll down. Introduce a commit change message, e.g. "My first update", and select the radio button "Commit directly to the master branch". Then click on "Commit changes". Voilá!

<p align="center">
<img src=../../../20171024_GitHub_Chemistry_Cambridge/blob/master/images/p3_3.png width="800">
</p>

- To view your **history of commits** for **README.md**, click on **README.md** and then on the "History" button on the right.
- Alternatively, to view your **history of commits** for your first repository, click on the name of your repository and select the tab depicting a small clock and the number of commits next to it.

Bonus points (5 min):

- Try to create a new file
- In your new repository, have a look at the "Settings" tab, explore "Collaborators" and try to add the person sitting next to you.


#### Your GitHub account

- Click on your top-right "avatar" icon and select "Settings".

<p align="center">
<img src=../../../20171024_GitHub_Chemistry_Cambridge/blob/master/images/p3_4.png width="800">
</p>

- Explore the tabs "Profile", "Account" and "Emails".


**Key glossary:**

- **Repository**: it can be thought of as a project folder. A **repository** contains all of the project files, issues, wikis and more. It also stores the history and versions of each file.

- **Commit**: equivalent to saving your changes to a file. When you **commit** you usually include a brief description of the changes you made so you can identify versions later if you want to undo a change.

- **Branch**: an identical copy of a project at a particular point in time kept separate from the 'master' branch (primary copy). This keeps your code in the 'master' branch safe while you make changes and experiment with code on the new branch. You can merge your new branch back into the 'master' branch when you want to publish your changes.

- **Master**: the default branch in your repository.

- **Collaborator**: someone with read and write privileges to a repository as approved by the repository owner.



### Making changes using Git in the command-line

#### Check if Git is already installed in your computer, otherwise install it

(Git is already installed so you can jump to the next section)

- (If in Mac), go to *Finder* -> *Applications* -> *Utilities* -> *Terminal* and type `git --version`.
  - If you get as output something like `git version 2.5.4 (Apple Git-61)`, then Git is already installed -> Jump to the next section.
  - If you get something around `git: command not found`, keep reading.

- To install Git in Mac, follow one of the next strategies:
  1. When running one of the following commands `git --version`, `git config` or `xcode-select --install` you may be offered to install developer command line tools. Accept the offer and follow with "Install".
  2. Go to https://git-scm.com/downloads and download git. Double click on the downloaded executable and follow instructions.
  3. If you have `homebrew` installed, type the following in the Terminal: `brew install git`.

- Check the following for installing in [Windows](http://happygitwithr.com/install-git.html#windows) or [Linux](http://happygitwithr.com/install-git.html#linux).


#### Tell Git who you are (your GitHub username) and what your email address is

Use your GitHub username and email address to tell Git who you are:

```bash
cd ~/Course_Materials
git config --global user.name "semacu"
git config --global user.email "sermarcue@gmail.com"
```

**Remember to change** "semacu" and "sermarcue@gmail.com" to the username and email you used when creating the GitHub account.

Check:

```bash
git config --list
```


#### Clone the repository created before

```bash
git clone https://github.com/semacu/my_first_repository.git
cd my_first_repository
ls -lh
```

Your first repository created using GitHub (my_first_repository) is now a local repository located in your Desktop folder. *Remember what we discussed earlier about Git being a distributed version control system*.


#### Tell git what's your remote repository url to pull and push commits

```bash
cd ~/Course_Materials/my_first_repository
git remote set-url origin https://semacu@github.com/semacu/my_first_repository.git
```

Check:

```bash
git remote -v
```


#### Make a change to the `README.md` file using your favourite text editor

- Go to the cloned folder (`my_first_repository/`) and open `README.md` with your favourite text editor, e.g. gedit
- Change `README.md`, e.g. add a new line "This is my second line of script" and save changes.
- Now, go back to the Terminal and check how changes are tracked by Git:

```bash
cd ~/Course_Materials/my_first_repository
git status
```

The status of `README.md` is modified but the changes are not staged (red).


#### Stage and commit the change

Staging:

```bash
git add README.md
git status
```

The status of `README.md` is modified and now the changes are `staged` (green) and ready to commit.

Committing:

```bash
git commit -a -m "My second update"
git status
```

#### Push changes to your online GitHub repository

```bash
git push origin master
```

Now check that your change to `README.md` made to your online GitHub repository.

Bonus points (5 min):

- Make another change to `README.md` using the online GitHub repository and pull the change to your local repository (Hint: use `git pull`).


**Key glossary:**

- **Clone**: a copy of an online repository on your local computer so you can make edits on your own personal copy without having to be online. You can sync changes between your clone and the remote copy (GitHub) when you are online.

- **Remote**: a version of your project repository that is hosted on the Internet or network somewhere (e.g. copy of your project on GitHub vs. on your local computer).

- **Stage** and **commit**:

<p align="center">
<img src=../../../20181003_Intro_git_GitHub/blob/master/images/stage_commit.png width="500">
</p>

<p align="right">
(https://git-scm.com/book/en/v2/Getting-Started-Git-Basics)
</p>


- **Push**: sends the recent commit history from your local repository up to GitHub.

- **Pull**: grabs any changes from the remote GitHub repository and merges them into your local repository.



### Extras

- Create an issue
- Fork a repository from another user e.g. https://github.com/githubtraining/hellogitworld, make some changes to the `README.txt` and create a pull request
- Create a new branch, open a pull request and merge the newly created branch with the master branch





## Outlook

- This was an overview to the basic functionality of Git and GitHub to version control and share scripts and text files.

- Next steps for computational reproducibility, going back to the Nature Methods August 2018 editorial [**Easing the burden of code review**](https://www.nature.com/articles/s41592-018-0137-5):

*[...] Yet, even in the era of Git repositories, peer reviewing code can be frustrating and time consuming [...] Computational tools are complex objects that depend on many components to run. Dependencies include the operating system, programming language, external code libraries, configuration settings and run parameters. Reproducing these conditions is made even harder by the fact that components typically exist in multiple versions. Many come with their own prerequisites, creating a maddening rabbit hole of dependencies on dependencies [...]*

In other words, future steps will be to be able to execute code directly online (cloud). Two new resources are beginning to make a difference in this area: [Code Ocean](https://codeocean.com/) (Nature Methods, Nature Biotechnology and Nature Machine Intelligence have launched a trial to facilitate the peer review of computational methods and to improve their reproducibility) and [Binder](https://mybinder.org/) - check them out if you are interested :wink:

- Another future step, the ability to version control *large data files* (Gb - Tb) is currently not available. Some promising steps include the libraries [piggyback](https://cran.r-project.org/web/packages/piggyback/index.html) and [git lfs](https://git-lfs.github.com/).



## The End

Many Thanks for your attention! Enjoy Git and GitHub! :octocat:

Any questions about this workshop or the materials? Just email: sermarcue@gmail.com or mark.fernandes@cruk.cam.ac.uk



## References and materials

Blogs:
- [Beyond Basic R - Version Control with Git](https://owi.usgs.gov/blog/beyond-basic-git/)

Books:
- [Happy Git and GitHub for the R user](http://happygitwithr.com/)
- [Git book](https://git-scm.com/book/en/v2)

Courses:
- [Open Scientific Code using Git and GitHub](https://open-source-for-researchers.github.io/open-source-workshop/) by Yo Yehudi
- [A Friendly Introduction to GitHub](https://kirstiejane.github.io/friendly-github-intro/)
- [Software Carpentry: Version Control with Git](http://swcarpentry.github.io/git-novice/)
- [Resources to learn Git](http://try.github.io/)
- [GitHub On Demand Training](https://services.github.com/on-demand/)
- [A quick introduction to Git and GitHub](http://www.datacarpentry.org/semester-biology/materials/git-in-30-minutes/)

Help:
- GitHub [Help](https://help.github.com/)

Papers:
- Nature Methods 2018 editorial, [Easing the burden of code review](https://www.nature.com/articles/s41592-018-0137-5)
- Perkel 2018:
  - [When it comes to reproducible science, Git is code for success](https://www.natureindex.com/news-blog/when-it-comes-to-reproducible-science-git-is-code-for-success)
  - [TechBlog: Git: The reproducibility tool scientists love to hate](http://blogs.nature.com/naturejobs/2018/06/11/git-the-reproducibility-tool-scientists-love-to-hate/)
- Silver 2018 [Microsoft’s purchase of GitHub leaves some scientists uneasy](https://www.nature.com/articles/d41586-018-05426-0)
- Russell et *al.* 2018 [A large-scale analysis of bioinformatics code on GitHub](https://www.biorxiv.org/content/early/2018/05/14/321919)
- Perez-Riverol et *al.* 2016 [Ten Simple Rules for Taking Advantage of Git and GitHub](http://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004947)
- Perkel 2016 [Democratic databases: science on GitHub](https://www.nature.com/news/democratic-databases-science-on-github-1.20719)
- Markowetz 2015 [Five selfish reasons to work reproducibly](https://genomebiology.biomedcentral.com/articles/10.1186/s13059-015-0850-7)

Videos:
- [GitHub Training & Guides](https://www.youtube.com/githubguides)
- [Git & GitHub tutorial for Beginners](https://www.youtube.com/watch?v=3RjQznt-8kE&list=PL4cUxeGkcC9goXbgTDQ0n_4TBzOO0ocPR)

Websites:
- [git](https://git-scm.com/)
- [Mastering Markdown](https://guides.github.com/features/mastering-markdown/)



## Acknowledgements

<p align="center">
<img src=../../../20171024_GitHub_Chemistry_Cambridge/blob/master/images/UniversityCambridge_logo.png height="50"> <img src=../../../20171024_GitHub_Chemistry_Cambridge/blob/master/images/CRUKCI_logo.jpg height="50">
</p>

