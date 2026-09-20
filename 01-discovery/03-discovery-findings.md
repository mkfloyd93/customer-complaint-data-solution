# Discovery Findings

## Purpose

This document summarizes the key findings from stakeholder discovery for the Customer Complaint Intelligence & Reporting Solution.

Discovery focused on understanding the current complaint and customer feedback landscape across Evergreen Community Bank, including how different teams define, capture, manage, escalate, and report customer concerns.

The findings below will be used to refine the business problem and establish requirements for the future solution.

---

## Refined Problem Statement

Evergreen Community Bank does not currently have a shared enterprise understanding of customer complaints and related customer feedback.

Customer Service, Compliance, Digital Banking, and branch locations capture and manage different but related types of customer concerns based on their individual business responsibilities. These differences are expected and do not require each team's complaint counts, definitions, or operational processes to match.

However, the relationships between these records, definitions, categories, and underlying customer issues are not consistently defined or captured. As a result, leadership cannot reliably interpret complaint activity across the organization, understand how departmental metrics relate to one another, or identify broader patterns and emerging customer issues.

Reporting is also fragmented and relies on manual processes. Potential data-quality issues, inconsistent categorization, unclear handoffs, and disconnected systems may further limit enterprise visibility and will require additional investigation.

---

## Key Discovery Findings

### 1. Different teams capture different but related customer concerns

There is not currently a single enterprise definition or conceptual framework for customer complaints and related customer feedback.

Each business area captures information based on its responsibilities:

- **Customer Service** manages operational complaint cases resulting from customer interactions and referrals.
- **Compliance** manages complaints and cases that may involve regulatory, legal, fair-lending, consumer-protection, or reputational risk.
- **Digital Banking** receives broader customer feedback through sources such as app-store reviews and authenticated digital feedback.
- **Retail Banking** receives complaints directly from customers in branches. Some are resolved locally, while others are referred or escalated to another team.

These differences do not necessarily represent conflicting definitions or incorrect processes. The teams have different business needs and therefore capture different aspects of the customer experience.

The enterprise currently lacks a shared framework for understanding how these different concepts relate.

### 2. Different complaint counts are expected, but their meaning and relationships are unclear

The original request was partly driven by concern that complaint numbers reported by different departments did not match.

Discovery indicated that matching departmental totals should not be the goal.

Customer Service, Compliance, Digital Banking, and Retail Banking are not necessarily measuring the same population or business concept. Different counts may therefore be valid and expected.

The larger issue is that leadership does not have a consistent way to understand what each departmental metric represents or how those metrics should be interpreted together.

For example, a Compliance case count may represent a specific subset of customer concerns requiring regulatory or risk oversight, while Customer Service reporting represents a broader set of operational complaint cases. Digital Banking may provide an additional view of customer feedback that does not follow the same case-management process.

The future solution should provide enough definition and context for users to understand these differences and interpret departmental information as part of a broader enterprise view.

Discovery also identified potential value in understanding when records across systems relate to the same customer concern or underlying issue. The feasibility and business value of establishing these relationships, particularly for historical records, require further investigation and should not yet be considered necessary for the success of the initial solution.

### 3. A shared enterprise conceptual model is needed

Discovery identified several related concepts that may need to be distinguished at the enterprise level.

Examples raised during stakeholder discussions include:

- Customer feedback or signals
- Expressions of dissatisfaction
- Customer Service complaint cases
- Compliance complaint cases
- Underlying customer issues or incidents

The exact enterprise definitions and relationships between these concepts have not yet been finalized.

A shared conceptual model will be needed so that different operational processes can retain their appropriate definitions while still contributing to an enterprise understanding of customer concerns.

This model should clarify relationships such as whether:

- One customer concern can generate multiple operational records
- One complaint can result in multiple cases or escalations
- Multiple complaints can relate to the same underlying issue
- Customer feedback can represent a complaint without becoming an individually managed case
- Different departmental categories can be mapped to broader enterprise concepts

### 4. Complaint information is fragmented across systems and channels

Complaint and feedback information enters the organization through multiple channels and is stored in different systems.

Current sources include:

- Customer Service complaint records
- Compliance cases
- Authenticated digital feedback
- Public app-store reviews
- Branch interactions and referrals
- Existing enterprise customer, product, branch, and organizational reference data

Not all customer concerns currently result in a structured complaint record.

For example, a complaint resolved immediately by a Customer Service representative or branch employee may not always be formally recorded. Public digital feedback also does not currently follow the same structured intake process as Customer Service or Compliance cases.

This fragmentation limits the bank's ability to understand the customer experience across organizational boundaries.

### 5. Cross-team handoffs and relationships are not consistently captured

Customer concerns can move between departments, particularly from Customer Service or Retail Banking to Compliance.

However, the relationship between records created by different teams is not consistently preserved.

For example, a Customer Service complaint that results in a Compliance case does not currently have a consistently populated shared identifier connecting the two records.

This creates difficulty when attempting to determine whether records across systems represent:

- The same customer concern
- Separate concerns from the same customer
- Multiple interactions related to one issue
- Separate but related operational cases

The ability to understand these relationships will be important for enterprise reporting.

### 6. Categorization and operational decision-making involve significant judgment

Several stakeholders described variation in how employees identify, categorize, document, and escalate complaints.

Examples include:

