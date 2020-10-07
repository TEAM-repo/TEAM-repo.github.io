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
* **tester**: responsible for verifying that the project is reproducible 
* **documenter**: responsible for making sure that the workflow and the decisions are well-documented
* **domain expert**: while everyone on the team should have some basic understanding of the domain, it might be helpful to have someone who can dive deeper into additional articles/literature to help the team understand the background of the project/field
* **developer / scientist**: responsible for implementing the project, developing and testing models, communicating results

## Team Communication

The team should agree on a channel of communication that all teammates will be regularly checking.
While Facebook Messenger and WhatsApp are viable options, there are a lot of distractions that might hinder your ability to focus on the project.

We recommend using Slack, potentially aided by GitHub Projects (or a Trello board). 
Some of Slack's helpful features include:
* reply to a message in a thread to make it easier to follow a specific discussion (esp. when discussing different topics) and keep the relevant information in the same thread
* tagging specific team members (using `@username`) to get their attention
* you can see all conversations that you were tagged in using the `@ Mentions and reactions` icon at the top left (above the list of channels)
* you can also save/pin conversations for easy access
    * if you hover over a message, you can click the bookmark icon (that says "Save"); it will add the note to your saved items -- on the top _left_ side of the app, you will get a new "Saved items" menu; 
    * if you click on the vertical ellipses (the three dots) that show up when you hover over the note (to the right of the "Save" bookmark icon), you'll get a menu of options; click "Pin to channel", then to find the pinned note, go to the top right side of the app, under your profile picture: click on the “info icon” :information_source:: there you can find any of the “pinned” conversations.

Google Docs/Spreadsheets are another set of tools that can help the team stay organized by keeping track of tasks, progress, and upcoming deadlines.

### Regular Check-ins / Status Updates

In Agile methodology (a software development model), teams run through **daily stand-ups**: teammates stand up in a room together and provide a quick update addressing the following three points:
* what I worked on / finished yesterday
* today's task
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

If you don't have Jupyter notebooks installed on your computer, you can access Google's Colaboratory via <https://colab.research.google.com>. Also, if you upload the `.ipynb` notebook into your Google Drive, when you click on the notebook, it will ask you if you want to open it with Colaborate.

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

Here's a **GitHub Basics Tutorial - How to Use GitHub** <https://youtube.com/watch?v=x0EYpi38Yp4> to get you started.

------

To really see the power of GitHub, you need to work with a team. So, let's get started!

# Hands-on with GitHub

Within your team designate one person as a Project Manager (PM). That person is the owner and the maintainer of the project repository.

## New repo

The PM creates the `PROJECT_REPO` using the GitHub interface.
* Select an option to add a `README.md` when creating the repo.
* Select an option to add a `.gitignore` file for Python (you can always change it later)
* Share the link with the team (we'll refer to it as the `PROJECT_REPO`).

## Fork the repo

Team members **fork** the `PROJECT_REPO` using the GitHub interface.

This forked repo has a different URL (i.e., web address) for each team member. We will refer to it as `PROJECT_REPO_FORK`.

## Clone the (forked) repo

Now that each team member has their own fork (i.e., copy) `PROJECT_REPO_FORK`, which is connected to the main `PROJECT_REPO`, it's time to **clone** the fork to your local computer.

To clone  `PROJECT_REPO_FORK` to your computer, open a Terminal window and type:
```
git clone PROJECT_REPO_FORK
```

**Note**: if you type `pwd` (i.e., _print working directory_) it will produce a path to the folder on your computer which now contains a cloned version of your forked repo (`PROJECT_REPO_FORK`). 

You can verify that the new repo is there by running `ls -l` (Note: _these are not ones (1) but "ells" (lowercase Ls)_). Once you run the `ls` command you should see your `PROJECT_REPO_FORK` folder on the list.

Congrats! You can now switch to that folder by typing
```
cd PROJECT_REPO_FORK
```

If you run `ls` you should see the README.md file (if the PM added it to the repo when they created it).

Woohooo! We are done with the setup and are ready to start working with the files.


------

# Making а simple change in _your fork_

Someone on the team should now try to make a change to the `.gitignore` file **in their `PROJECT_REPO_FORK`**. 

Navigate (using `cd`) to the directory that you were working in.

If you are on the Terminal, I'd recommend opening it using the command-line editor.

* Open the `.gitignore` file and write `.DS_Store` at the top of the file.
* Save the file.
* Verify that your changes are detected by running `git status`. It tells you which files you have modified. 
   * If the notebook that you created is "red" in the "Untracked files" category, make git aware that it needs to keep track of it by adding it to the notebook.
   * Add the changes by running `git add .gitignore`
* See the difference by running `git status` and make sure that only the files you intended to change are “green”.
* Commit your changes `git commit -m "Added .DS_Store to .gitignore"`
* Make your change show up on the github repo website by pushing to the repo using `git push` (note: not including `origin <branchname>` after `git push` defaults to `origin master`)

That was a great contribution, however, it now lives in _your fork_ and not in the main `PROJECT_REPO`. 
Nobody from your team has access to it.
You need to make your PM aware of this awesome addition by issuing a **Pull Request** (usually abbreviated as PR).

Pull Requests (PRs) are typically issued through the GitHub web interface. 

**Important**: make sure to select the "[compare across forks](#)" link and then set the `base` and `head` repositories and branches accordingly.

PM needs to approve and merge this pull request before the other teammates can create their own PR from the `PROJECT_REPO` to their `PROJECT_REPO_FORK`.
After they merge their PR, they'll be able to run `git pull` in their `PROJECT_REPO_FORK` to update their files locally.

-----

OK, now that we practiced the simple change in a `.gitignore` file, we can try our hand at managing a Jupyter notebook.

------

## Committing changes you make to the notebook

!!! **Every time, before you make any changes**, make sure to bring your files up-to-date by checking if your repo is behind the upstream, using a PR to get the changes and running `git pull` on your computer. 
If you run into merge conflicts, the easiest solution is to rename the conflicting notebook and pull it again.

Next, make your changes to the notebook `NOTEBOOK.ipynb`.

Before you submit your changes, make sure to clear all cell output by going to the top menu and clicking
```
Cell -> All Output -> Clear
```

Switch to the Terminal window. 

Navigate (using `cd`) to the directory that you were working in.

Verify that your changes are detected by running `git status`. It tells you which files you have modified. 

If the notebook that you created is "red" in the "Untracked files" category, make git aware that it needs to keep track of it by adding it to the notebook.

Add the changes from the notebook that you modified by running
```
git add NOTEBOOK.ipynb
```

See the difference by running `git status` and make sure that only the files you intended to change are “green”.
```
git commit -m “Message explaining what you changed”
```

Make your changes show up on the github website by pushing them to the repo (not including `origin <branchname>` after `git push` defaults to `origin master`):
```
git push
```

If there are merge conflicts, you can save your version by running `git stash` or renaming it and then `git pull` again.



---------

If you have any questions or suggestions, don't hesitate to reach out to me via ykk@ucsb edu.

These materials are released under the CC BY 4.0 by Yekaterina Kharitonova. For attribution, please reference the paper:
["Redesigning a Software Development Course as a Preparation for a Capstone: An Experience Report"](https://dl.acm.org/citation.cfm?id=3287498).

Page last updated: Oct 7, 2020

