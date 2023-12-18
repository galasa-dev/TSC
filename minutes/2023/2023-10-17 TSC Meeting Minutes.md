# 17-10-2023 Galasa TSC Meeting Minutes

## Recording: [Here](https://zoom.us/rec/share/szh2CNGDxewtOUiUA4akEb6EkTmEJc6qTzBv-1cGoAWkwoIQdGc3kh9DSYprhJM8.U9TO17LX4tMz9MgF)

## Agenda

- Publicity
- Slack channel update
- Blockers
- Cluster infrastructure progress
- Whats in 0.30.0
- Whats planned in 0.31.0
- How might we get a 3270 resource accessible from the IBM cloud to test our 3270 functionality against
- When can we deprecate and retire eclipse plugins for Galasa. Under what conditions could we do that ?

## Minutes

Publicity
- GSE conference in 2 weeks
- Share submissions have gone
- GSE Nordics have 'come up' - live demo of creating tests from scratch needs adding.
- @hobbit1983 is investigating further.
- Publicity of the new galasa properties get functionality (new in 0.30.0).
- Video introducing CPS
- Whats in the 0.30.0 release
- Look in the KanBan board, there is a column "Done in this release". https://github.com/orgs/galasa-dev/projects/3/views/1

Release notes will be published on galasa.dev website, but summary:
- Cluster move
- Release of 0.30.0
- galasactl properties get/set/delete commands.
- OMP-owned cloud account

PII questionaire
- @louisa-seers chasing up with John Mertec.
- Access to 3270 resource outside of the IBM firewall ?
- OMP may have access to a mainframe.
- First step @louisa-seers to talk to John Mertec to see if we can have any access.
- Question about should we deprecate/retire/remove eclipse plugins ?

AOB
- Lots of discussion on about this in the meeting (see transcript). eg: Reasons why we want to do this.
- What conditions which need to be met before we can think about this:
- CLI to be able to pull 3270 images into files from tests run on ecosysyems
- CLI ability to kill a running test
- CLI ability to create an OBR project for projects which don't have one
- Add this to the agenda to the next TSC meeting
