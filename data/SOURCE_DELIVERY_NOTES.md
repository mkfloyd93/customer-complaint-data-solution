# Evergreen Community Bank — Current-State Data Discovery Package

> **Simulation Note:** These are fictional source extracts created for a portfolio project. The package is constrained to data the stakeholder interviews support as currently available to the analyst/data team. It is intentionally not a pre-integrated reporting model.

## Files supplied

### `customer_service_complaints.csv`
**Source:** Customer Service application  
**Current delivery path:** Database/system extract available to the data team.

Fields reflect the Customer Service interviews: complaint identifier, received/resolved dates, customer when identifiable, one primary category, notes, contact channel, product when applicable, branch when relevant, status, and referral/escalation destination where represented.

There is no formal severity field. Source category values and source notes have not been cleaned into an enterprise standard.

### `compliance_cases.csv`
**Source:** Separate Compliance tracking/vendor application  
**Current delivery path:** Scheduled/exported data used for Compliance reporting; sensitive fields are restricted.

Fields reflect the Compliance interview: case identifier, complaint type, regulatory category, customer information when available, received date, source, assigned owner, assigned/required-action/closed dates, status, investigation notes, disposition, and whether further escalation was required.

There is no structured shared identifier connecting Compliance cases to Customer Service complaints. A Customer Service complaint number may appear manually in Compliance notes, inconsistently.

This discovery extract excludes underlying restricted case details that are not necessary for the current analysis.

### `authenticated_digital_feedback.csv`
**Source:** Authenticated Digital Banking platform  
**Current delivery path:** Stored internally and extractable.

Fields reflect the Digital Banking interview: customer identifier, date/time, feedback text, digital channel, page/feature, session or technical information, device information, plus the Digital team's own topic/classification. These records are customer feedback signals and should not automatically be interpreted as formal complaint cases.

### Enterprise reference extracts
- `customer_reference.csv`
- `product_reference.csv`
- `branch_reference.csv`
- `date_reference.csv`

The BI interview establishes that standard enterprise dimensions exist for customers, products, branches, and dates. The interviews do not define their exact production schemas, so these reference extracts use plausible simulated reference attributes while avoiding unsupported activity, transaction-volume, behavioral, balance, or sensitive demographic data. The added descriptive attributes are simulation assumptions, not facts learned during stakeholder discovery.

## Relevant sources NOT supplied as current structured extracts

### App-store reviews
Digital Banking monitors public app-store reviews, but the BI interview states that app-store review data is not currently part of the internal data environment and is handled through app platforms/manual reporting. No `app_store_reviews.csv` is supplied. A sustainable ingestion method remains a current-state gap to investigate.

### Branch-local complaint records
There is no separate reliable branch complaint dataset. If a branch refers an issue to Customer Service and a complaint is created, it can appear in the Customer Service extract. A locally resolved concern may have no structured complaint record.

### Branch activity / digital usage context
The requirements review says contextual information should be investigated before using raw branch or Digital feedback volumes for comparison. The interviews do not establish a specific currently available activity/usage extract for this project, so no such dataset has been invented.

### Technology incidents / defects
Technology teams track incidents and defects elsewhere, but relationships to complaint/feedback records are not standardized and their data has not yet been established as part of the current discovery package.

## Discovery boundaries

- Different departmental counts and categories are not automatically data-quality problems.
- Preserve source meaning and source classifications during profiling.
- Historical cross-system record matching is an investigation item, not an initial success requirement.
- Sensitive information should not be included merely because it exists.
- Data-quality concerns raised by stakeholders are hypotheses to validate against the extracts.
- Missing operational records (for example, complaints resolved but never recorded) cannot be discovered as rows in an extract; that remains a known process limitation.
- The eventual reporting capability must support at least a monthly leadership cadence, but source-specific refresh design is not assumed here.


## Reference schema note

The enterprise reference extracts use a small set of plausible simulated attributes relevant to this project rather than attempting to reproduce a full banking data warehouse dimension. Customer names are synthetic. Reference attributes beyond the existence of standard customer, product, branch, and date dimensions are simulation assumptions.
