Throughout October I researched four organisations, their project donation and incubation processes, and the requirements they normally ask projects to fulfil to go from a one level of incubation to the next. Here, I'm documenting my findings of each individual org, the elements they have in common, and the steps I believe we should follow to create our own framework. Although many of these processes are more for incubation, I think it'

## 1. Organizations

In my work, I looked into 4 orgs that have documented their processes publicly: the Linux Foundation Networking (LFN), Apache, Eclipse, and the Open Source Geospatial Foundation (OSGeo). Below, I describe each organisation in turn, using the following structure: 

- **Incubation Process**: describes the lifecycle of a project in the org, along with a short description of every step
- **Documents & Guidelines**: lists the documents to submit and guidelines to follow to move from a step to the next in the lifecycle
- **Roles & Approvals**: who is involved and who decides when a project is ready for each transition
- **Additional Notes**: other important elements to consider for that org and its process
- **References**: where the information was retrieved from

### Linux Foundation Networking (LFN)

Our sister organisation, the LFN, is "Linux Foundation's open source networking umbrella". They work on different projects for network infrastructures.

#### Process

![[Pasted image 20261124133030.png]]

Note: Projects don't have to start on step 1. Rather, they can join at a higher level if they already meet its requirements. Additionally, this process isn't linear. Projects can go from graduated to archived, and LTS projects can go back to graduated if development is picked back up.

1. **Candidate:** Project looking to join the LFN group. They get assessment from the LFN into how to be onboarded.
2. **Sandbox:** The entry point for early-stage, new or emerging projects that are still exploring their community, governance and roadmap. They get constant hands-on support and guidance from the LFN.
3. **Incubation:** Projects that follow open source best practices, have a diverse contributor base, adhere to governance principles of the LFN, and cooperate with other LFN projects. They get moderate support from other LFN staff, but are expected to be self managed.
4. **Graduated:** Projects with established communities, constant, stable operation,  and proven governance. They comply with open-source best practices, following them consistently, and can vote on the *Technical Advisory Council* (TAC).
5. **Maintenance or LTS:** Stable, feature-complete projects. They receive bug fixes, security updates, and support, but slower development. They receive less marketing support.
6. **Archived:** Projects that don't have an active community or have not received commits in the previous 12 months.

#### Documents & Guidelines

There's a [series of beautiful tables](https://lf-networking.atlassian.net/wiki/spaces/LN/pages/716406785/LFN+Lifecycle+States+Guidelines#Guidelines) that document different requirements projects need to cover at a certain stage. The following table summarises some of its contents:

| Transition                  | Requirements                                                                                                                                |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| Candidate → Sandbox         | Complete the LF project formation and present to the TAC using the **Candidate Project Template**                                           |
| Sandbox → Incubation        | Show open source best practices, a varied contributor base and open governance, using the **Sandbox Project Template**                      |
| Incubation → Graduated      | Show project maturity, a documented release process, diversity and readiness for self-management                                            |
| Graduated → Maintenance/LTS | Reach a stable state focused on long-term support rather than new development (see the proposed _LFN Maintenance/LTS Project Requirements_) |

