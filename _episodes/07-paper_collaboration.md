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

## Recommended Trello template
The standard to do, in progress and done lists are usually sufficient but feel free to add more. The following labels will likely be helpful.

![paper_labels](../fig/paper_labels.png)

Plots, Tables, and Writing will make it more transparent what the card's task is and will make it easier to find the task you are looking for. Needs discussion is a helpful label to flag something you are unsure of so you can prioritise discussing the card in the next meeting. Processing is a useful label in case of supercomputer maintenance or outages. You will be able to see which tasks you need to prioritise before the supercomputer is down.

Here is an example of a Trello board used for developing a survey paper.

![paper_example](../fig/paper_example.png)

As the board gets busier, you can use filters to find important tasks. For example, the supercomputer is about to go into maintenance for a week, so I want to see all processing tasks assigned to me. I click the filter button in the top right and click "Cards assigned to me" and the Processing label.

![paper_filter](../fig/paper_filter.png)

I can now see that I have one processing task assigned to me, so I will complete it before the supercomputer is down for maintenance.

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

## Paper version control
Proper verson control of your paper will allow you to compare with earlier versions (if you want to revert a change) and prevents the need of keeping multiple versions. Overleaf has become hugely popular for collaborating on papers and for the following methods we will assume that is what you are using to write your latex papers. There are several methods of version control with Overleaf, the project lead should choose the method before beginning writing the paper.

### Method 1: Overleaf premium
If you, or the paper owner, has Overleaf premium, then Overleaf will keep track of changes for you. To view the history, you click the History button, and you can view all the changes you and your collaborators have made.

![overleaf_histroy](../fig/overleaf_history.png)

You can see the differences each change made with the "Compare to another version" button in the top left. For example, here is a diff where I can see myself adding an equation.

![overleaf_diff](../fig/overleaf_diff.png)

As you can see, most of the version control is automated. The only manual version control required is adding labels (the blue button on the top right in the History tab).

![overleaf_label](../fig/overleaf_label.png)

Once you've added a label, you can view them in the Labels section of the History tab to compare the differences between versions.

![overleaf_label_view](../fig/overleaf_label_view.png)


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


## Reflect
Once the paper is published or the project is completed it is important to have a final meeting to reflect on project. Think if there are things you could improve on for future projects.


{% include links.md %}

