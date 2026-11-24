Throughout October I researched four organisations, their project donation and incubation processes, and the requirements that both of these processes have. Because both processes are related, and both were part of my research, I've created a separate write-up about project incubation in <TODO: Insert link here>, in case this is something we want to implement too.

This text is broken down in three parts:
1. The organisation I researched and their processes
2. The elements they have in common
3. My recommendations

## 1. Organisations

In my work, I looked into 4 orgs that have documented their processes publicly: the **Linux Foundation Networking** (LFN), Apache, Eclipse, and the Open Source Geospatial Foundation (OSGeo). Below, I describe each organisation in turn, using the following structure: 

- **Donation Process**: the steps that projects go through to be transferred into an org or foundation
- **Documents & Guidelines**: the forms, guidelines, and other documents required for each part
- **Roles & Approvals**: who is involved and who signs off on the donation
- **Additional Notes**: other important items we should consider, including what the original owner keeps
- **References**: where I found this information

---
### 1.1 Linux Foundation Networking (LFN)

Our sister organisation, the LFN, is "Linux Foundation's open source networking umbrella". They work on different projects for network infrastructures.

#### Donation Process

1. **Get familiar with the LFN:** Read [Getting Started With LFN](https://lf-networking.atlassian.net/wiki/spaces/LN/pages/15634966/Getting+Started+With+LFN), the [Upstream First Best Practices Guide](https://lf-networking.atlassian.net/wiki/x/wCbv), the [LFX for LFN guide](https://lf-networking.atlassian.net/wiki/x/8knv) and the [LF Networking landscape](https://landscape.lfnetworking.org/).
2. **Choose a stage:** Review the [Lifecycle States and Guidelines](https://lf-networking.atlassian.net/wiki/spaces/LN/pages/716406785/LFN+Lifecycle+States+Guidelines), the [Project Review Process](https://lf-networking.atlassian.net/wiki/spaces/LN/pages/15645972) and the [Tools and Services](https://lf-networking.atlassian.net/wiki/spaces/LN/pages/15692692) that are available at each state to inform your decision.
3. **Prepare the proposal:** Create a [Project Proposal](https://lf-networking.atlassian.net/wiki/spaces/LN/pages/15638426/Project+Proposals) and fill in the [Project Data Template](https://wiki.lfnetworking.org/x/L4QKBg) with project information, milestones and deliverables, and submit it to the LFN wiki.
4. **Preliminary outreach:** Email LFN staff and the Technical Advisory Council (TAC).
5. **Review period:** Submit the proposal and data template to the TAC at least two weeks before the review. They may also request more information or meetings.
6. **Formal application:** Present the proposal to the TAC. Wait then for a review by the TAC and, possibly, the Governing board.
7. **Approval and onboarding:** LFN staff guide the project members through onboarding of its services and tools. Assets related to the project must be moved to neutral ownership. 
8. **Announcement and post-induction:** The project becomes public and starts using LFN resources.

#### Documents & Guidelines

| Step                 | Documents / guidelines                                                                                                                                                                                                                                                                                                                                                |
| -------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Proposal             | [Project Proposal Powerpoint Template](https://lf-networking.atlassian.net/wiki/spaces/LN/pages/15638426/Project+Proposals) and the **[Project Data Template](https://wiki.lfnetworking.org/x/L4QKBg)**                                                                                                                                                               |
| Hosting requirements | An open source licence for the code, support from a Linux Foundation (LF) member, and agreement to neutral ownership of project assets.|
| Trademark            | The LF or the project's legal entity must own the project's trademark ([LF Projects Trademark Policy](https://lfprojects.org/policies/trademark-policy/))                                                                                                                                                                                            |
| Domains              | Domains are transferred to the LF's domain registrar. Projects must then decide whether to also move their DNS to that of the LF. After preparing the domain, a ticket about this transfer must be raised.                                                                                                                  |
| Repositories         | The LF must have access to every GitHub organisation used to host the project's code.                                                                                                                                                                              |
| Legal entity         | LFN technical projects are set up as series of LLCs.                                                                                                                                                               |
| Policies             | [LF Projects Code of Conduct](https://lfprojects.org/policies/code-of-conduct/) and [Anti-Trust Policy (PDF)](https://r.lfnetworking.org/Antitrust%20Slide.pdf)                                                                                                                                                                                                       |

#### Roles & Approvals

- **LFN staff:** They are the first point of contact for any project and must guide it through onboarding.
- **Governing Board:** A group that may review proposals.
- **Technical Advisory Council (TAC):** Handles project introductions and reviews proposals.

#### Additional Notes

- Projects don't have to start on step 1. Rather, they can join at a higher level if they already meet its requirements. This means donation doesn't always lead to incubation.

#### References

- [How to Join the LFN as a Project](https://lf-networking.atlassian.net/wiki/spaces/LN/pages/15692670)
- [LFN Project Induction](https://lf-networking.atlassian.net/wiki/spaces/LN/pages/1221656579/LFN+Project+Induction)
- [LFN Lifecycle States & Guidelines](https://lf-networking.atlassian.net/wiki/spaces/LN/pages/716406785/LFN+Lifecycle+States+Guidelines)
- [Why host your project at the Linux Foundation (PDF)](https://www.linuxfoundation.org/hubfs/Why%20Host%20a%20Project.pdf?hsLang=en)
- [Open Source Communities and Trademarks: A Reprise (LF blog)](https://www.linuxfoundation.org/blog/2020/07/open-source-communities-and-trademarks-a-reprise/)
- [LF IT services onboarding (domains, email, GitHub)](https://confluence.linuxfoundation.org/x/cKayAQ)

---

### 1.2 Apache Software Foundation (ASF)

#### Donation Process

1. **Proposal accepted:** Donation happens after the IPMC votes to accept the project into the incubator (see [[Project Incubation]] and [A Guide To Proposal Creation](https://incubator.apache.org/guides/proposal.html)).
2. **Sign the agreements:** For a corporate contribution, the [Software Grant Agreement (SGA)](https://apache.org/licenses/software-grant-template.pdf) or [Corporate CLA (CCLA)](https://apache.org/licenses/cla-corporate.pdf) must be completed, submitted and received by Apache **before** any code is imported. For code made of individual contributions, the import is safe once the major contributors (by volume) have completed [Individual CLAs (ICLAs)](https://www.apache.org/licenses/icla.pdf) or SGAs. See [ASF Contributor Agreements](https://apache.org/licenses/contributor-agreements.html) for how to submit them.
3. **Record the import publicly:** Attach the code to a JIRA ticket and tag the previous version control revision, so the exact imported version can be identified. If the import isn't attached to JIRA, it must be committed to version control.
4. **Audit cryptography:** Check the code against Apache's [cryptography guidance](http://www.apache.org/dev/crypto.html) and report any restricted cryptography.
5. **Import the code:** The incoming community chooses whether to import a snapshot of the latest code or a full export with history. The source is first committed unchanged (e.g. to `${project}/trunk/import`) with its original headers and notices, plus the standard LICENSE and an appropriate NOTICE file. The commit message must include the JIRA ticket URL, the original copyright owner and notes on the related paperwork.
6. **Clean up the code:** In a series of separate commits, replace headers with the standard Apache headers (see the [source headers policy](http://www.apache.org/legal/src-headers.html)), make sure LICENSE and [NOTICE](http://www.apache.org/legal/src-headers.html#notice) are correct, move copyright attributions from source files into NOTICE (one owner per commit) and audit for licensing issues. This can start before the import but must be finished before any release.
7. **Move the project's home:** Optionally repackage the code under the Apache namespace, update documentation and build files (e.g. Maven `groupId`, `scm`, `licenses`) and move development to an Apache issue tracker.
8. **Transfer trademarks:** If the donors own trademarks the project needs, they are transferred to the ASF before graduation.

#### Documents & Guidelines

| Step                     | Documents / guidelines                                                                                                                                                                                                                                                                 |
| ------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Corporate donation       | [Software Grant Agreement (PDF)](https://apache.org/licenses/software-grant-template.pdf) and/or [Corporate Contributor License Agreement (PDF)](https://apache.org/licenses/cla-corporate.pdf)                                                                                        |
| Individual contributions | [Individual Contributor License Agreements (ICLAs)](https://www.apache.org/licenses/icla.pdf) from the major contributors                                                                                                                                                              |
| Code import              | [Code Import Guide](https://incubator.apache.org/guides/transitioning_asf.html): JIRA record, [cryptography audit](http://www.apache.org/dev/crypto.html), header and LICENSE/NOTICE clean-up ([source headers policy](http://www.apache.org/legal/src-headers.html)), licensing audit |
| IP clearance             | [Podling IP Clearance](https://incubator.apache.org/guides/ip_clearance.html)                                                                                                                                                                                                          |
| Documentation            | [Apache Branding Guide](https://incubator.apache.org/guides/branding.html), with disclaimers where appropriate                                                                                                                                                                         |
| Trademarks               | Trademark transfer to the ASF (the Cookbook notes the detailed guidance is still to be written). See also the [Podling Name Search Guide](https://incubator.apache.org/guides/names.html)                                                                                              |

#### Roles & Approvals

- **Donor (copyright owner):** signs the Software Grant or CCLA. Major individual contributors sign ICLAs.
- **Mentors:** help the podling with the LICENSE and NOTICE files and the clean-up.
- **Incoming community:** decides whether to import a snapshot or the full history, and agrees the issue-tracker transition on the public dev@ list.
- **Incubator PMC (IPMC):** must have accepted the project before the import.

#### Additional Notes

- **Donating means giving up control:** the project and its trademarks belong to the ASF once donated.
- **Order matters:** the agreements must be received before the code is imported, and the licensing clean-up must be finished before the first release.
- **No early publicity:** podlings can't issue press releases about joining the ASF before the IPMC accepts them (see the [Podling Publicity/Media Guidelines](https://incubator.apache.org/guides/publicity.html)).

#### References

- [Apache Incubator Cookbook](https://incubator.apache.org/cookbook/#what_are_the_steps_to_becoming_an_apache_software_foundation_top_level_project)
- [Code Import Guide (Transitioning to the ASF)](https://incubator.apache.org/guides/transitioning_asf.html)
- [ASF Contributor Agreements](https://apache.org/licenses/contributor-agreements.html)
- [Individual Contributor License Agreement (PDF)](https://www.apache.org/licenses/icla.pdf)
- [Software Grant Agreement (PDF)](https://apache.org/licenses/software-grant-template.pdf)
- [Corporate Contributor License Agreement (PDF)](https://apache.org/licenses/cla-corporate.pdf)

---

### 1.3 Eclipse Foundation

#### Donation Process

1. **Proposal and trademark assignment:** The project submits a proposal through the [proposal web form](https://www.eclipse.org/projects/handbook/#starting-proposal-document). During the proposal phase, any existing trademark for the project name must be assigned to the Eclipse Foundation before the project is created.
2. **Creation review:** The one-week creation review also elects the initial committers.
3. **Committer agreements:** The EMO emails each listed committer to collect their agreement (see [Committer Paperwork](https://www.eclipse.org/projects/handbook/#paperwork)). Provisioning only starts once at least one committer's agreement has been received and processed by the EMO Records Team.
4. **Provisioning:** The Infrastructure Team provisions the project's resources.
5. **Initial contribution:** The project pushes its existing code to the official repository, which automatically starts an initial contribution review.
6. **IP review:** The EMO IP Team reviews the code and any third-party content. Builds can be made before then, but official releases need IP approval.
7. **Ongoing contributions:** Contributors who aren't committers sign the [Eclipse Contributor Agreement (ECA)](https://www.eclipse.org/legal/eca/) before contributing.

#### Documents & Guidelines

| Step                                     | Documents / guidelines                                                                                                                                                                                                                                       |
| ---------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Trademark                                | Assignment of any existing project-name trademark to the Eclipse Foundation                                                                                                                                                                                  |
| Committers employed by an Eclipse member | **[Member Committer and Contributor Agreement (MCCA)](https://www.eclipse.org/legal/committer_process/EclipseMemberCommitterAgreement.pdf)**, signed by the member organisation                                                                              |
| Other committers                         | **[Individual Committer Agreement (ICA)](https://www.eclipse.org/legal/committer_process/EclipseIndividualCommitterAgreement.pdf)**, for committers whose employer isn't a member or hasn't signed an MCCA, or who are self-employed, unemployed or students |
| Non-committer contributors               | **[Eclipse Contributor Agreement (ECA)](https://www.eclipse.org/legal/eca/)**, confirming they license their contributions under the project's licences and have the right to contribute them (see the [ECA FAQ](https://www.eclipse.org/legal/eca/faq/))    |
| Initial contribution                     | Push of the existing code + initial contribution review + IP review of project code and third-party content                                                                                                                                                  |
| Copyright headers                        | Consistent copyright headers naming the copyright holder and licence, using an SPDX-License-Identifier                                                                                                                                                       |

#### Roles & Approvals

- **Eclipse Management Organisation (EMO):** schedules the creation review and sends out the committer agreements.
- **EMO Records Team:** processes the committer agreements.
- **EMO IP Team:** reviews the initial contribution and third-party content.
- **Committers:** manage the IP review process, with help from contributors where needed.

#### Additional Notes

- **Copyright stays with the contributors:** Eclipse doesn't require copyright transfer. Under the ECA, contributors keep ownership of their contributions and grant a licence instead.
- **Trademarks go to the foundation:** the Eclipse Foundation asserts ownership of all project name trademarks.
- **Legal work comes first:** unlike Apache, where the trademark transfer can happen just before graduation, Eclipse handles trademarks and agreements before or during provisioning.
- Contacts for agreement questions: the EMO Records Team ([emo-records@eclipse-foundation.org](mailto:emo-records@eclipse-foundation.org)) or [license@eclipse-foundation.org](mailto:license@eclipse-foundation.org).

#### References

- [Eclipse Foundation Project Handbook – Starting a Project](https://www.eclipse.org/projects/handbook/#starting)
- [Eclipse Foundation Project Handbook – Committer Paperwork](https://www.eclipse.org/projects/handbook/#paperwork)
- [Eclipse Foundation Project Handbook (full)](https://www.eclipse.org/projects/handbook/)
- [Eclipse Foundation Legal Resources](https://www.eclipse.org/legal/)

---

### 1.4 Open Source Geospatial Foundation (OSGeo)

OSGeo's model is closer to **affiliation** than donation. Projects at the lower tiers (listed on the website, OSGeo Community initiative) stay independent, and the sources don't describe any transfer of copyright or trademarks even for full OSGeo Projects. The legal step is a check that the project has the right to be distributed as open source.

#### Donation Process

1. **Website listing:** The project shows it has a geospatial focus, an open source licence and accepts contributions (see the [Add a project](https://www.osgeo.org/community/getting-started-osgeo/add-a-project/) guide and the [Step 1 wiki checklist](https://wiki.osgeo.org/wiki/Incubation_Committee#Step_1:_Add_OSGeo_Website_Project_Page)).
2. **Community initiative:** The project's licence must be [OSI-approved](https://opensource.org/licenses), and its source code headers are checked (see [OSGeo Community Projects](https://wiki.osgeo.org/wiki/OSGeo_Community_Projects) and the [Step 2 wiki checklist](https://wiki.osgeo.org/wiki/Incubation_Committee#Step_2:_Join_OSGeo_Community_Projects_Initiative)).
3. **Incubation application:** The project applies to become an OSGeo Project through the [application form](https://www.osgeo.org/about/committees/incubation/application/), after joining the [incubator mailing list](https://lists.osgeo.org/mailman/listinfo/incubator) (see [[Project Incubation]] and the [Step 3 wiki guide](https://wiki.osgeo.org/wiki/Incubation_Committee#Step_3:_Incubation_process_and_Graduation)).
4. **Provenance review / source code audit:** During incubation, a review confirms that the project is open source and that the team has permission to distribute its code.
5. **Graduation:** The Board appoints the project team as a new OSGeo committee, which gives it access to an OSGeo budget and some liability insurance.

#### Documents & Guidelines

| Step                 | Documents / guidelines                                                                                                                                                                                                       |
| -------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Website listing      | [Add a project](https://www.osgeo.org/community/getting-started-osgeo/add-a-project/) guide                                                                                                                                  |
| Community initiative | [OSI-approved licence](https://opensource.org/licenses) with checked source code headers ([OSGeo Community Projects](https://wiki.osgeo.org/wiki/OSGeo_Community_Projects))                                                  |
| Incubation           | [Application form](https://www.osgeo.org/about/committees/incubation/application/) and [Project Evaluation Criteria](https://wiki.osgeo.org/wiki/Project_Evaluation_Criteria)                                                |
| Provenance review    | Graduation checklist ([PDF](https://github.com/OSGeo/osgeo/blob/master/incubation/documents/graduation_checklist.pdf) / [Markdown](https://github.com/OSGeo/osgeo/blob/master/incubation/documents/graduation_checklist.md)) |

#### Roles & Approvals

- **Mentor:** helps the project obtain legal counsel during incubation.
- **Incubation Committee (IncCom):** oversees the provenance review as part of incubation.
- **Board of Directors:** appoints the graduated project as an OSGeo committee.

#### Additional Notes

- OSGeo flags two kinds of project as not fitting its open source spirit: projects that require a data licence to unlock functionality, and projects published without any governance or developers.
- I couldn't load the graduation checklist to confirm its exact legal and ownership items (e.g. whether OSGeo asks to hold trademarks or domains). It's worth reading it directly before relying on this section.

#### References

- [OSGeo Incubation Committee (website)](https://www.osgeo.org/about/committees/incubation/)
- [Incubation Committee (wiki)](https://wiki.osgeo.org/wiki/Incubation_Committee)
- [OSGeo Incubation Process](https://www.osgeo.org/about/committees/incubation/incubation-process/)
- [OSGeo Community Projects](https://wiki.osgeo.org/wiki/OSGeo_Community_Projects)
- [Graduation checklist (Markdown)](https://github.com/OSGeo/osgeo/blob/master/incubation/documents/graduation_checklist.md)

---

## 2. Comparison

|                            | LFN                                                         | Apache (ASF)                                                            | Eclipse                                                         | OSGeo                                                   |
| -------------------------- | ----------------------------------------------------------- | ----------------------------------------------------------------------- | --------------------------------------------------------------- | ------------------------------------------------------- |
| **When donation happens**  | During onboarding after TAC approval                        | After IPMC acceptance, before code import; trademarks before graduation | During proposal (trademark) and provisioning (agreements, code) | No formal transfer; provenance review during incubation |
| **Code / copyright**       | Open source licence required                                | Software Grant or CCLA, plus ICLAs from major contributors              | Contributors keep copyright and license it (MCCA / ICA / ECA)   | Project keeps it; licence and provenance checked        |
| **Trademarks**             | Owned by the LF or the project entity                       | Transferred to the ASF                                                  | Assigned to the Eclipse Foundation                              | Not described                                           |
| **Domains & repositories** | Domains move to the LF registrar; LF gets GitHub org access | Moved to ASF infrastructure                                             | Provisioned by the Eclipse Infrastructure Team                  | Not described                                           |
| **Legal review**           | Not described in the joining guide                          | Cryptography and licensing audit; header and NOTICE clean-up            | EMO IP review of code and third-party content                   | Provenance review / source code audit                   |
| **Who signs off**          | TAC (and possibly the Governing Board)                      | IPMC                                                                    | EMO                                                             | IncCom → Board of Directors                             |

### Common Elements

These documents and legal processes appear in all four frameworks.

|Common element|Type|LFN|Apache (ASF)|Eclipse|OSGeo|
|---|---|---|---|---|---|
|**Written proposal / application**|Document|Project Proposal + Project Data Template|Podling proposal (template)|Proposal (web form)|Incubation application form|
|**Open source licence requirement**|Legal process|Open source licence (e.g. OSI-approved) required to be hosted|Code relicensed under Apache headers with LICENSE and NOTICE files|Contributions licensed under the project's licences (ECA), with SPDX licence headers|OSI-approved licence, with source code headers checked|
|**Legal / IP review of the code**|Legal process|Intake code scan for basic security and licence compliance|Licensing and cryptography audit during code import|EMO IP review of the initial contribution and third-party content|Provenance review / source code audit|
|**Formal review and approval by a governing body**|Process|TAC review (and possibly the Governing Board)|IPMC vote|EMO creation review|IncCom review → Board of Directors|
|**Ongoing status documentation**|Document|Project Data Template, updated at every lifecycle review|Podling reports (monthly, then quarterly)|Progress and release reviews|Project status reports from the mentor (Project Status Template)|