# DevOps Strategy

- [Objective](#objective)
- [What is DevOps?](#what-is-devops)
- [DevOps Principles](#devops-principles)
  - [Design Ethos](#design-ethos)
- [DevOps Framework](#devops-framework)
  - [Requirements](#requirements)
    - [Metrics](#requirements-metrics)
    - [Deliverables](#requirements-deliverables)
  - [Design](#design)
    - [Metrics](#design-metrics)
    - [Deliverables](#design-deliverables)
  - [Code](#code)
    - [Metrics](#code-metrics)
    - [Deliverables](#code-deliverables)
  - [Build](#build)
    - [Metrics](#build-metrics)
    - [Deliverables](#build-deliverables)
  - [Validation](#validation)
    - [Metrics](#validation-metrics)
    - [Deliverables](#validation-deliverables)
  - [Release](#release)
    - [Metrics](#release-metrics)
    - [Deliverables](#release-deliverables)
  - [Deploy](#deploy)
    - [Metrics](#deploy-metrics)
    - [Deliverables](#deploy-deliverables)
  - [Monitor](#monitor)
    - [Metrics](#monitor-metrics)
    - [Deliverables](#monitor-deliverables)
  - [Framework Tools](#framework-tools)
- [Automation Framework](#automation-framework)
- [Recommended Reading and Sources](#recommended-reading-and-sources)
  - [Recommended Reading](#recommended-reading)
  - [Additional Sources](#additional-sources)

## Objective

In order to develop any framework, workflow, or toolset, a team must understand the methodologies or technologies it is leveraging to implement said initiative. This level of understanding applies to “DevOps” as a whole as well as principles and frameworks within. What is DevOps? What is its purpose? Is it a tangible asset or theory that cannot be quantified? Is it a role? Is it a tool with a command line?

Many organizations face challenges to properly succeed in DevOps, not because of lack of talent or resources, but due to improper scope or understanding what they’ve set about achieving with obtaining “DevOps”.

This document hopes to guide an organizational understanding of DevOps; its principles, frameworks, and objectives; while also aligning to the organization's core values and strategic visions.

## What is DevOps?

As stated, what is DevOps? Aside from being a portmanteau of “Development” and “Operations”; DevOps is difficult to define as no great consensus has been adopted and it is an evolving target within the industry. Using Wikipedia as one source, there it is not definitively defined:

> ...suggested defining DevOps as "a set of practices intended to reduce the time between committing a change to a system and the change being placed into normal production, while ensuring high quality"

Even with the great minds of industry, it is still a somewhat elusive term, creating challenges to scope. Which begs the question, if the industry cannot define it, how can we hope to achieve it as an organization? Ultimately, DevOps becomes a cultural and process oriented term more so than an actual toolset or “check box” to be achieved.

As defined by this strategy document, achieving DevOps within an organization is a ***culture*** and ***tooling*** of:

- Continuous Integration
- Continuous Deployment
- Continuous Feedback
- Continuous Improvement
- Continuous Quality

To get a more diversified and deeper understanding, consult the “Recommended Reading” section for in-depth research into the theory and practices. Each of those sources expands on the above in much greater detail.

As with all projects and initiatives, the successful adoption of DevOps is in defining the proper requirements that align its greater theories and methodologies to our organization. Using the above terms as the definition, we will define principles to work within to ensure our successful adoption.

## DevOps Principles

Prior to executing uniform and consistent DevOps practices, principles need to be established to guide the execution and processes. A sort of CONOPS, or Concept of Operations. For our organization, these principles should include the following to ensure effective DevOps is achieved. Each project, product, or solution should evaluate and meet these principles:

1. Simplicity
2. Cloud Native
3. Automated
4. Secure
5. Scalable
6. Cost Optimized

Again, if the solutions do not meet the above considerations, it should be re-evaluated and re-designed until all are achieved or otherwise compensated via other means.

To assist in achieving these principles, a DevOps Framework is outlined below to guide in adoption of this process.

### Design Ethos

In order to accomplish our objectives, the below phrases help drive home a few core principles:

- KISS: Keep It Simple, Scalable
- Simplicity beats complexity every time
- Business processes need to be ironed out before technical pipelines can be implemented<sup>1</sup>

Also keep in mind Conway's Law:

> Any organization that designs a system will produce a design whose structure is a copy of the organization’s communication structure.

## DevOps Framework

To ensure each principle is met and DevOps can be achieved, the below framework should be used for each project or initiative to ensure consistency and uniformity between differing efforts. Each phase in the framework should produce a deliverable that will be used in the succeeding phases. These can and *should* be viewed as cyclical in execution and organizationally adopted. This cyclical execution ensures the ability to enable continuous improvement and an opportunity to evaluate and improve the processes for each phase.

1. Requirements
2. Design
3. Code
4. Build
5. Validation
6. Release
7. Deploy
8. Monitor

> Security should be integral in every phase, with "trust, but verify" scanning processes during Validation

Aside from the Requirements and Design phases, each succeeding phase should be automated in accordance the organization's Automation Framework and tooling.

At a minimum, each phase should also involve stakeholders from the following teams:

- Development (Engineering)
- IT Operations (Infrastructure)
- Security

Without involvement from these key stakeholders, the true effect of DevOps (breaking down silos) cannot be achieved.

This framework can also be viewed as a “pipeline” in which to facilitate a DevOps workflow, visualized here as a Kanban board:

![fcb2fb6abdcb463fac3d8eaf030b59b1](https://user-images.githubusercontent.com/16600691/110018925-76f82780-7ced-11eb-9f5e-c8bc555b7ede.png)

### Requirements

To define and achieve success, requirements must be obtained. Without requirements, the scope and success of any project will be in jeopardy. In the DevOps sense, the requirements phase should include goals, metrics, and expectations for each DevOps initiative.

Sample questions to answer:

- What automation tools are required (and in accordance with the Automation Framework)?
- Which components should be automated?
- What is the timeline?
- What is the desired end state of this effort?
- Is this scoped correctly to achieve the DevOps [principles](#devops-principles) and frequent releasing?

Keep in mind, these should be scoped and well-defined deliverables. As with any DevOps initiative, preventing scope creep is key to successful implementation.

#### Requirements: Metrics

- Timing
  - Lead Time (timing from assignment to completion time)
  - Cycle Time (timing from beginning of task to completion)
- Number of stakeholders involved.
- Number of requirements to be addressed.

#### Requirements: Deliverables

- Clear expectations of the initiative.
- Achievable metrics to base success.
- Sufficient information to continue into the Design phase.
- Adequate scoping to avoid creepage.
- Publish document detailing the requirements for stakeholder review. 

### Design

Upon clear definition of requirements, the next phase in the cycle is determining the design to meet those requirements.

This design should include the high-level architecture of the pipeline, as well as the technologies that facilitate the continuous movement within the pipeline.

Note, this is not a re-architecture of the application (although it could be required depending on the continuous feedback), but an architecture of the *DevOps* process, to include all facets of the *continuous* DevOps mindset.

Ensure the design accounts for small implementation batches, helping to enable the continuous nature required to achieve DevOps.

- **Always ask**: is this design in compliance with the DevOps principles and ethos?

#### Design: Metrics

- Timing
  - Lead Time
  - Cycle Time
- Number of tools required to achieve requirements.

#### Design: Deliverables

- Simple design that will implement the pipeline.
- Design published for all stakeholders to review.

### Code

The Code phase is the first phase that implements automation and non-human interaction. Upon understanding the requirements and design, the code used to facilitate the product is created. This will vary depending on project and requirements. However, the automation leveraged between the Code and Build phases should be replicated as much as possible between projects to reduce overall effort between projects.

#### Code: Metrics

- Timing
  - Lead Time
  - Cycle Time
- Coding language(s) used for the project.

#### Code: Deliverables

- Source code of the application, ready for the pipeline.
- Automation to initiate the Build phase or completeness for a pull-based build.
- Frequent commits and small, scoped batches or features.
- Target daily commits to initiate the pipeline. 
- Metrics stored in a way to enable monitoring, historical lookup, and comparison.

### Build

The Build phase begins with what should be automated through the rest of the pipeline. During the Build phase, the source code committed in the Code phase is properly built to enable the remaining phases of DevOps.

This build phase will be different depending on the source code; however, the end state should always be the same: a functional binary of code that can be tested and executed.

#### Build: Metrics

The phase should also include automated reporting of standardized build metrics, including:

- Phase Timing
  - Lead Time
  - Cycle Time
- Build Success/Failure
- Individual binary build time (if applicable)
- Build size (if applicable)
- Detailed build times:
  - Start of the build
  - Dependency capture
  - Publishing to repository
  - Artifact cleanup

#### Build: Deliverables

- Binary or other wised package source code.
- Delivery to the common repository for that code type.
- Automated reporting of metrics to relevant stakeholders.
- Metrics stored in a way to enable monitoring, historical lookup, and comparison.

### Validation

The Test phase includes all manner of software or system validation. This should include testing of the individual builds or services to ensure functionality, quality, and security. Any errors during this phase should be reported via automated means to enable prompt response, cycling back to the Code phase.

#### Validation: Metrics

- Phase Timing
  - Lead Time
  - Cycle Time
- Code quality metrics
- Security report and metrics
  - Vulnerability report
  - Number of vulnerabilities
    - High/Medium/Low
- Test metrics
  - What components failed?
  - Percentage of failed components?
  - Duration of each test
  - Historical comparison data

#### Validation: Deliverables

- Pass/Fail assessments:
  - Functional
  - Quality	
  - Security (SAST/DAST/etc.)
  - Additional as required per code type.
- Reporting, detailing the above pass/fail tests, to include:
  - Functional
  - Quality
  - Security
- Metrics stored in a way to enable monitoring, historical lookup, and comparison.

### Release

After successful completion of the Test phase, the workflow automatically continues to release the artifact into a repository or other staging environment for further review/approval. Where applicable to the deliverable, this should also release validated artifacts into a completed system of components for a full end-to-end regression test.

#### Release: Metrics

- Phase Timing
  - Lead Time
  - Cycle Time
- Validation
  - Complete regression test results
  - Test metrics
    - What components failed?
    - Percentage of failed components?
    - Duration of each test
    - Historical comparison data
- Detailed release times:
  - Building of environment or duration of updating existing environment
  - Publishing to repository
  - Artifact cleanup (if applicable)

#### Release: Deliverables

- Delivery into a “Pre-Production” or “Staging” environment
  - Enables complete system regression testing.
- Production-ready release to a repository (i.e. Docker container, Product URL, etc.)
- Metrics stored in a way to enable monitoring, historical lookup, and comparison.

### Deploy

This is the final movement phase of the lifecycle, with the artifacts delivered into an end-state or production environment. Artifacts at this phase should have completed all validation and integrity checks, ensuing a stable, predictable product presented to the customer.

Not all initiatives will require this phase, as some may be delivered offline to a given customer at which point the final state would be the release of a valid artifact to its downloadable or transportable repository.

To orchestrate the release of an artifact, this phase typically consists of tools that leverage:

- Configuration management
- Infrastructure as Code (IaC)

#### Deploy: Metrics

- Phase Timing
  - Lead Time
  - Cycle Time
- Does it require deployment?
- Detailed deployment times:
  - Building of secondary (canary) environment or duration of updating existing environment
  - Artifact cleanup or failover (if applicable)
- Validation metrics
  - Deployment failed?
  - Percentage of failed components?

#### Deploy: Deliverables

- Complete and functional delivery into a production environment.
- Metrics stored in a way to enable monitoring, historical lookup, and comparison.

### Monitor

While all phases require continuous operations to achieve DevOps goals, this is especially important during the Monitor phase. This phase provides continuous observability to the environments deployed during the deployment phase. The deliverables of this phase should provide key metrics to enable continuous feedback and improvement.

#### Monitor: Metrics

- Phase Timing
  - Lead Time
  - Cycle Time
- Application-specific metrics, including:
  - User login times
  - User concurrency
  - Response times
  - Up time
  - Maintenance periods
  - Component availability
  - And many more depending on the application and system deployed.

#### Monitor: Deliverables

- Continuous monitoring of an application, component, or system to provide critical data into the DevOps workflow.
- Metrics stored in a way to enable monitoring, historical lookup, and comparison.

### Framework Tools

To accomplish these tasks from a technical perspective, the organization must standardize on an acceptable "toolbox" to ensure the principles can be met. Every project or initiative should adopt this standardization. Without standardization, chaos is and will prevail throughout the technology teams, thus working directly against DevOps theory.

By adopting a common toolbox, this ensures every initiative conforms to the same tooling and processes throughout the organization.

Aside from client-required contractual obligations or minimal edge cases, this toolbox should be the default tooling in use by the organization to maximize effectiveness and ensure consistency across our entire IT landscape.

As an organizational goal, we should leverage a tool that allows for effective work, but strive to achieve that with the minimalist approach available. More is not better in this regard and will ultimately affect, and work against, DevOps adoption.

Use this table to map DevOps Phase and Tool relationships. Upon completion, review and reduce duplicate/competing tooling to ensure efficiency within the organization.

Upon acceptance and unification of this toolbox within the organization, socialize and hold accountable all stakeholders in the DevOps processes.

This is a sample of the data:

| Phase | Functional Activities | Tool Examples |
| --- | --- | --- |
| Requirements | Inventory, Identify | JIRA/Confluence/Sharepoint/Slack/Kanban |
| Design | Value Stream Mapping, Planning | What Language? (Java, Python, Ruby, etc.), Value Stream Mappings, Version Control |
| Code |     | GitHub, GitLab, TFS, Azure DevOps |
| Build |     | GitLab-CI, Jenkins, Gradle, Maven |
| Validation | Code quality, Security, Functionality | SonarQube, Selenium, JMeter, SOAP UI, SAST/DAST |
| Release |     | Docker, Helm, RPM, WAR, Nexus |
| Deploy |     | Terraform, Ansible, Helm |
| Monitor |     | Grafana, Prometheus, Splunk, Graylog, FluentD, Nessus, Tripwire |

## Automation Framework

Automation, as a component of DevOps (largely the singular focus in most organizations), plays a major role in accomplishing the continuous movement defined by DevOps. As guidance, an Automation Framework should be developed to ensure consistency between various projects or initiatives. This Automation Framework builds from this strategy document by diving deeper into the toolset components, providing a structure for those tools to facilitate autonomy in a standardized fashion.

## Recommended Reading and Sources

### Recommended Reading

These works are recommend reading to understand the full impact and ideals behind DevOps.  They were also used as source material to build this document.

- DevOps Adoption Playbook
  - Sanjeev Sharma
- DevOps Handbook
  - Gene Kim, Jez Humble, Patrick Debois, John Willis
- The Phoenix Project
  - Gene Kim, Kevin Behr, George Spaffort
- The Goal
  - Dr. Eliyahu Goldratt

### Additional Sources

- [12 Factor App](https://12factor.net/)
- [SAFe DevOps Series](https://www.scaledagileframework.com/devops/)
- [DevOps Tools & Frameworks](https://analyticsindiamag.com/devops-tools-frameworks-everything-you-need-to-know)

* * *

<sup>1</sup>The Phoenix Project
