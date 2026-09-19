# Stakeholder Discovery Plan

## Discovery Approach

Following the initial conversation with the VP of Customer Experience, I will conduct additional discovery conversations with the stakeholders identified in the stakeholder analysis. The goal of these conversations is to build a more complete understanding of the problem from the perspectives of the teams involved before defining requirements or evaluating potential solutions.

Each stakeholder conversation will follow a consistent overall structure while including questions specific to that stakeholder's role and area of expertise.

For each conversation, I will:

1. **Share and validate the current problem statement.** I will explain my current understanding of the problem and ask whether it aligns with the stakeholder's perspective. Any disagreements, missing context, or differences in how teams understand the problem will be documented for further investigation.
2. **Explore the stakeholder's area of the current state.** Questions will be tailored to understand the processes, data, definitions, business rules, reporting needs, pain points, constraints, and other considerations relevant to their role.
3. **Understand what success looks like from their perspective.** Each stakeholder will be asked what a successful outcome would look like for them. These responses will be compared across stakeholders to identify shared goals as well as potentially conflicting needs or expectations.
4. **Ask what else should be considered.** Each conversation will include an opportunity for the stakeholder to raise concerns, context, dependencies, risks, or other information that may not have been covered by the prepared questions.

The findings from these conversations will be compared across stakeholders to identify common themes, conflicting definitions or requirements, gaps in the current process, and areas requiring additional discovery.

## Current Problem Statement

Evergreen Community Bank does not currently have a consistent, trusted view of customer complaints across the organization. Customer Service, Compliance, Digital Banking, and branch locations capture and report customer complaints or feedback through different processes, and the resulting information does not always align.

This makes it difficult for leadership to understand overall complaint trends, identify recurring or significant customer issues, and determine when further investigation or action is needed. The current reporting process also requires significant manual effort and is primarily reactive.

A previous attempt to standardize complaint reporting was unsuccessful in part because teams did not share a common definition of what constitutes a complaint. Any future solution will need to address these differences without creating unnecessary manual work and while accounting for regulatory, privacy, and access requirements.

## Stakeholders

| Stakeholder | Role in Initiative | What I Need to Learn | Potential Impact / Considerations | Discovery Priority |
|---|---|---|---|---|
| Customer Service Manager | Complaint process and reporting owner | How complaints are received, categorized, tracked, resolved, and reported; how the monthly report is created; current definitions and business rules; pain points and manual work | Customer Service appears to be a primary source of complaint data. Any future solution could affect its reporting process and workflows. | High |
| Senior Customer Service Representative | Day-to-day process SME | How complaints are actually entered and handled; where judgment is required; common exceptions or workarounds; data quality issues; differences between documented and actual processes | Provides visibility into the operational process and can identify issues or manual steps that may not be apparent from management-level discovery. | High |
| Compliance Manager | Regulatory complaint process and reporting owner | How Compliance defines a complaint; which complaints require regulatory tracking or escalation; reporting requirements; how Compliance data relates to Customer Service data; sensitive-data considerations | Regulatory requirements may affect definitions, data handling, access, retention, and reporting. Differences between Compliance and Customer Service are a major reason for the initiative. | High |
| Digital Banking Product Manager | Owner of digital customer feedback channels | How app reviews and in-app feedback are collected and monitored; what is considered actionable; whether feedback becomes a formal complaint; available data and reporting needs | Digital feedback is currently less structured than other complaint sources and may not map directly to the existing complaint process. | High |
| Retail Banking Operations Manager | Branch representative and business consumer | How branches receive and escalate complaints; consistency of the process across branches; what branch leadership needs from complaint reporting; current visibility gaps | Branches may be both a source and consumer of complaint information. Any solution should avoid adding unnecessary manual work for branch employees. | Medium |
| BI Manager | Technical and reporting partner | Where relevant data currently lives; existing reporting architecture and capabilities; how current reports are produced; potential integration options; technical constraints and dependencies | Will help determine what solution approaches are technically feasible and how a future reporting solution could fit within the existing environment. | Medium |
| Data Governance Lead | Data governance and standardization partner | What happened during the previous complaint-standardization effort; why agreement could not be reached; existing definitions, ownership, stewardship, or governance standards; approach to establishing authoritative definitions and sources | The lack of a shared definition of "complaint" contributed to the previous effort failing. Resolving definitions and ownership may be necessary before a trusted reporting solution can be created. | High |
| Information Security | Security and data-access partner | Requirements for handling customer-level and potentially sensitive complaint information; appropriate access controls; restrictions affecting reporting or data integration | Security requirements will depend on what data the solution ultimately needs and which users require access. More detailed engagement can occur after data and access requirements are better understood. | Later |


## Discovery Sequence

Stakeholder conversations will be conducted sequentially so that information learned in earlier interviews can inform questions and follow-up areas in later conversations. The sequence prioritizes stakeholders closest to the current complaint processes and the areas where inconsistencies have already been identified.

Customer Service and Compliance are early priorities because their reporting differences contributed directly to the initial request. Digital Banking and Data Governance will help explore broader customer feedback, complaint definitions, and the challenges encountered during the previous standardization effort. Retail Banking Operations will provide the branch perspective, while the BI Manager will support the transition from business and process discovery into more detailed data and technical discovery.

Information Security will be engaged later, once the types of customer information involved and the expected access requirements are better understood.
