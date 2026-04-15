# powerbi-project-reporting-narratives
![Power BI](https://img.shields.io/badge/Power%20BI-DAX-yellow?logo=powerbi&logoColor=white)
![DAX](https://img.shields.io/badge/DAX-User%20Defined%20Functions-blue)
![Project Controls](https://img.shields.io/badge/Project%20Controls-PMO%20Focused-success)
![Narrative Reporting](https://img.shields.io/badge/Narrative%20Reporting-Best%20Practice-informational)
![License](https://img.shields.io/badge/License-MIT-green)
![Status](https://img.shields.io/badge/Status-Stable-brightgreen)

A collection of DAX User‑Defined Functions (UDFs) and supporting measures designed to generate structured, professional project reporting narratives in Power BI.
This repository focuses on project controls use cases, helping teams explain what the data means, not just what the numbers are.

### Purpose
Project dashboards often present metrics without context, leaving stakeholders asking:

What reporting period does this relate to?
Which version or forecast is being used?
Is the project actually on track?
What is driving schedule delays or cost overruns?

This repository addresses that gap by providing standardised narrative patterns that:

Clearly state reporting context
Explain schedule and cost performance using thresholds
Identify which project phases drive variance
Scale from single‑project to portfolio views


### What’s Included

DAX User‑Defined Functions for:

- Reporting context narratives
- Schedule and cost status narratives

Supporting measures for:

- Schedule variance
- Cost variance
- Worst‑performing phases
- A single orchestration measure that combines context and status into a final narrative

All narrative logic is separated from calculation logic to keep models auditable and maintainable.


### Example Output

Reporting context: Reporting date 31 Mar 2025, file version Forecast v1.
This project is 18% behind plan, with costs over forecast by 7%, driven by delays in Procurement, with cost pressures primarily in Execution.


### Required Measures (High Level)
To use the patterns in this repository, your model will typically include:

- Reporting Date
- Schedule Version
- Schedule Variance %
- Cost Variance %
- Worst Schedule Phase
- Worst Cost Phase

Optional measures (supported but not required):
- SPI
- CPI


### Intended Use Cases

Project status tables (project on rows)
Portfolio summary views
Management commentary cards
Tooltips and report headers
Automated monthly reporting packs


### Notes on Scope
These patterns focus on narrative generation, not on defining how schedule or cost variance is calculated. They are designed to sit on top of your existing project controls model.

### License
MIT License — free to use, adapt, and extend.

### Acknowledgements
Inspired by real‑world PMO and project controls reporting challenges, where clarity, consistency, and auditability matter as much as accuracy.
