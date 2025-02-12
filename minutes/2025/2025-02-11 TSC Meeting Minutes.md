# Galasa TSC Meeting 11th February 2025

## Recording: [Here](https://zoom.us/rec/play/DJXztdC1tP9ekasCswyFhYI-RHAQtZNXFUb7K4RUH0_iwoYfM9jhboig2ySvT4W9-JqC5G5IOcqbchgA.Lz1FEiicDQpec-lb?canPlayFromShare=true&from=share_recording_detail&continueMode=true&componentName=rec-play&originRequestUrl=https%3A%2F%2Fzoom.us%2Frec%2Fshare%2FuvnllMqt1VY86fugq7BGlrcBeAhWSsf_dqp1o2jZJGSGi0o0ac8i7XsCSOS4wkp4.i5MpuIKTg2hGaZjs)

## Agenda
- Publicity & Conferences
- Development Update
- Roadmap Update
- AOB

## Attendees
* Louisa Seers
* Jade Carino
* Mike Cobbett
* Joe Sexton
* Eamonn Mansour
* Roger Brooks

## Minutes
Welcome and Introductions
- Joe introduced himself as part of the Macro 4 team and explained his role and interest in Galasa.

Recording and Sharing Development Updates
- Louisa suggested sharing development updates on YouTube for transparency and engagement. Mike agreed to record sessions and assess the quality before publishing.

Development Updates (Mike Cobbett)
- Version 0.38 (December Release):
  - Introduction of encrypted secrets in Galasa Service.
  - Upgrade of dependencies to improve security and maintain up-to-date libraries.
- Version 0.39 (January Release):
  - Improvements to test result grouping for easier querying.
  - Consolidation of Java repositories into a monorepo for easier contributions.
  - Standardized versioning for better clarity.
- Version 0.40 (Upcoming – End of February):
  - Changes to CPS properties, allowing blank values and ‘@’ in names.
  - Support for customizable Z/OS login prompts.
  - Introduction of role-based access control (RBAC) with different user roles (tester, admin, owner).
  - Support for forks to streamline open-source contributions.
Roadmap and Future Development Plans
- Planned features include:
  - Security Improvements: Expiry times for access tokens, HTTPS inside clusters, encrypted local credentials.
  - Web UI Enhancements: Improved visibility of test cases, test runs, and logs, along with success/failure charting.
  - Repository and Service Upgrades: Updating the etcd version for better security and authentication options.
  - Expanded Configuration Options: Support for password-protected Maven repositories and improved handling of HTTPS certificates for external test connections.
  - Scaling Improvements: Continued work on infrastructure for efficient test execution.

Discussion on Galasa Usage and Contributions
- Joe’s team is evaluating Galasa as a potential replacement for their internal test ecosystem. They primarily use local Galasa rather than the service for stability. Their framework processes test definitions differently from Java-based Galasa tests, requiring a custom interpreter.
- Parallel Testing Challenges: Joe raised concerns about running tests that require multiple interactive screens within the same test execution. Mike noted that multiple Galasa instances can run in parallel if they use separate home folders, but shared folders can cause contention issues. Joe mentioned timing constraints when synchronizing multiple interfaces, which may need further investigation.

Conference Submissions and Upcoming Events
- GSE UK Virtual Conference (April 29 - May 1): Call for papers is open. Past sessions have included both introductory and advanced Galasa topics. Discussion on the most suitable tracks, with 102 and Open Mainframe Project tracks being the most relevant. Jade confirmed availability on Thursday and is considering submitting a talk.
