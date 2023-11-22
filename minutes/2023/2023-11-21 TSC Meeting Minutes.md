# 21-11-2023 TSC Meeting Minutes

## Agenda

- Galasa publicity (GSE UK feedback, GSE Virtual, blogs etc.)
- Have we followed through with Galasa Slack Channel? Is it now closed?
- OMP and IBM Cloud - what is the progress?
- Eclipse Plug-In - what is the future of the plug-in? Make a decision if we get quorum.
- What are the development team working on?
- Blockers to delivery
- AOB

## Attendees 

-	James Davies
-	Louisa Seers
-	Mike Cobbett
-	Petr Plavanik
-	Jade Carino
-	Fiona Ampfo
-	Holly Hunt
-	Savvas Kyriacou
-	Eamonn Mansour

## Minutes

Agreed that we would add the meeting minutes as files in the archive.

Galasa publicity (GSE UK feedback, GSE Virtual, blogs etc.)
- Jade gave a session on Testing the Mainframe without Knowing the Mainframe. Michelle gave a session on using Galasa within her internal Macro 4 tests. Well attended, very interactive and great engagement - questions throughout. Jade hasn't spoken to Lewis about GSE Virtual Conference.
- SHARE agenda for Orlando 2024.
- Shout-out to Mike about the great Youtube videos that he has been posting. Mike was asking about how the OMP do it.
- Brainstorm on the videos and blogs that we would want to create - good to have a prioritised list.
- Louisa to set up meeting to brainstorm ideas.
- Jade looking to convert the demo that she did into a blog post. 

Have we followed through with Galasa Slack Channel? Is it now closed?
- Mike put some notices on the slack channel to let them know that they're going, but nobody seemed to move from the Galasa Slack Workspace.
- Will to email everybody individually and freeze new messages so that we force people to move over.
- TSC did vote and get quorum to officially move to OMP Slack, just needs to move officially.

OMP and IBM Cloud - what is the progress?
- Currently the team have moved from the IBM internal cloud officially, however they have had to split the infrastructure in the meantime before we get official confirmation that we can move.
- Louisa to ask John Mertic what the latest is on the IBM Cloud provisioning.

Eclipse Plug-In - what is the future of the plug-in? Decide if we get quorum.
- The IBM position is that we're going to remove it, the team believe that this is the best idea.
- It stops Galasa to move as quickly on some aspects such as security and authentication. Upgrading couchdb and etcdb is difficult because of the Eclipse plug-in.
- CLI has improved significantly over the past year - Eclipse takes up less than 10% of the IDE market - and the belief is that the functionality from the CLI has increased over time. Now, a user has all the functionality of the Eclipse in the CLI apart from debugging looping rogue running tests, and collection of 3270 images that run on an ecosystem.
- Reasons why the IBM team want to step back: have a skills gap for what the project need in terms of taking the Eclipse plug-ins forward, majority of the questions are around how to install into Eclipse rather than the plug-in specifically, the CLI means that the developer doesn’t have a huge step up with the OBR.
- Petr has a VSCode extension but if the CLI is as easy to use and as powerful unless there is a specific reason that it’s more powerful than the CLI would be absolutely fine.
- There has been a vote in the TSC to remove the Eclipse plugin with 9 votes.
- Vote was conducted and the following voting reps agreed: James Davies, Mike Cobbett, Petr Plavanik, Jade Carino, Savvas Kyriacou, Eamonn Mansour, Louisa Seers
- Team will have to make small changes in a number of places to remove the plug-in, for example build processes and documentation.
- After the meeting, Mike C wrote up the arguments for and against in a document [here](./2023-11-21-why-drop-eclipse.md) 

What are the development team working on? See [status](./2023-121-team-status.pdf)
- Docs: restructured docs to be more command-line centric; and Eclipse docs separated from the CLI docs.
- Video on the CLI around developing test cases. Installing, setting up, creating a test, building it, examining it, running locally and then adding to automation.
- Video on the Configuration Property Store around how to install Ecosystem, and how to configure properties.
- Continuous Delivery for 0.30.0 issues.
- CLI Properties get/set – yaml format of output, using yaml in configuration as source to maintain ecosystems, easily pulling properties from one ecosystem and inject into another.
- Linux Foundation Scans – Tidying loose ends by removing and fixing copyright issues, on the way to getting first LF security scan on our code. - #1636
- Authentication – tweaking and testing but mostly developed.
- Next up: HTTPS certificates, CLI killing rogue tests, being able to CRUD streams, and gather 3270 screen images during a test run.
- Start of the next iteration is next week.

Blockers to delivery
- 3270 resource available is vague – good to details as to what that means and how we can get access. That is blocking Galasa moving the test infrastructure to within the IBM firewall.
- Louisa to have an update on the OMP Mainframe for next TSC meetings.

AOB
- Next meeting for the 19th December is absolutely fine.
- Looking at goals for 2024 in the January meeting – Louisa to add to agenda.
