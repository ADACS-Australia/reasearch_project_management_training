---
title: "Trello"
teaching: 10
exercises: 5
questions:
- "What is Trello?"
- "How do I keep track of my tasks?"
- "How do I use Trello workspace and boards to collaborate with others?"
objectives:
- "Become familiar with how to use Trello"
keypoints:
- "Making Trello workspaces"
- "Making Trello cards"
- "Making Trello card templates"
---

# Trello
Trello is one of the most popular project management applications thanks to it being easy to use and flexible. If you have not already, create a Trello account [here](https://trello.com/).
## Making your first workspace and board
When you first make a Trello account you will see this screen.

![trello_first_workspace](../fig/trello_first_workspace.png)

We recommend that you name your first Workspace "Personal" (you can change this later). Click continue and then skip the free trail.

You can then click "Create your first board" and name it something related to your work like "Research". There are several useful templates but for now we will show you how to make one from scratch.

![trello_first_board](../fig/trello_first_board.png)

## Project Plan
Once you have made the project Trello board, the first thing you should do is fill in the description (or a card) with your project plan. You can add a description by pressing "Show Menu" (top right) and clicking on the description. The following is our recommended description template which is excellent for collaborative projects but you may also find helpful for personal projects.

~~~
Title

Description:

Estimated completion date:

Collaborators:
# Name, Role, Affiliation, FTE, Email
- @Jocelyn (link to account), Project Lead, CIC, 0.5, jocelyn@gmail.com

Goals:

Requirements:
E.g. Supercomputing or telescope time

Risk and mitigation measures:

Software:

Documentation:

Data storage (Eg. google drive folder):

~~~
{: .language-MD}

This project plan is for your internal reference, and it should assist your communication and data management.

### Title and description
These can be kept brief and should be used to quickly introduce a new collaborator to what we plan to do and include any relevant plots.

### Estimated completion date
In research, there are rarely hard deadlines for project completion, but it is still helpful to estimate how long a task will be complete so researchers can budget their time.

### Collaborators
Stating all the collaborators and their roles will clarify who holds which responsibilities from the beginning. The Full-Time Equivalent (FTE) has two purposes; it will give the project lead an idea of how much work they can assign and for the collaborators' reference to track how much time they have already committed before accepting new projects.

### Goals
These goals can be brief and straightforward (e.g. publish a paper and process some data) and used to keep the project on track. When deciding on the next steps, you should consider the project's goals to ensure that you are not doing work that is outside the scope of the project.

### Requirements
There are likely some supercomputing or telescope requirements for your project. It is important to state these early on to plan proposals and estimate when you will get processed data.

### Risks and mitigation measures
If your proposals are not accepted, are there other telescopes or supercomputers that you can use? Will you back up your data in case the supercomputer crashes and you lose it? A quick consideration of the risks and what you can do to mitigate them can save you a lot of pain down the road

### Software
If you're developing software as part of this project, you should include the GitHub repository link. If there is software that you depend on or are adapting, it is useful to include those links here. Where possible, you should version control your software within your groups' GitHub organisation

### Documentation
Here, you can link the documentation you're developing or any other helpful documentation.

### Data storage
The best method of data storage is very project dependent. How to access the data should be described here, which could be a link to cloud storage or the directory on a supercomputer. E.g. Google drive, R drive or CloudStor and who has access

## Creating cards
YOu can think of each Trello card as a single task (even if that task has several steps). Click "Add a card" and give in a simple title. You can then click on the card and give it a description.

![simple_card](../fig/simple_card.png)

You can then add to the card so it contains more information
- Members: You can assign users to cards so you can easily see who is working on task.
- Labels: The labels are customizable so you can use them in any way that you find useful. You can label you cards into types of tasks (Eg. processing, writing, researching) or urgency for example.
- Checklist: You can use checklists to keep track of which steps you have completed.
- Dates: You can set a due date and set yourself due date reminders.
- Attachments: You can attach any type file. You can attach files in comments so you can explain what changes you've made to the image and have a record of all image versions.
- Comment: You can use comments to keep notes of what you've done and even commands you've run and their output

Here is an example of what the card could look like


![detailed_card](../fig/detailed_card.png)

## Making card templates
Card templates are useful as reminders or what information to include or to save yourself time when you know you will be making a large number of similar cards.

Here is an example of a simple template
![template_card](../fig/template_card.png)
I created this template by filling in the description and clicking "Make template" at the bottom right of the card. You can now make new cards from this template and use the text as a reminder of what you should include.

Templates are also useful for keeping track of processing steps. Here is an example of a processing template which will remind you of the data to record and has a checklist to help me keep track of which step you are on.
![processing_template](../fig/processing_template.png)

## Creating research group workspaces
You can make a Trello workspace for your research group that will allow all workspace users to have access to all of the Trello boards within the workspace. You can make a new workspace by clicking Trello then the new workspace button.

![make_workspace](../fig/make_workspaces.png)

You can then name your workspace whatever you wish

![pulsar_workspace](../fig/pulsar_workspace.png)

Then add members by sending them an email invite

![add_members](../fig/add_members.png)

You can then create a board for every large project you have. All members of your workspace will have access to these boards.

![several_boards](../fig/several_boards.png)

Recomendations on how to uses these boards effectively will be covered in the following episodes
<!--TODO add links to the episodes-->

### Private boards
By default, all workspace members have access to the boards in said workspace. If you have private data that you are not ready to share with everyone in your group you can switch your board to private.

![make_private](../fig/make_private.png)

You can also keep it in your personal workspace and move it to the group workspace when you are ready to share the results.

![change_workspace](../fig/change_workspace.png)

{% include links.md %}

