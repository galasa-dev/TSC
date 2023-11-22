# 12-09-2023 Galasa TSC Meeting Minutes

## Agenda

- Announcement of Galasa - Press Release etc.
- Galasa publicity (conferences, blogs etc.)
- Galasa Slack Channel – vote on whether to move from separate Galasa workspace to OMP workspace.
- Let the TSC know that the Galasa Iteration Meetings and thrice-weekly scrums have now been set up and have public access. Ask if anyone else wants to be included so Louisa can add to the meeting list.
- Roadmap from Mike C on future items looking ahead.
- What are the development team currently working on?
- Blockers to delivery?
- AOB

## Attendees

• Louisa Seers
• Petr Plavjanik
• Venkat Balabhadrapatruni
• Will Yates
• Jade Carino
• Holly Hunt
• Savvas Kyriacou
• Dom Starkey
• James Davies
• Mike Cobbett

## Minutes

Announce (press release: https://openmainframeproject.org/blog/galasa-bringing-automated-test-commodity-to-open-source/)
- Open Mainframe Summit happened last week (11th September). Successful launch, around 40 people in the room when John M gave a shout out to Galasa. Louisa gave a talk, had some interest from new users.

Publicity
- Blog: https://openmainframeproject.org/announcements/omp-welcomes-galasa-into-its-ecosystem/
- GSE 2023 – talks scheduled by Jade Carino.
- SHARE March 2024 – Will has some talks in the Open-Source track.
- FINOS 2023 – Louisa has a talk scheduled as the second half of the Open Mainframe Summit. Attendance TBC.

Slack channel
- Could add a non-editable message to let users know that we have moved workspace and a link to the new workspace.
- Benefit that it's aligned to Zowe.
- Email the list of people that are on the Galasa channel to let them know.
- Barriers to entry for the two slack channels? Do you need to sign up to extra stuff? – Answers concluded that right now, a user could sign up with no additional issues.
- Would need to make sure we update the Galasa.dev website.
- Existing Galasa workspace, we have two main channels (general and current release), on the OMP slack, can we create multiple channels.
- Create channels: galasa-dev, galasa-users, galasa-tsc.
- Vote has been decided: yes to move to the TSC.

Scrum and Iteration Calls
- Louisa to add Petr, Will and Venkat. No problem with time zone at the moment, Louisa has made the team aware that if we need to move the time, they can let her know.

Roadmap – attached to this issue.
- How to add to the roadmap?
- Raise the issue within the Github page (https://github.com/orgs/galasa-dev/projects/3), then we can raise issues to discuss within the TSC or within the iteration.
- Add a tag if it’s needed discussion within the TSC.
- The stories are broken down into epics and individual stories – bigger development efforts needed to go into the story point.
- Add an item in the Kanban board (https://github.com/orgs/galasa-dev/projects/3) and then turn into an issue – add to the ‘projectmanagement’ repository.
- If a customer asks: https://github.com/galasa-dev/projectmanagement/issues

Infrastructure Cluster
- The infrastructure that Galasa currently sits on for builds is going away, so Mike and the team are currently working with John M on finding alternative funding for IBM Cloud to move.

Highlights of the last month
- Added requestor flag, so it defaults to the user ID of the person using the test (defaulted to unknown previously).
- OMP logo has been added to the Galasa website.
- Renamed executable as users were struggling to work out which file to download.
- If you create a project, you can now choose Maven, Gradle, or both.
- CLI ‘runs get’ can support the –active flag, so you can see what is currently running. Previously, you had to see all the tests that were running.
