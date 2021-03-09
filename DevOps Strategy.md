# DevOps Strategy

- [Objective](#objective)
- [What is DevOps?](#what-is-devops)
- [DevOps Principles](#devops-principles)
    - [Design Ethos](#design-ethos)
- [DevOps Framework](#devops-framework)
    - [Framework Tools](#framework-tools)
- [Automation Framework](#automation-framework)
- [Recommended Reading and Sources](#recommended-reading-and-sources)
    - [Recommended Reading](#recommended-reading)
    - [Additional Sources](#additional-sources)

## Objective

In order to develop any framework, workflow, or toolset, a team must understand the methodologies or technologies it is leveraging to implement said initiative. This level of understanding applies to “DevOps” as a whole as well as principles and frameworks within. What is DevOps? What is its purpose? Is it a tangible asset or theory that cannot be quantified? Is it a role? Is it a tool with a command line?

Many organizations face challenges to properly succeed in DevOps, not because of lack of talent or resources, but due to improper scope or understanding what they’ve set about achieving with obtaining “DevOps”.

This document hopes to guide an organizational understanding of DevOps; its principles, frameworks, and objectives.

## What is DevOps?

As stated, what actually is DevOps? Aside from being a portmanteau of “Development” and “Operations”; DevOps is difficult to define as no great consensus has been adopted and it is a moving target within the industry. Using Wikipedia as a source, even there it is not definitively defined:

> ...suggested defining DevOps as "a set of practices intended to reduce the time between committing a change to a system and the change being placed into normal production, while ensuring high quality"

Even with the great minds of industry, it is still a somewhat elusive term, creating challenges to scope. Which begs the question, if the industry cannot define it, how can we hope to achieve it as an organization? Ultimately, DevOps becomes a cultural and process oriented term more so than an actual toolset or “check box” to be achieved.

As defined by this strategy document, achieving DevOps within an organization is a ***culture*** of:

- Continuous Integration
- Continuous Deployment
- Continuous Improvement
- Continuous Quality

To get a more diversified and deeper understanding, consult the “Recommended Reading” section for in-depth research into the theory and practices. Each of those sources expands on the above in much greater detail.

As with all projects and initiatives, the successful adoption of DevOps is in defining the proper requirements that align its greater theories and methodologies to our organization. Using the above terms as the definition, we will define principles to work within to ensure our successful adoption.

## DevOps Principles

Prior to executing uniform and consistent DevOps practices, principles need to be established to guide the execution and processes. A sort of CONOPS, or Concept of Operations. For our organization, these principles should include the following tenets to ensure effective DevOps is achieved. Each project, product, or solution should evaluate and meet these principles:

1.  Simplicity
2.  Cloud Native
3.  Automated
4.  Secure
5.  Scalable
6.  Cost Optimized

Again, if the solutions do not meet the above considerations, it should be re-evaluated and re-designed until all are achieved or otherwise compensated via other means.

To assist in achieving these principles, a DevOps Framework is outlined below to guide in adoption of this process.

### Design Ethos

In order to accomplish our objectives, the below phrases help drive home a few core principles:

- KISS: Keep It Simple, Scalable
- Simplicity beats complexity every time<sup>1</sup>
- Business processes need to be ironed out before technical pipelines can be implemented <sup>2</sup>

Also keep in mind Conway's Law:

> Any organization that designs a system will produce a design whose structure is a copy of the organization’s communication structure.

## DevOps Framework

To ensure each principle is met and DevOps can be achieved, the below framework should be used for each project or initiative to ensure consistency and uniformity between differing efforts. Each phase in the framework should produce a deliverable that will be used in the succeeding phases. These can and *should* be viewed as cyclical in execution and organizationally adopted. This cyclical execution ensures the ability to enable continuous improvement and an opportunity to evaluate and improve the processes for reach phase.

1.  Requirements
2.  Design
3.  Build
4.  Validate
5.  Release
6.  Deploy
7.  Monitor

> Note: Security should be considered during every phase, with "trust, but verify" scanning processes during #4
> 
> Aside from the Requirements and Design phases, each succeeding phase should be automated in accordance the organization's Automation Framework.

At a minimum, each phase should also involve stakeholders from the following teams:

- Development (Engineering)
- IT Operations (Infrastructure)
- Security

Without involvement from these key stakeholders, the true effect of DevOps (breaking down silos) cannot be achieved.

This framework can also be viewed as a “pipeline” in which to facilitate a DevOps workflow, visualized here as a Kanban board:

![fcb2fb6abdcb463fac3d8eaf030b59b1](https://user-images.githubusercontent.com/16600691/110018925-76f82780-7ced-11eb-9f5e-c8bc555b7ede.png)

### Framework Tools

To accomplish these tasks from a technical perspective, the organization has to standardize on an acceptable "toolbox" to ensure the principles can be met. Every project or initiative should adopt this standardization. Without standardization, chaos is and will prevail throughout the technology teams, thus working directly against DevOps theory.

By adopting a common toolbox, this ensures every initiative conforms to the same tooling and processes throughout the organization.

Aside from client-required contractual obligations or minimal edge cases, this toolbox should be the default tooling in use by the organization to maximize effectiveness and ensure consistency across our entire IT landscape.

As an organizational goal, we should leverage a tool that allows for effective work, but strive to achieve that with the minimalist approach available. More is definitely not better in this regard and will ultimately affect, and work against, DevOps adoption.

Use this table to map DevOps Phase and Tool relationships. Upon completion, review and reduce duplicate/competing tooling to ensure efficiency within the organization.

| Phase | Functional Activities | Tool Examples |
| --- | --- | --- |
| Requirements | Inventory, Identify | JIRA/Confluence/Sharepoint/Slack/Kanban |
| Design | Value Stream Mapping, Planning | Java, Python, Ruby, Value Stream Mappings |
| Build |     | GitLab-CI, Jenkins, Gradle, Maven |
| Validate | Code quality, Security, Functionality | SonarQube, Selenium, JMeter, SOAP UI, SAST/DAST |
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
- The Lean Startup
    - Eric Reis

### Additional Sources

- [12 Factor App](https://12factor.net/)
- [SAFe DevOps Series](https://www.scaledagileframework.com/devops/)
- [DevOps Tools & Frameworks](https://analyticsindiamag.com/devops-tools-frameworks-everything-you-need-to-know)


* * *

<sup>1</sup>Jock Willink
<sup>2</sup>The Phoenix Project
