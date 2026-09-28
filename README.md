# Customer Complaint Intelligence & Reporting Solution

## Overview

This project was designed as an end-to-end data solutions case study for a fictional regional bank, **Evergreen Community Bank**.

The initial request was intentionally simple:

> “We need a Power BI dashboard for customer complaints. Leadership doesn't have a reliable way to understand what customers are complaining about or whether things are getting better. Right now, different departments send us their own reports, and the numbers never seem to match. We'd like one dashboard that leadership can use every month.”

Rather than immediately building the requested dashboard, I approached the problem as a data solutions analyst would: first understanding **what the business was actually trying to solve, how different teams defined and captured complaints, what data was available, and what would be required to create a trustworthy enterprise reporting solution.**

## Project Scope

The project was intended to follow the full lifecycle of a data solution: **business and stakeholder discovery → findings validation → requirements definition → data discovery and profiling → solution evaluation and design → build and reporting → validation and handoff.**

The goal was to practice the complete process behind a data solution rather than starting with a dataset and immediately building a dashboard.

## ⚠️ Project Stopped During Data Discovery

This project stops at the beginning of the data discovery phase, before data profiling or solution implementation.

The fictional business scenario and stakeholder interviews for this portfolio project were developed using ChatGPT. I created the discovery approach and interview questions, used ChatGPT to simulate stakeholder responses, and then performed the analysis used to develop the discovery findings and requirements.

When I reached the data discovery phase, I used ChatGPT to generate synthetic datasets intended to represent the source systems described during stakeholder discovery. I reviewed the generated data against the previously established stakeholder interviews and requirements and identified multiple inconsistencies.

I went through several rounds of review and correction to reconcile the synthetic data with the discovery work. However, after repeated inconsistencies, I no longer had sufficient confidence that the generated datasets reliably represented the current state established during discovery.

**I made the decision not to continue into data profiling, solution design, or dashboard development using data I did not trust.**

In a real data project, moving forward with questionable source data simply to complete a deliverable would create a larger problem. Data discovery exists in part to determine whether available data is appropriate for the intended solution and to surface gaps before those gaps become embedded in reporting.

For that reason, I am preserving this project as a **discovery and requirements case study rather than manufacturing a finished dashboard from unreliable synthetic data.**

The completed work demonstrates:

- Stakeholder discovery and interview planning
- Translating an ambiguous dashboard request into a defined business problem
- Current-state analysis
- Identification of differing definitions and business processes
- Development and validation of discovery findings
- Business and solution requirements development
- Requirements traceability
- Data-source planning
- Validation of proposed source data against established requirements
- Recognition of data reliability issues
- Knowing when not to proceed with implementation

Stopping the project at this point is itself part of the analysis: **a reporting solution is only as trustworthy as the assumptions and data supporting it.**

## Repository Structure

```text
customer-complaint-data-solution/
│
├── 01-discovery/
│   ├── interviews/
│   ├── 01-initial-discovery.md
│   ├── 02-stakeholder-discovery-plan.md
│   ├── 03-discovery-findings.md
│   └── 04-discovery-findings-review.md
│
├── 02-requirements/
│   ├── 01-business-requirements.md
│   ├── 02-solution-requirements.md
│   └── 03-requirements-review.md
│
├── data/
│   ├── PACKAGE_QA.csv
│   ├── SOURCE_DELIVERY_NOTES.md
│   ├── authenticated_digital_feedback.csv
│   ├── branch_reference.csv
│   ├── compliance_cases.csv
│   ├── customer_reference.csv
│   ├── customer_service_complaints.csv
│   ├── date_reference.csv
│   └── product_reference.csv
│
└── README.md
```

## Skills Demonstrated

**Discovery & Analysis**
- Stakeholder discovery
- Requirements elicitation
- Current-state analysis
- Business process analysis
- Data-source identification
- Data-quality hypothesis development
- Requirements traceability
- Data governance considerations

**Delivery & Collaboration**
- Stakeholder facilitation planning
- Cross-functional discovery
- Requirements validation
- Translating business needs into solution requirements
- Documentation
- Governance and ownership planning

**Data Readiness**
- Source-data validation
- Assessing data fitness for analysis
- Identifying inconsistencies between requirements and proposed source data
- Evaluating whether data is sufficiently trustworthy to proceed

## About the Scenario

Evergreen Community Bank and all stakeholders in this repository are fictional.

Stakeholder responses and synthetic source data were generated with ChatGPT for portfolio purposes. The discovery approach, stakeholder questions, analysis, findings, requirements, review decisions, and decision to discontinue the project were developed as part of my portfolio work.

No real customer or banking data is included in this repository.