- Determining whether an interaction should be formally recorded
- Selecting a primary category when multiple issues are involved
- Deciding whether a repeat contact should update an existing record or create a new one
- Determining when an issue should be escalated
- Using broad categories such as "Other"
- Determining how much information should accompany a referral

Training and guidance exist in some areas, but stakeholders indicated that employees still rely on judgment.

Operational categories also differ between teams because they support different business purposes.

Enterprise reporting may require mappings between departmental categories rather than forcing all teams to use identical operational categories.

### 7. Current reporting is fragmented and includes significant manual effort

Current complaint reporting is produced separately by different business areas.

Customer Service's monthly reporting requires manual extraction, cleanup, calculation, and commentary. Compliance maintains separate reporting based on its own requirements. Digital Banking reviews customer feedback through separate product and platform processes.

Stakeholders expressed interest in reducing manual reporting and reconciliation effort.

A future solution should automate reporting where practical while avoiding the creation of additional manual processes solely to support analytics.

### 8. Stakeholders want actionable visibility, not simply complaint counts

Across stakeholder groups, there was interest in using complaint information to identify and respond to customer issues earlier.

Desired visibility includes areas such as:

- Complaint and feedback trends
- Common topics and categories
- Recurring customer issues
- Emerging issues
- Severity or risk
- Source and channel
- Products and services involved
- Branch-level patterns
- Resolution and aging
- Relationships between complaints and known incidents or broader problems

Stakeholders also emphasized the importance of context.

For example, raw complaint counts may not provide a meaningful comparison between branches with different customer volumes or transaction complexity.

The future solution should support interpretation and action rather than simply aggregating records.

### 9. The solution should minimize operational burden

A consistent theme across stakeholders was concern about introducing additional work for operational teams.

Stakeholders generally did not want:

- Another system requiring duplicate entry
- Significant additional documentation
- Existing operational processes replaced solely for reporting purposes
- Reporting requirements that interfere with serving customers

Where possible, the future solution should reuse information already captured through operational processes and automate integration and reporting.

Process or system changes may still be necessary where current practices prevent important information from being captured, but the business value of those changes should justify the additional effort.

### 10. Governance, ownership, privacy, and access will be important

A sustainable enterprise solution will require more than technical integration.

Business definitions, category mappings, and other reporting rules will need documented ownership and a process for managing changes.

The appropriate authoritative source may also vary by concept. For example, Customer Service may remain authoritative for the status of a Customer Service case, while Compliance remains authoritative for Compliance case status and disposition.

The solution must also account for differences in data sensitivity.

Compliance records may contain sensitive customer, employee, legal, or investigative information that should not be broadly available. Leadership may only require aggregate information, while operational users may require more detailed access.

Security and access requirements will need to be incorporated into the eventual solution design.

---

## Data Quality Hypotheses Requiring Validation

Stakeholder discovery identified several potential data-quality issues. These should currently be treated as hypotheses rather than confirmed findings.

Data discovery and profiling should determine the frequency and impact of:

- Missing complaint records when issues are resolved without formal documentation
- Duplicate or near-duplicate complaint records
- Repeat contacts recorded inconsistently
- Inconsistent category usage
- Overuse of broad categories such as "Other"
- Missing or incomplete branch referral information
- Inconsistent customer, product, or branch information
- Variation in free-text documentation quality
- Missing relationships between Customer Service and Compliance records
- Limited ability to associate customer feedback with broader incidents or issues

Stakeholder perceptions will be compared with the available data before conclusions are made about the severity of these issues.

---

## Emerging Business Needs

Based on discovery, the future capability will likely need to:

- Establish shared enterprise definitions for customer complaints, feedback, cases, and related concepts
- Define how departmental complaint and feedback concepts relate to one another
- Preserve legitimate differences between departmental processes and definitions
- Establish mappings between departmental categories and broader enterprise concepts where appropriate
- Represent relationships between related records without incorrectly combining or double-counting them
- Provide leadership with an interpretable enterprise view of customer concerns
- Support more detailed operational analysis for appropriate users
- Improve visibility into trends, recurring issues, emerging problems, severity, and resolution
- Reduce manual reporting and reconciliation
- Reuse existing operational data and minimize duplicate data entry
- Establish ownership for definitions, mappings, and reporting rules
- Maintain appropriate privacy, security, and role-based access

These needs will be refined and translated into formal requirements in the next phase.

---

## Open Questions

Discovery also identified questions that require further analysis:

- What should constitute a complaint at the enterprise level?
- Should customer feedback, complaints, operational cases, and underlying issues be modeled as separate concepts?
- What relationships between those concepts need to be represented?
- Which departmental categories can or should be mapped to broader enterprise categories?
- Which systems and fields should be authoritative for different pieces of information?
- How reliably can existing records be connected across systems?
- What approach should be used when relationships can only be inferred?
- What information is required for leadership reporting versus operational analysis?
- What data can be included at each level of access?
- Which current process or system changes are necessary for a reliable initial solution, and which could be addressed as longer-term improvements?

---

## Next Steps

The next phase will translate the discovery findings into business, functional, reporting, data, governance, security, and nonfunctional requirements.

Once the initial requirements have been established, data discovery and profiling will be used to validate stakeholder assumptions, assess the current state of the available data, identify gaps between the requirements and current capabilities, and inform the evaluation of potential solution approaches.