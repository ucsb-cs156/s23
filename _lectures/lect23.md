---
title: "Week 08 - 05.24 Wed"
lecture_date: 2023-05-24
description: "Sprint Planning continued"
ready: true
layout: default
parent: lectures
---

# Reminder: CATME survey due Thursday midnight

But please do it tonight to avoid further spam in your inbox, and anxiety for Prof. Conrad

# Sprint Planning for Legacy Code project

The detailed instructions below are repeated from yesterday.  Here's the short version:

* Each team already has a Kanban board setup for the legacy code project (see links below).
* You should add the `In Review` column if it is not already present.
* Then, populate your todo column with issues (which may require more than just copy/paste; you'll need to break big things down into smaller things)
* Before you leave today, every team member should be assigned to start on something.
* Every team member should *always* be assigned to at least one in progress issue until your team is done with the project.

# Details

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
 
