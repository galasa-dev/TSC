# Meeting Minutes for Galasa TSC 7 May 2024

Recording: https://zoom.us/rec/share/hbsDxPdj_k_P6q0Ch9NvRacltDMqj7KRdZEfyEdRsdBGB2FPXiygAI6hDthU-Daf.qGQLNR_y9Xd9qApz

Current agenda items:
* Galasa 2Q 2024 Roadmap
* Galasa TSC Charter (no voting yet but discussion on how we're getting on)
* OpenSSF Best Practices Badge Progress (https://www.bestpractices.dev/en/projects/8343)
* Version 1 of Galasa - What would be in the new version? What would make it a version 1? When do the TSC need to vote on this?
* AOB / Publicity

## Attendees

* Louisa Seers
* Mike Cobbett
* Savvas Kyriacou
* Kristina Mayo
* Will Bartolomeo
* Vibhor Agarwal
* Valery Aranouski
* Eamonn Mansour
* Uladzislau Kalesnikau
* Fiona Ampofo

## Minutes

Roadmap
* Version 1
 * Focus is to add Security to the ecosystem – move everything to REST calls and add everything to the backend.
 * Move away from Eclipse plugins to the CLI which goes directly over REST to the server.
 * Just turned on authentication in 0.33.0 which shipped last week. You now need a token to access the ecosystem.
  * Can get from the WebUI if you can authenticate in the WebUI.
  * Can be logged into by any of the OAuth providers like Github.
 * Looking at the second item which is the revokable access tokens. This means that right now, any person that loses their laptop loses the token.
 * Java 11 goes out of support in October 2024 so the team are looking to update to Java 17.
  * Two things to consider: what do we build Java with and what version of Java do we run the server-side stuff on.
  * On a local system, what do the teams need for the tests to compile and run.
  * No particular opinions from the team – Issue #.
 * Could probably release V1 without secrets manager.
  * Want etcd to get upgraded before then.
  * Could cope with the new version of CouchDB.
 * Best practices badge progress is going well, Louisa aims to complete by the end of the month: Best Practices Badge.
 * Experimental Managers
  * We know that Db2 managers have made challenges.
  * What is the criteria to be included in the v1.
  * The alpha and beta managers are currently set from the past and could do with updating for V1.
 * Storing user passwords on the user's computer, any plans to change that?
  * Could we draw them from the IDE they run in, the CLI makes that difficult because we can’t draw secrets from the IDE vault (like Eclipse).
  * Zowe uses the OAS secrets manager such as the keychain on MacOS or secrets storage on Windows.
  * Could have a look at who has submitted that code in Github for Zowe.
  * They use it through the Zowe CLI secrets files (Zowe CLI).
 * Next TSC – agenda item for next time – Version 1
* Github Actions
 * Want to move to Github actions because it would be free, and it would use Github which is much more transparent.
 * Visibility of build output is much more transparent.
 * OMP Mentorship program – we have applications out at the moment.
* Q2 2025 – COBOL Check item
 * Ulad mentioned that they were also looking at integrating with COBOL Check on Zowe.

Charter
* Louisa showed the beginning of the PPT that she is putting together to break down the charter so we can work through it together.
* No opinion on that on the call – a lot of new participants.

AOB
* GSE UK went well, there were several sessions – one for Eamonn and Louisa, and another from Will Yates.
* Natwest open source program office call that Louisa presented on.
* Blog about the first quarter of the year and our achievements out on Thursday.
