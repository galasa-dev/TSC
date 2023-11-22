# Why has Galasa support for Eclipse been withdrawn ?

## What has been decided
The Galasa support of Eclipse is being withdrawn. This was decided by the Technical Steering Committee on 21st Nov 2023.
Minutes of that meeting are available here: https://github.com/galasa-dev/TSC

## Why withdraw Galasa support for eclipse ?

1. The command-line tool does it all
The `galasactl` command-line tool can do (almost) everything that eclipse can do.
The items it can't do are being scheduled shortly to make the tools equivalent.

2. The Eclipse Galasa plugins require lots of specialised Eclipse skills to maintain, update and improve.
So dropping support for eclipse reduces the burden of support for the small Galasa open-source team.

3. Users find it very hard to install, and keep up-to-date.
Specific versions of base eclipse are needed, which are tricky to download.
Specific versions of Java are needed also, and other combinations of plugins which make keeping a development environment
fully working is a periodic pain whenever you need to upgrade.
The install process for the `galasactl` command-line tool takes seconds, and is pretty fail-safe.
The Galasa team have fielded so many questions on just how to install things into eclipse, and issues which are Eclipse such that it makes supporting the Galasa plugins within eclipse a burden that the small Galasa dev team can no longer afford.

4. Supporting eclipse is slowing down development of other items
Supporting eclipse is taking effort and attention away from the implmenetation of other much-needed improvements to the eclipse framework and ecosystem. Having a large eclipse code-base around makes it harder to progress many of these items without major re-implementation of the Eclipse plugin codebase.
For example: Eclipse contacts all of the back-end services in a Galasa ecosystem, but the Authentication requirements demand that all traffic to the ecosystem goes through a REST interface, so the client can be checked for valid permissions to do things. The authentication item alone would require a re-write of much eclipse function, to route traffic through a rest interface layer, so direct access to etcd/couchdb is not performed. 
Removing eclipse allows us to build-out from a more secure base, and lock-down the ports and access points of the Ecosystem to only REST calls (which can be authenticated with JWTs).

5. Eclipse isn't as popular as it once was
Eclipse has been loosing market share of the IDE market. Jetbrains IntelliJ and Microsoft VSCode together account for more than 80% of the developers worldwide, according to the 2023 survey from Stack Overflow.
Given such unfamiliarity with Eclipse, the pain of supporting it can only get worse, and the bang-for-buck of improving it will be decreasing over time also. The `galasactl` tool can be used in conjunction with any IDE, for example: it can be run within a terminal window on Eclipse, Intellij or Vscode.
It is thought that supporting Eclipse, and not supporting other IDEs can alienate users of those other IDEs, and they are typically reticent to install, learn and use Eclipse if they already use a different IDE.

6. There is a friction between developing test cases in eclipse and wanting to then run those test cases within an Ecosystem as part of a CI/CD pipeline.
The Galasa support within Eclipse does some 'magic' behind the scenes by creating an OBR on-the-fly which is used to launch the test selected by the user. This is fine to begin with, but when the tests have to be dropped into an automated pipeline, suddenly there is a development activity required to understand and create an OBR so that tests can be deployed to an Ecosystem. This 'step' is a barrier between running tests locally and running them remotely which doesn't exist if the CLI tooling is used. OBRs are introduced from day one, and used from day one. The OBR used to launch local tests on the CLI si the same OBR as is used to launch tests on an Ecosystem.


## What we loose by dropping support for Eclipse
1. A point and click interface to launch tests in an ad-hoc manner.
Obviously, not having a UI in which you can choose a selection of tests, and run them locally or in an Ecosystem means there is currently no point-and-click user interface to make such operations simple.
Overall, if a UI is required, it is thought that a web-based UI would be more fitting, as that is again IDE-agnostic, and can be used by non-developers and developers, whereas Eclipse use is only used by the latter of these two groups.
The team would like to expand the Galasa web UI at some point, mostly for test status reporting and monitoring the health of the ecosystem, and ecosystem admin tasks, so future work items in this area is expected in due course.

## Still want Eclipse support ?
Galasa is an open-source project. If you wish to resource the upkeep and enhancement of the Eclipse feature, we would love
to hear from you, and can help facilitate its' revival.
