# Galasa TSC Meeting 19th December 2023

## Agenda
- Publicity - anything to celebrate in the last month?
- Where we can store documentation?
- OMP and IBM Cloud - what is the progress?
- What are the development team working on?
- Blockers to delivery
- What about next year - 2024?
- AOB

## Attendees
* Louisa Seers
* Fiona Ampofo
* Eamonn Mansour
* Holly Hunt
* Mike Cobbett
* Jade Carino

## Minutes
Publicity
* DevOps Pro 2024 - Louisa got a session accepted for online 2024
* Mike wrote and recorded a video for the CLI
* Where should the videos go?
* Discussion about whether we should put the videos on the OMP YouTube channel.
* Put the Galasa template up onto Github so that other people could use that as well. Make a note for the retrospective.
* Playbacks for next year - cadence to be confirmed.
* Either a blog or video once a month from the backlog.

How do we store and collaborate on documentation?
* Github may be the best place to put everything.
* Pro and cons for various approaches - for next time.

OMP and IBM Cloud
* Louisa has resent documentation to John Mertic for him to chase.

What are the development team working on?
* The team is currently focused on enhancing security measures in various aspects of their work.
* The Configuration Property Store is a key element of their security efforts. It allows users to extract properties in YAML format, and subsequently, these properties can be applied or recreated by playing back the file.
* Galasa is currently providing support for properties in version 0.31.0. Users can query a user in one system, retrieve a file, and then call it back to another system, facilitating the storage and management of properties in an ecosystem using a CI/CD approach.
* The team aims to minimize direct interaction with etcd, the underlying system holding values. By avoiding direct use of etcd and closing off related ports, users can go through the REST interface, enhancing authentication and overall security.
* While Eclipse is still in use, going through etcd is necessary. The team is working to bridge this gap without concealing the solution.
* Authentication improvements are ongoing, separating the UI's runtime from the services it requires. All UI traffic passes through a REST call into their system before reaching the backend, even for authentication. This approach is designed to enhance security, especially in environments with firewalls.
* Ongoing work includes allowing Eclipse to stop running tests and requeue a running test, still in the early stages.
* Extracting 3270 images from the system via the command line poses a challenge for the team.
* After completing these tasks, the team will consider removing the Eclipse plug-in.
* Implementation of HTTPS certificates is part of the ongoing enhancements.

Blockers for Development
* Access to the OMP 3270 machine.

Looking to 2024
* Louisa wants to spend the January session talking about our goals for 2024, what we want to achieve as a project and then what tactically we need to do to get there. That includes users, technical work and community driving.
