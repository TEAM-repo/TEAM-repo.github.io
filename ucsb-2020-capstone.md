---
layout: default
title: Capstone Resources 
description: Resources for the capstone teams
---

## Getting Ready for Collaborative Work

Congratulations! You are getting ready to work in teams and learn a lot about collaboration, productivity, and data science.

Before we get started, it would be helpful if you:
* create a GitHub account
* install `jupyter notebook` on your computer
* ...

Strongly recommended:
* download the Slack desktop client (don't use the web version unless you absolutely have to; notifications and navigation is much better in the application itself)
* create an account on Overleaf
* ...

## Team roles and expectations

Once you are assigned into a team, we recommend that you select a **Project Manager (PM)** who will be in charge of organizing the team and communicating with your team's liaison/client. The PM's expectations and responsibilities are listed here: [pm_expectations.md]({{site.materials_repo}}pm_expectations.md).

Additional roles that we recommend for your team to consider:
* tester: responsible for verifying that the project is reproducible 
* documenter: responsible for making sure that the workflow and the decisions are well-documented
* domain expert: while everyone on the team should have some basic understanding of the domain, it might be helpful to have someone who can dive deeper into additional articles/literature to help the team understand the background of the project/field
* developer / scientist: responsible for implementing the project, developing and testing models, communicating results

## Team Communication

The team should agree on a channel of communication that all teammates will be regularly checking.
While Facebook Messenger and WhatsApp are viable options, there are a lot of distractions that might hinder your ability to focus on the project.

We recommend using Slack, potentially aided by GitHub Projects (or a Trello board). 
Some of Slack's helpful features include:
* reply to a message in a thread to make it easier to follow a specific discussion (esp. when discussing different topics) and keep the relevant information in the same thread
* tagging specific team members (using `@username`) to get their attention
* you can see all conversations that you were tagged in using the `@ Mentions and reactions` icon at the top left (above the list of channels)
* it is helpful to use the "Save" (bookmark icon) for any messages that you want a quick access: hover over the message and select that icon in the menu that pops-up on the right
* on the top right side of the app, under your profile picture, is an "info icon": there you can find any of the "pinned" conversations

Google Docs/Spreadsheets are another set of tools that can help the team stay organized by keeping track of tasks, progress, and upcoming deadlines.

### Regular Check-ins / Status Updates

In Agile methodology (a software development model), teams run through **daily stand-ups**: teammates stand up in a room together and provide a quick update addressing the following three points:
* what I worked on / finished yesterday
* what is my today's task
* obstacles / blocks / help that I need.

The reason for standing up is to keep the meeting quick. 
You don't necessarily need to be standing, nor does your meeting need to be daily.
Set an interval that your team agrees on (preferably, more than once a week) and know that failure to communicate is one of the warning signs that the team needs to pay attention to and resolve as soon as possible.

You can use a Slack channel `#updates` to provide these daily check-ins: at the end of the day, have everyone post their answer to the three points listed above.

The main takeaway is that your team needs to be **in regular communication** with the PM and each other, and have a way to quickly clear up or address any issues that come up.

### Meeting Agenda

If your meeting has no agenda, nobody is taking notes, and/or there are no follow-up actions, then you are wasting everyone's time.

You can use a simple Google Doc for notes or use this sample agenda for the client-team meeting ([agenda.md]({{site.materials_repo}}agenda.md)); guidelines/template: <https://www.overleaf.com/read/jkkfjwhwjcjp>.
I recommend using Overleaf, since documents typeset in LaTeX are easier to backup, and they also support mathematical formulas, which might be handy for communicating algorithms.

## Jupyter notebooks

* Work through a tutorial on how to use the notebook (don't just watch it, follow along).
* Learn the shortcuts! They will save you a ton of time.
* Use the notebook to document your process: write down your questions, ideas, things to look up.
* Keep your EDA notebook separate: it makes it easier to keep it in another tab and minimizes scrolling, when you are working on the main notebook.
* Always use `Clear All Output` before committing your notebook. 
    * Jupyter notebooks are stored in a JSON format, so if you don't clear the cells, the output is stored in the notebook's JSON file as well, which will generate merge conflicts the next time someone tries to submit their changes.
    * You can easily rename the notebook and pull-in the new changes if you run into merge conflict, but it's easier to just clear the cells. :-)


And that brings us to...

## Version Control

git and GitHub are two of the currently popular tools to keep track of the changes in text-based files.

**What's the difference between git and GitHub?**
A lot of times you'll hear people use these terms interchangeably but that's not entirely correct.

**git** runs locally on your computer and keeps track of the changes that you make to the files on your machine.
You won't be able to share these changes with your teammates using git alone, and that's where GitHub comes in.

**GitHub** is a web service, a "cloud" platform that hosts your projects in repositories and allows you to share your repos with the world.
There are alternative solutions to GitHub, such as GitLab and BitBucket, but they are all designed to let you `push` your local changes to the cloud to enable backup, sharing, and collaboration.




## Plan your project

[project_plan.md]({{site.materials_repo}}project_plan.md):  A scaffolding to help plan the project and provide the structure for the final write-up (overall project goals, the solution to the client’s problem and how it fits the client’s needs, how the team will accomplish this solution, and specific tasks for this phase).
---

If you have any questions or suggestions, don't hesitate to reach out to me via ykk@ucsb edu.

These materials are released under the CC BY 4.0 by Yekaterina Kharitonova. For attribution, please reference the paper:
["Redesigning a Software Development Course as a Preparation for a Capstone: An Experience Report"](https://dl.acm.org/citation.cfm?id=3287498).

Page last updated: Oct 5, 2020

