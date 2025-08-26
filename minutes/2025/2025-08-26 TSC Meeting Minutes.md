# Galasa TSC Meeting 26th August 2025

## Recording: [Here](https://zoom.us/rec/play/uEYvO2F9s4QYovKbWT4snol2Y1THPvbFaWIN4y0lEDccx-ci-KsZq1rKMh7rxR6Uc1z_iv26EzFZJGaQ.L5amjOueHvyCJP8l?eagerLoadZvaPages=sidemenu.billing.plan_management&accessLevel=meeting&canPlayFromShare=true&from=share_recording_detail&continueMode=true&componentName=rec-play&originRequestUrl=https%3A%2F%2Fzoom.us%2Frec%2Fshare%2F7z76MUvFYwmHQaktmFjLOlim2bJMANQwFXOPC2xLj9sxLbRAX8HnITAZE-2hIHfb._sqnThSbSog4oaPD)

## Attendees
- Louisa Seers
- Joe Sexton
- Eamonn Mansour
- Jade Carino
- Ian Deeley
- Roger Brooks

## Minutes
* Development Updates
  * Jade presented updates included in version 43 of Galasa. These focused on improving the robustness of run cancellation, ensuring that both individual and grouped runs can be cancelled more reliably. This update also ensures that DSS resources are properly cleaned up after cancellation.
  * The cancellation functionality is currently only available via the CLI, but the web UI now reflects the cancellation status of runs.
  * Several security-related upgrades were made, including updates to Golang packages (net and crypto) and the Kafka client library to address vulnerabilities.
  * The team has fully transitioned away from Travis CI, which was previously used for internal documentation builds. All documentation is now hosted on GitHub wiki pages.
  * A cookie consent banner was added to the external documentation site (galassa.dev) to comply with EU legislation.
  * The infrastructure was improved by replacing a wildcard TLS certificate with individual certificates for each subdomain, enhancing security and aligning with Linux Foundation best practices.
* Web UI Enhancements
  * The web UI now supports German translation, contributed by external contributor Chervin Beeson, who is also continuing to work on further enhancements.
  * Users can now personalize their experience by selecting their preferred date-time format and time zone.
  * A health indicator has been added to the footer of the UI to show the status of the Galasa service.
  * Major improvements were made to the test run interface. Users can now search for test runs using various filters (e.g., time frame, tags, status), view metadata and artifacts directly in the browser, and share permalinks to specific runs.
  * The run log is now searchable within the UI, with support for filtering by message type (e.g., error, warning, info) and copying specific log sections.
  * Users can customize the test run table by hiding or reordering columns and saving their preferred layout.
  * The team is working on allowing users to save queries in the UI for reuse, and on improving resource cleanup for manager-allocated resources in the event of test failures or hangs.
* Community Contributions
  * Shivam, a student contributor, successfully added German translation support and found the development environment accessible thanks to recent improvements. Eamonn noted that contributors can now run the web UI locally while connecting to a remote backend, simplifying setup.
  * Louisa highlighted the importance of student contributions and how projects involving popular technologies like GitHub Actions and UI development tend to attract more engagement.
* Conference Planning
  * Joe Sexton shared plans to present at GSE UK on November 3rd, focusing on how his team is adapting existing tests to run with Galasa by generating Java files from current test definitions. This approach avoids the need to rewrite thousands of tests manually and improves traceability of test failures.
  * Jade will also be presenting at GSE UK on the Tuesday, with a session titled “Testing Mainframe as a Newbie Mainframer.”
  * Louisa, who is chairing the App Dev track, confirmed she will attend both sessions and encouraged collaboration between presenters.
* Closing Remarks
  * Louisa praised the UI improvements and emphasized their value in showcasing Galasa at conferences. She noted that the updates are generating positive attention on social media and within the Z community.
  * She encouraged the team to continue sharing progress publicly and thanked Jade for the development update.
  * The meeting concluded with a brief discussion of upcoming events, blog posts, and continued collaboration.
