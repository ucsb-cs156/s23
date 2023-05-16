---
title: "Week 07 - 05.16 Tue"
lecture_date: 2023-05-16
description: "Db Tips, and Agile Retrospective"
ready: true
layout: default
parent: lectures
---

{% include drop_down_style.html %}

# Ten minute standup 2:01pm-2:11pm

* Do a written update on the slack channel
* Do an out loud standup


# Database tips: 2:11pm- 2:15pm

* How to reset the db on localhost: `mvn clean`
* [How to reset the db on dokku](https://ucsb-cs156.github.io/topics/dokku/postgres_database.html#resetting-the-database) 
* When should I do this?
  - If you are getting strange `SQL` errors in your backend console output
  - Especially if you get these after making a change to an `@Entity` class.

In real world applications, this is done with something called *database migration frameworks*.

That's a topic we've tried to introduce into this course a few times (unsuccessfully so far).

If someone would like to take on a CMPSC 192 or CMPSC 196 independent study on this topic in Summer or Fall, let me know.

# Outline of rest of week 

Wednesday Discussion:

10 minute standup followed by:

* 5pm: Gauchoride: Customers will be there 
* 6pm: Happy Cows: Customer will zoom in
* 7pm: Courses: You and me are the customers

We'll go over the apps and what they do, and start organizing the Kanban boards.

Thursday: Work session on team03 (try to get it done, or close to done).

# Agile Retrospective Intro (2:20-2:45)

# Today (outline)

The most important aspect of Agile: The Retrospective

We "inspect and adapt".

* Pause all work/submission for team02/team03.
* Focus only on the retro, and do not rush through it.
* A retro that lasts less than 30 minutes raises questions about whether it is a good faith effort.
* Give it the time that it needs.

# Retrospective: the heart of Agile

The core principle of Agile is "inspect and adapt".  
* It was "inspecting and adapting" that led the original authors of the [Agile Manifesto](https://agilemanifesto.org/) to their ideas.
* It has been by "inspecting and adapting" that the Agile philosophy continues to grow and develop.

Inspect and Adapt is, in many ways, linked to the *Scientific Method*; 
* we observe
* we form a hypothesis
* we do an experiment

All in the service of doing a better job of software development.

In a retro, the team stops, pauses, reflects, and most importantly *comes up with an actionable change* for their practice.

# Today's Retro (2:45 - 3:15)

* Start by having everyone take 5 minutes to read through this article: [https://ucsb-cs156.github.io/topics/agile/agile_retros.html](https://ucsb-cs156.github.io/topics/agile/agile_retros.html)
  - Really read it!  It has the instructions for the most important activity in today's class
 
* Next, choose a leader for your retro. It should be someone that has read the instructions and is comfortable leading the group. 
* Then, locate the Google Drive folder for your team.  It should be linked in your Slack channel with a `gdrive` link this:

<img width="260" alt="image" src="https://user-images.githubusercontent.com/1119017/166498621-8fc7d61a-4d76-404d-9514-ea4672667ad9.png">

Check that each member of the team is able to access the folder.

In that folder, create a folder called `Retros` and in that folder, create a document `Retro1`

Then follow the instructions in the [https://ucsb-cs156.github.io/topics/agile/agile_retros.html](https://ucsb-cs156.github.io/topics/agile/agile_retros.html) article for  Stop/Start/Continue retro.

In the document, write down who your retro leader is.

At the end of the process, you should have in your document:
* Name of person leading the retro at the top, and a list of who participated
* A document with three parts, "stop/start/continue", and items from each member under the three categories
* Dot voting (three votes per team member participating) on the items in the document.
* A summary at the bottom on an "experiment" in the form "If we change X we hope to see Y result"
  - This should be related to one of the top three items by votes that your group agreed on.
* A brief explanation of how you will know whether your experiment was or was not a success.

# After the retro is done

* Ask a staff member to look over your GDrive document; they'll check it to make sure it has the required elements:
  - items from each member under start/stop/continue
  - dot voting
  - an experiment, including the criteria by which you can know whether the experiment was a success

# Next steps if there's more time

* Start looking over your repo for the legacy code project (links here: <https://ucsb-cs156.github.io/s23/lectures/lect20/> )
* Start looking at the issues for your legacy code project (links below)
  - Note that each of these is still being refined by the staff
  - You will have a part in shaping these issues also; that's what we're doing in class tomorrow   
  - We'll talk in section Wednesday and in lecture next Tuesday about how to divide up and prioritize the issues
  - We'll also talk about how code reviews and grading works for the legacy project phase.
* Also start playing with the applications
  - In some cases, the features you can access will be limited because you don't have admin access
  - By Thursday, I'll have instructions for you to set up prod and qa instances for your individual forks of the projects so that can try the admin features also

# Legacy code issues

- 5pm: Gauchoride: [Issues](https://github.com/ucsb-cs156/proj-gauchoride/issues), [Brainstorm Document](https://docs.google.com/document/d/1oDyqpJzZJpRjhOn_uON-b1ssP6DokY8CPWRRkIi4mMM/edit)
- 6pm: Happy Cows: [Issues](https://github.com/ucsb-cs156/proj-happycows/issues)
- 7pm: Courses: [Issues](https://github.com/ucsb-cs156/proj-courses/issues) 

# Legacy code prod and qa apps (central)

| Section | App | Type | Link       | 
|------|------------|---|---|
| 5pm | gauchoride | prod | <https://proj-gauchoride.dokku-00.cs.ucsb.edu/> | 
| 5pm | gauchoride | qa | <https://proj-gauchoride-qa.dokku-00.cs.ucsb.edu/>  | 
| 6pm | happycows | prod | <https://proj-happycows.dokku-00.cs.ucsb.edu/> | 
| 6pm | happycows | qa | <https://proj-happycows-qa.dokku-00.cs.ucsb.edu/>  | 
| 7pm | courses | prod | <https://proj-courses.dokku-00.cs.ucsb.edu/> | 
| 7pm | courses | qa | <https://proj-courses-qa.dokku-00.cs.ucsb.edu/>  | 

