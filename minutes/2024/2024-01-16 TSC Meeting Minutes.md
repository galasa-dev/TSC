# Galasa TSC Meeting 16th January 2024

## Recording: [Here](https://zoom.us/rec/share/4AQKL-9FrGYFaGkC2icl7wEZ5SrDNEHlwERN5wTujz1dkiUNRmPbuwPbR_ArvKxT.VAWPUf_E9XkrLIqn)

## Agenda
- High level roadmap for 2024 (link to follow)
- Publicity - GSE Virtual Conference CFP opens, Michelle's Planet Mainframe Article
- Goals for 2024, what do we want to aim for as a project?
- Dev Containers
- AOB

## Attendees
* Louisa Seers
* Michelle Harris
* Vibhor Agarwal
* Jade Carino
* Holly Hunt
* Will Yates
* Savvas Kyriacou
* Mike Cobbett
* Eamonn Mansour
* Fiona Ampofo
* Dom Starkey

## Minutes
Roadmap
* Mike walkthrough of the roadmap [here](https://github.com/galasa-dev/TSC/blob/main/minutes/2024/Galasa%20Roadmap%20-%20January%202024.pptx).
* Suggestion to add issue numbers on the roadmap to encourage openness so that we can cross reference the roadmap to Github issues.
* Discussion about the Eclipse plug-in, agreement that we have the CLI which has parity of functionality.

Goals for 2024 [link](https://github.com/galasa-dev/TSC/blob/main/minutes/2024/Galasa%20TSC%20Objectives%20for%202024.docx)
* Louisa walked through the goals, mission, and vision for 2024.
* Moving to Github Actions Pipelines which hasn't been discussed properly. Intention behind that was to not reply on the Github monitor which has been quite unstable since starting in the New Year.
* Choices - moving where the Tekton builds happen into the cluster in the 'Plan A' account, or we could utilise Github Actions. It gives us some good examples beyond Maven repository. It's not as reliable as we need it to be, and the builds that happen in the IBM firewall aren't useful because there isn't transparency
* List problems that are driving that decision in the roadmap.
* Measuring the objectives and users within the galasa team. Potentially reduce the number of slack channels that we currently have.
* Look at measuring using Brew Install and apt-get that could help us measure the use of the project.
* Eamonn has found a counter that can help give a download count to measure the usage of Galasa.
* Difference between the number of downloads and the number of users - do they download it in an automated way?
* The website links for Slack channels are outdated and need 

Publicity
* SHARE Galasa session on the open source track has been submitted.
* Find out who the current owner of the COBOL Check project is, and do a "from unit test to integration test for mainframe software" session.
* DevOps Pro and Open Source Summit is something that we can go to and increase traffic.
* Regular playbacks to be recorded on YouTube.
* We have a media backlog in projectmanagement repository that we can allocate a blog post or video.

Dev Containers
* Bring forward to the next TSC to talk it through. What is the benefit and how it would work?

AOB
* The work for Kafka on the roadmap is to be determined and scoped out by Jade.