#### References
- [LFN Lifecycle States & Guidelines](https://lf-networking.atlassian.net/wiki/spaces/LN/pages/716406785/LFN+Lifecycle+States+Guidelines)
- [LFN's About page](https://lfnetworking.org/about/)

### Apache

#### Process

The following process describes the happy path to incubate a project into the ASF. The steps don't have to happen in this exact order, and repeating steps can happen.

1. Find champion and mentors to prepare proposal. These are all mentors of the ASF
2. Create incubation proposal, refine it, and present it to the incubator committee. [Template](https://cwiki.apache.org/confluence/spaces/INCUBATOR/pages/131468547/New+Posling+Proposal). [Previous proposals](https://cwiki.apache.org/confluence/display/INCUBATOR/Proposals). There's discussion about the proposal.
3. Voting happens on accepting project into incubation program
4. Set project infrastructure up. This can be done by champion or podling community members.
5. Import initial code [Code Import Guide with full details on initial code import](https://incubator.apache.org/guides/transitioning_asf.html), [Software grant (PDF)](https://apache.org/licenses/software-grant-template.pdf), [Contributor License Agreement (PDF)](https://apache.org/licenses/cla-corporate.pdf). 
6. Build community around the 'podling'. Make constant releases and improvements conformant to the [ASF Release Policy](http://www.apache.org/legal/release-policy.html). Releases should follow [Incubator Releases Guide](https://incubator.apache.org/guides/releasemanagement.html#choice_of_disclaimers) 
7. Assess podling readiness with mentor.
8. Discuss graduation with committee. This should include evaluating the maturity of the project, which can be done with help of the [Apache Project Maturity Model](https://community.apache.org/apache-way/apache-project-maturity-model.html).
9. Transfer existing trademarks to ASF
10. Voting on graduation happens
11. Have project be graduated and accepted as part of the ASF

[[Transferring Resources Checklist]]

#### New Responsibilities 
- After graduation, a project becomes responsible for its own Oversight, Security, and Communication

#### References

- Retrieved mostly from the [Apache Incubator Cookbook](https://incubator.apache.org/cookbook/#what_are_the_steps_to_becoming_an_apache_software_foundation_top_level_project)

### Eclipse


*Retrieved from https://www.eclipse.org/projects/handbook/#starting* 

#### Process

1. Proposal
2. Provisioning
3. Incubation
4. Mature
5. Archived

#### Life of a project at the Eclipse Foundation

All projects start in the proposal phase. The Eclipse Foundation offers a proposal [web form](https://www.eclipse.org/projects/handbook/#starting-proposal-document). 

##### Project proposal to provisioning 

![[Pasted image 20261027092708.png]]

- The provisioning process starts with an email to start the paperwork process.
- Legal processes happen before the provisioning stage
- Seems like they don't provide champions or mentors, like the Apache Foundation does ([[Apache Incubator]])

##### Project Phases

![[Pasted image 20261027091404.png]]

#### Incubation 

- Once the project has been moved to the incubation phase, it starts active development.
- Incubation serves as an onboarding process to adopt practices and principles of the [Eclipse Foundation Development Process](https://www.eclipse.org/projects/handbook/#edp). 
- A stable codebase is required before starting incubation
- Checklist to graduate a project
	- Project team has demonstrated that they’re working in an open, transparent, and meritocratic manner
	- Team members are engaged in activities that foster vendor neutrality
	- Team members are faithfully engaging in the IP due diligence process and healthy security/vulnerability management
	- Team members have engaged in a progress review
	- Team members are distributing software

#### Mature phase

- In this state, project members (committers) engage in standard development activities like writing code, running builds, releasing software, and converting active contributors into new committers.

#### References

### Open Source Geospatial Foundation (OSGeo)


https://www.osgeo.org/about/committees/incubation/

https://wiki.osgeo.org/wiki/Incubation_Committee

#### Stages

1. Listing project in OSGeo Website
2. Join OSGeo Community initiative.
3. Being recognised as an OSGeo Project.

#### Evaluation Criteria

The project must be:
- **Technical:** Technical excellence, good end-user documentation and a document release process
- **Social:** Use of open source licenses, collaboration, and open communication with the community
- **Fair:** Contributions treated and accepted in a fair and consistent fashion. They should be protected with a **Code of Conduct**. 


|   OSGeo Community Initiative  | OSGeo Project    |
| --- | --- |
|  ![[Pasted image 20261110131202.png\|300x300]]   |  ![[Pasted image 20261110131208.png\|300x300]]   |


#### Incubation process to get to being recognised

1. Completing the incubation application process and submitting it to the corresponding group
2. Review by the Incubation Committee, evaluated using a [list of criteria](https://wiki.osgeo.org/wiki/Project_Evaluation_Criteria)
3. Choose a mentor for the project. The mentor can be chosen by the org or the project team.
4. A list of all projects accepted for incubation is presented to the OSGeo board of directors
5. Mentor reports incubation status periodically using a [Template](https://wiki.osgeo.org/wiki/Project_Status_Template)
6. IncCom and Mentor agree on project being ready for graduation / full status
7. Chairman of the IncCom presents projects ready for graduation at the next meeting of the Board of Directors. Board of Directors accepts or rejects project graduation.
8. After graduation, a member of the project is selected to report to the foundation board periodically on status.



#### References

