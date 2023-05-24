---
title: "Week 08 - 05.23 Tue"
lecture_date: 2023-05-23
description: "Retro, Sprint Planning (or finishing team03)"
ready: true
layout: default
parent: lectures
---

# New CATME survey dropped

Please complete by midnight Thursday.

# If your team has submitted team03 (ten of twelve teams)

Please divide the 75 minutes of class time between

1. Retro (30-45 minutes)
2. Sprint Planning for Legacy Code project (30-45 minutes)

More on each of these below.

# If your team has not submitted team03 (two of twelve teams)

* You will be responsible for holding a 30 minutes retro outside of class
  - Please, **right now** before starting work on team03, work out when you are going to meet
  - Could be face-to-face, or over zoom; work that out too.
  - Deadline is midnight Monday May 29.
  - Possible tools: your slack channel, a [doodle](https://doodle.com/en/), a [when2meet](https://www.when2meet.com/)
  - Post the future meeting time and place (or zoom link) to your team slack channel
  - More details on what you'll need to do to verify that you held your retro below.
* Hold a standup on team03, and review the Kanban board to determine what still needs to be done
* Work on team03, and use `#help-lecture-discussion` on slack to ask for help
* 10% late penalty applies, and final deadline for submission is 11:59pm Tuesday May 23.

# Retro

The following instructions apply both to:
* the teams holdngretro held in class on Tuesday 05/23
* AND the teams making up the retro later in the week.

1. Visit your team's gdrive link (the one pinned to your team's slack channel)
   - In the linked team folder, there should already be a subfolder called `retros`, and in that folder, a document called `Retro1` from your 05/16 retro.
   - Add a second document called `Retro2`.  At the top, put the retro date (e.g. 05/23/23), the name of the person leading the retro, and the names of the team members participating (and any that are absent).
   - Ideally, the retro leader is a different person from the one that led the previous retro.
