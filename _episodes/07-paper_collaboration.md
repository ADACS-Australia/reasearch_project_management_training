---
title: "Project and Paper Collaboration"
teaching: 0
exercises: 0
questions:
- "How should I store my data so my work is reproducible?"
- "How can I version control my paper?"
- "What is the most efficient way to collaborate with my colleagues?"
objectives:
- ""
keypoints:
- ""
---

# Project Collaboration

## Project Planning
Once you have made the project Trello board, the first thing you should do is fill in the description (or a card) with your project plan. The following is a project planning template that we recomend.
~~~
Title

Description:

Estimated completion date:

Collaborators:
# Name, Role, FTE, Email
- @Jocelyn  (link to account), Project Lead, 0.5, jocelyn@gmail.com

Goals:

Requirements:
Eg. Supercomputing or telescope time

Risk and mitigation measures:

Github repos:

Data storage (Eg. google drive folder):

~~~
{: .language-MD}

This project plan is for your internal reference and it should assist your communication and data management.

### Title and description
These can be kept breif and should be used to quickly introduce a new collaborator to what we plan to do and include any relevant plots

### Estimated completion date
In research, there are rarely hard deadlines for project completion but it is still useful to estimate how long a task will complete so researchers can budget their time.

### Collaborators
Stating all the collaborators and their roles will make it clear from the beginning who holds which responsibilites. The Full Time Equivlent (FTE) has two purposes, it will give the project lead and idea of how much work they can assign and for the collaborators own reference so they can track how much time they have already commited before accepting new projects.

### Goals
These goals can be simple and breif (eg. publish a paper and process some data) they are most useful to keep the project on track. When deciding on next steps you should consider the goals of the project to assure that you are not doing work that is outside of the scope of the project.

### Requirements
There are likely some supercomputing or telescope requirements for your project. It is important to state these early on so you can plan proposals and estimate when you well get and have processed data.

### Risks and mitigation measures
If your proposals are not accepted, are there other telescopes or supercomputers that you can use? Will you back up your data incase the supercomputer crashes and you lose it? A quick consideration of the risks and what you can do to mitigate them can save you a lot of pain down the road

### Github repos
If you're developing software as part of this project you should include the github repository link. If there is software you depend on or are adapting it is useful to include those links here.

### Data storage
The best method of data storage is very project dependent. How to access the data should be described here which could be a link to cloud storage or the directory on a supercomputer.

# Paper Collaboration

## Reproducible data
It is important to make all results reproducible in research. Not only is this good practice so that other researchers can use your work, it will also improve the organisation of your data. You can assure this, first plan where to store your data so it is accessible in the future. The best solution is dependent on the size of your data.

### Small data (<1 GB)
If your data is less than a GB then you can store this data on a github repository. This is the easiest solution as you can build the data into your github scripts so you can simply download the data and reproduce your results

### Large data (<1 TB)
This data is too large to store on most online resources so you need to decide a long term place to store it. Some options are
- on a supercomputer
- on a local hard drive
- on a cold storage service

You must then include in your GitHub's README.md instructions on where the data is, how to download the data and, if it is not available to the public, who can download it on your behalf.

### Enormous data (>1 TB)
Some data is too large to store anywhere so instead you must document how to recreate the data. This should include the observations/data location, the software required to process it and what options you used to create the data.

## Using a GitHub repo for the paper
It is common use some simple python to create some plots or format a csv into a latex table. When we start collaborating this can bit complicated if we have several versions of these scripts and we're emailing the scripts back on forth. It is better to make a new GitHub repo so it is easier to collaborate and version controlled. The goal of the repository should be that you can run all of the scripts and reproduce all plots, tables and results from your paper. Not only is this good software practice, it is also good research practice to make it easier for future researchers to recreate your work. A link to the GitHub page should be put in the Trello Boards description.

## Recommended template

## Paper version control
Proper verson control of your paper will allow you to compare with earlier versions (if you want to revert a change) and prevents the need of keeping multiple versions. Overleaf has become hugely popular for collaborating on papers and for the following methods we will assume that is what you are using to write your latex papers. There are several methods of version control with Overleaf, the project lead should choose the method before beginning writing the paper.

### Method 1: Overleaf premium


### Method 2: Github pull and push
With a free overleaf account, you can make a GitHub repository that overleaf can push and pull to. You can use this to commit changes frequently and even use the GitHub page to tag release versions (first draft, referee response, final etc.).

You can create a GitHub repository by clicking the menu in the top right of the paper's overleaf page

![overleaf_menu](../fig/overleaf_menu.png)

and then click the GitHub button under Sync

![overleaf_github](../fig/overleaf_github.png)

Then give your new GitHub repository a Name and description and click "Create a GitHub repository". By default, it will make a private repository, and this is usually best to ensure no one accesses your paper before publication.

![overleaf_github_sync](../fig/overleaf_github_sync.png)

All users should frequently push their changes. You can do this by clicking the menu, GitHub, and then Push.

![overleaf_sync](../fig/overleaf_sync.png)

Then write a commit message.

![overleaf_push](../fig/overleaf_push.png)

Once you have made significant progress and you would like to mark this as a specific version (first draft, referee response, final etc.), you can go to the GitHub page and make a release. You can use these releases (also known as tags) to compare versions with `git diff`
<!-- TODO add a link if Paul has a relevant section -->

### Method 3: Git tracking of zip files

## Reflect
Once the paper is published or the project is completed it is important to have a final meeting to reflect on project. Think if there are things you could improve on for future projects.


{% include links.md %}

