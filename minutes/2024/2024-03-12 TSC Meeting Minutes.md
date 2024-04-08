# Meeting Minutes for Galasa TSC 12 March 2024

Recording to be made available soon.

Current agenda items:
* Publicity
* Development Containers
* Review TSC Charter together - https://github.com/galasa-dev/TSC/blob/main/galasa-tsc-charter.md
  * Differentiation between voting members and committers for inclusion in the Charter for Galasa
* OMP and IBM Cloud - what is the progress?
* OpenSSF Badge progress - https://www.bestpractices.dev/en/projects/8343
* Open Mainframe Project Mentorship Application for Galasa
* What are the development team working on?
* Blockers to delivery
* AOB

## Attendees

* Louisa Seers
* Jade Carino
* Mike Cobbett
* Caroline McNamara
* Holly Hunt
* Michelle Harris
* Gerald Mitchell
* Fiona Ampofo
* James Davies

## Minutes

Publicity
* Caroline has written a blog about how to get the CLI up and running [link](https://openmainframeproject.org/blog/galasa-preparing-to-get-started-with-the-galasa-cli-on-my-mac/?utm_campaign=Open%20Mainframe%20Project%20Blog&utm_content=285701757&utm_medium=social&utm_source=linkedin&hss_channel=lcp-35545633).
* Dan Donnelly is also in the pipeline for a blog on the OMP.
* Blog ideas around dev containers, publishing test catalogue to an ecosystem, separate update on how to update a Galasa command line to an ecosystem with access tokens.
* SHARE Orlando 2024
  * Will did two sessions - writing an automated test from absolutely nothing on the laptop. Automating a COBOL application into CICS TS.
  * This is the spell book that Will used for the demo > [https://github.com/hobbit1983/SHAREDemo/](https://github.com/hobbit1983/SHAREDemo/)
  * Hack3270 which intercepts a 3270 datastream and can pull out hidden fields or protected fields and flipped bits on them to unprotect them or make them visible. This is used inside enterprises to uncover tricks that were implemented into BMS maps that users had created 30-40 years ago that nobody knew about. Highlight the areas of the map that are concerning - questions around how we would bring the code into Galasa. This code is under GPL.
    * Could Galasa highlight when running a test, highlight fields that are being used whilst running a test.
    * Broadcom mentioned that it's something they're considering so we should talk to Petr/Venkat/Vibhor about it.
    * Michelle agreed that it would also be very useful.
  * IBA Group
    * Big IDEA and Intellij fans. They want to use Galasactl as their base, but put tooling in around supporting Galasa in their IDEA.
    * Invite contact to the TSC - action on Louisa. 
* GSE UK Virtual
  * Two sessions for Galasa - one from the 102 track and one for the AppDev track.
* GSE UK November
  * Louisa and Michelle to think about joint session.
* Enterprise Systems Journal Article - Deadline Monday 18th March
* Discussion with NatWest on Galasa (was mentioned publically on LinkedIn, so felt comfortable to share) and they were enthused by it, Louisa to report if anything else comes of it.
* Conferences Louisa has submitted/is looking at for 2024: OSS EMEA, GSE Nordics, FOSS North, DevOps Pro, OSFF London, All Things Open.

Development Containers

* Dev containers allow you to run your machines within a docker image with all the information inside. It abstracts away from all the information that you may need to get up and running. You get exactly the same result across platforms once you've run the docker image.
* This is to avoid the cross-platform issues that we have previously had with Windows.
* This can remove all the pre-requestites and you would need a docker daemon or podman to use this.
* The containers will allow developers to build without all the different pieces involved. This is only the CLI project for the time being but this should be rolled out to the other projects fairly easily.
* Does the OMP have an image repository?

TSC Charter

* Contributors, committers, and voting members. Role of a contributor and committer is not quite as clear as it could be, if you're not aware of the terms in Github this could be confusing.
* What does it mean to be a voting member?
  * Depends what you're voting about? For example - items on the roadmap.
* What constitues a votable topic and how does it get voted on?
* What is the minimum number of people that is Quorum?
* List who is in what role. We could refer to roles as access roles rather than listing people. Separate file to say who is in what role and how to contact them.
* Series Manager - John Mertic, OMP Director
* All of the regular committers and maintainers of the project would be a technical group.
* Make sure we're happy with who is in which group. These roles now align to expectations - we should be happy with who is in which list.
* We should be careful not to set quorum too high because then you may never get that quorum.
* Action for TSC to review our current voting members that came with the project.

AOB

* Planning to release 0.32.0 next week.
* Voting on a cadence for versions that go out.
* Will has said that it might have a vote from the TSC if we had someone in the committee that wanted to make sure their contributions wanted to go into the new release. If there were problems then that would get voted on.