2. Conduct your retro.  If you need help remembering how it goes, these links may be helpful: 
   - General background on retros, including how to conduct a stop/start/continue <https://ucsb-cs156.github.io/topics/agile/agile_retros.html>
   -  If you want to change it up, here's [an alternative format suitable for beginners](https://retromat.org/blog/best-retrospective-for-beginners/).
   -  If you *really* want to change it up, the [retromat](https://retromat.org/) has hundreds of ideas for how to organize a retro.  Changing up the format keeps it interesting and may get better results.
   - One thing that some teams find helpful is to use your slack channel as a way for everyone to put in ideas; the idea is to not "press enter" until someone in the group gives a signal.  That way, no one sees what anyone else is typing ahead of time.  
   -  Or, you might try an free online retro tool such as one of the ones discussed in [this article](https://medium.com/productpeople/the-5-best-free-online-retrospective-tools-for-your-team-5cbb0b47f9c9).
   - If you use a free online tool, please invite the instructor (phtcon@ucsb.edu) and your team mentor to be part of the team, and include a link to the online output in your Google Drive document.  You don't need to duplicate the output as long as we can get to it from your Google Drive document.
3. If you don't use an online tool, record artifacts in your document.  These will vary depending on the style of the retro; if it's a start/stop/continue retro, it will include the list of thing that the team suggested should be stopped, started, or continued.
4. Include at least some discussion that looks at your previous retro's suggested experiment:
   - What did you suggest that the team try doing differently?
   - What was the outcome?
   - What did you learn, if anything, from the experiment?
5. Also include a suggestion for an experiment for the next sprint.

These instructions apply only to the teams making up the retro later in the week:

* Please include a screenshot of your zoom meeting, or a group photo showing who participated.
* As you conduct your retro, please reflect on factors led to the team not completing the project by the original deadline
* Please include some suggestions for what the team will do to avoid that from occuring during the project phase
   
# Sprint Planning for Legacy Code project

Each team already has a Kanban board setup for the legacy code project (see links below).

You should add the `In Review` column if it is not already present.

Then, you should populate your todo column with issues, start assigning them to your team, and start working.

You may not get through all of the Sprint planning today, but by the end of discussion section on Wednesday:
* Each of the six team members should be assigned to an issue in the todo column
* The previous bullet point shoudl *remain true* until your team reaches 100 points

Teams accumulate points when PRs are merged into main
* That is only done by the course staff for these projects.
* Each PR requires at least one code review from a team member, and at least one code review from a staff member
* The staff estimate points. Most issues are 5 to 10 points.
  - 5 points for very straightforward issues addressing a single concern
  - 10 points for issues that require a bit more work, but are nevertheless reasonably straightforward application of skills from team01, team02, team03.
  - 20 points is rare, and is reserved for issues that may be more complex, and/or require students to go significantly beyond the skills from previous course assignments.
* Note that breaking down issues into smaller chunks works to your benefit in multiple ways:
  - Easy to code review and merge (fewer merge conflicts), so faster point accumulation
  - Three 10 points issues and three 5 points issues adds up to 45 points; combining all of those together might only get you 20.
  - But the aim here should not be to "game the points". It should be to "get the issues implemented", in incremental "right sized" pieces.
  - If you do that, the points will take care of themselves.  
  
Points belong to the whole team, not to individuals
* Work as a team, and help each other.
* We do want to see every team member contribute
* Ultimately, it's a team project and a team grade.
* Having said that, really low CATME scores might result in a grade reduction.
 
  
## Where do issues come from?

For issues, you'll need to do a bit more work that in the previous team projects.

Here is where you'll get issues from:
* The three starter code repos have issues lists (as shown in the table below). 
  - A handful of these may be small easy issues. 
  - However, many (most?) of these issue *may not translate one-to-one into issues for your Kanban board*.
  - Instead, you are encouraged to try to *break the larger ones down into smaller issues*, each of which could be a single PR; more on this below.
  - This Sprint Planning meeting is where you can do some of that.
  - You may even need to add "issues about issues", e.g. an issue that says: "break issue #34 from proj-happycows into multiple issues on our team's repo".  Such an issue doesn't result in a PR, but it can still be moved across the Kanban board from `To Do`, to `In Progress`, to `In Review`, to `Done`.
* Your team's own ideas for features, based on the notes your team took last Wednesday during meetings with
  - Mike Fogelsanger for proj-gauchoride
  - Prof. Mattanjah deVries for proj-happycows
  - Prof. Phill Conrad for proj-courses

## Existing issues

Staff may add to these issues over the course of the project; when we do, we'll post an announcement in the project slack channels.

| Project |  Starter Code Repo | Issues Link | Project Slack Channel |
|---------|--------------------|-------------|-----------------------|
| proj-gauchoride | [Starter Code Repo](https://github.com/ucsb-cs156/proj-gauchoride) | [Issues](https://github.com/ucsb-cs156/proj-gauchoride/issues) | [`#proj-gauchoride`](https://ucsb-cs156-s23.slack.com/archives/C0595EWELLA) |
| proj-happycows | [Starter Code Repo](https://github.com/ucsb-cs156/proj-happycows) | [Issues](https://github.com/ucsb-cs156/proj-happycows/issues) | [`#proj-happycows`](https://ucsb-cs156-s23.slack.com/archives/C058QUC16QP) |
| proj-courses | [Starter Code Repo](https://github.com/ucsb-cs156/proj-courses) | [Issues](https://github.com/ucsb-cs156/proj-courses/issues) |  [`#proj-courses`](https://ucsb-cs156-s23.slack.com/archives/C058BPFQZ42) |

## You are encouraged to keep each PR small.

For example, implementing a new feature may require
* A new React Component (with tests and storybook entries, and perhaps fixtures to support those)
* A new React Page
  - This page might start out with a simple PR that establishes a placeholder with text "New feature coming soon", and a trivial set of tests and a storybook entry
  - It might later get data from the backend and display it using a component, and be linked to from the navigation bar.
* A new database table (or a new column in an existing database table, requiring modifications to an `@Entity` and/or `@Repository` class
* New API backend endpoints, which require controller methods and tests.

Each of these could (and arguably should be) a separate PR!  This helps to keep PRs small, which makes code review easier, and also helps the team to divide up work among the team members.

Still, you may need to document in the issues what the dependencies are (e.g. do issue 12 and 13 before starting 14).

# Legacy Code Background information

For each of the twelve teams, there is already:
* A repo, seeded with the starter code from previous quarters
* A prod and qa dokku instance
* A Kanban board

For each, I've set up Google OAuth client id and client secret, as well as the `UCSB_API_KEY` and `MONGODB_URI` for the `courses` project.  You are welcome to use `dokku config:show app-name` to get these values and use them for your localhost setup.

Links are provided below.

# Links


## 5pm - gauchoride

* Customer: Mike Fogelsonger (Director of Veterans and Military Services) and Holly Roose (Director, Promise Scholars Program, UCSB).

| Team | Repo | Github Pages | Prod | QA |
|--|--|--|--|--|
| s23-5pm-1 | [repo](https://github.com/ucsb-cs156-s23/proj-gauchoride-s23-5pm-1) | [pages](https://ucsb-cs156-s23.github.io/proj-gauchoride-s23-5pm-1/) | [prod](https://proj-gauchoride.dokku-01.cs.ucsb.edu) | [qa](https://proj-gauchoride-qa.dokku-01.cs.ucsb.edu)
| s23-5pm-2 | [repo](https://github.com/ucsb-cs156-s23/proj-gauchoride-s23-5pm-2) | [pages](https://ucsb-cs156-s23.github.io/proj-gauchoride-s23-5pm-2/) | [prod](https://proj-gauchoride.dokku-02.cs.ucsb.edu) | [qa](https://proj-gauchoride-qa.dokku-02.cs.ucsb.edu)
| s23-5pm-3 | [repo](https://github.com/ucsb-cs156-s23/proj-gauchoride-s23-5pm-3) | [pages](https://ucsb-cs156-s23.github.io/proj-gauchoride-s23-5pm-3/) | [prod](https://proj-gauchoride.dokku-03.cs.ucsb.edu) | [qa](https://proj-gauchoride-qa.dokku-03.cs.ucsb.edu)
| s23-5pm-4 | [repo](https://github.com/ucsb-cs156-s23/proj-gauchoride-s23-5pm-4) | [pages](https://ucsb-cs156-s23.github.io/proj-gauchoride-s23-5pm-4/) | [prod](https://proj-gauchoride.dokku-04.cs.ucsb.edu) | [qa](https://proj-gauchoride-qa.dokku-04.cs.ucsb.edu)

 
## 6pm - happycows

* Customer: Prof. Mattanjah de Vries, Distinguished Prof. of Chemistry, UCSB

| Team | Repo | Github Pages | Prod | QA |
|--|--|--|--|--|
| s23-6pm-1 | [repo](https://github.com/ucsb-cs156-s23/proj-happycows-s23-6pm-1) | [pages](https://ucsb-cs156-s23.github.io/proj-happycows-s23-6pm-1/) | [prod](https://proj-happycows.dokku-05.cs.ucsb.edu) | [qa](https://proj-happycows-qa.dokku-05.cs.ucsb.edu) |
| s23-6pm-2 | [repo](https://github.com/ucsb-cs156-s23/proj-happycows-s23-6pm-2) | [pages](https://ucsb-cs156-s23.github.io/proj-happycows-s23-6pm-2/) |[prod](https://proj-happycows.dokku-06.cs.ucsb.edu) | [qa](https://proj-happycows-qa.dokku-06.cs.ucsb.edu) |
| s23-6pm-3 | [repo](https://github.com/ucsb-cs156-s23/proj-happycows-s23-6pm-3) | [pages](https://ucsb-cs156-s23.github.io/proj-happycows-s23-6pm-3/) |[prod](https://proj-happycows.dokku-07.cs.ucsb.edu) | [qa](https://proj-happycows-qa.dokku-07.cs.ucsb.edu) |
| s23-6pm-4 | [repo](https://github.com/ucsb-cs156-s23/proj-happycows-s23-6pm-4) | [pages](https://ucsb-cs156-s23.github.io/proj-happycows-s23-6pm-4/) |[prod](https://proj-happycows.dokku-08.cs.ucsb.edu) | [qa](https://proj-happycows-qa.dokku-08.cs.ucsb.edu) |
 
## 7pm - courses

* Customer: All UCSB Students, Faculty, Staff and Admins
* Central issues collection: <https://github.com/ucsb-cs156/proj-courses/issues>
  - You can get issues from here to add to your own kanban boards

| Team | Repo | Github Pages | Prod | QA |
|--|--|--|--|--|
| s23-7pm-1 | [repo](https://github.com/ucsb-cs156-s23/proj-courses-s23-7pm-1) | [pages](https://ucsb-cs156-s23.github.io/proj-courses-s23-7pm-1/) | [prod](https://proj-courses.dokku-09.cs.ucsb.edu) | [qa](https://proj-courses-qa.dokku-09.cs.ucsb.edu) |
| s23-7pm-2 | [repo](https://github.com/ucsb-cs156-s23/proj-courses-s23-7pm-2) | [pages](https://ucsb-cs156-s23.github.io/proj-courses-s23-7pm-2/) | [prod](https://proj-courses.dokku-10.cs.ucsb.edu) | [qa](https://proj-courses-qa.dokku-10.cs.ucsb.edu) |
| s23-7pm-3 | [repo](https://github.com/ucsb-cs156-s23/proj-courses-s23-7pm-3) | [pages](https://ucsb-cs156-s23.github.io/proj-courses-s23-7pm-3/) | [prod](https://proj-courses.dokku-11.cs.ucsb.edu) | [qa](https://proj-courses-qa.dokku-11.cs.ucsb.edu) |
| s23-7pm-4 | [repo](https://github.com/ucsb-cs156-s23/proj-courses-s23-7pm-4) | [pages](https://ucsb-cs156-s23.github.io/proj-courses-s23-7pm-4/) | [prod](https://proj-courses.dokku-12.cs.ucsb.edu) | [qa](https://proj-courses-qa.dokku-12.cs.ucsb.edu) |
 
