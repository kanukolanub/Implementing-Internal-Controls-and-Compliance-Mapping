# Internal-control
Lab: Implementing Internal Controls & Compliance Mapping
Platform: eramba GRC (Community Edition)
📋 Overview
This lab demonstrates the end-to-end lifecycle of an Internal Control within a Governance, Risk, and Compliance (GRC) framework. Using eramba, I simulated the transition from a regulatory requirement (ISO/IEC 27001:2022) to a functional, monitored technical control.

🎯 Goal
The objective was to architect a "Continuous Monitoring" environment that ensures Access Control (Annex A 5.15) remains effective over time, rather than just being a "point-in-time" check.

🛠️ Tech Stack & Frameworks
GRC Tool: eramba Community Edition (v3.x)

Deployment: Docker / Self-hosted

Framework: ISO/IEC 27001:2022

Process Focus: Internal Control Management (ICM), Evidence Collection, Stakeholder Accountability.

🚀 Lab Walkthrough
Phase 1: Compliance Mapping
I began by defining the "Legal/Regulatory" layer.

Imported the ISO 27001:2022 Compliance Package.

Targeted Control A.5.15 (Access Rights).

Outcome: Created a digital link between the theoretical requirement and the organizational asset.

Phase 2: Internal Control Design
I designed a specific control to satisfy the requirement: "Quarterly User Access Review (UAR)".

Control Description: Automated review of all active accounts on the Production Database.

Maturity Level: Defined as "Defined & Managed."

Stakeholders: Assigned an Owner (IT Admin) and a Reviewer (IT Manager) to establish a segregation of duties.

Phase 3: Maintenance & Evidence Automation
The core of the lab involved setting up the "Audit Heartbeat."

Frequency: Configured for 90-day intervals.

Evidence Collection: Setup a requirement for a signed approval PDF to be uploaded for each cycle.

Workflow: Configured eramba to trigger email notifications to owners 5 days before the deadline.

Phase 4: Gap Analysis & Reporting
Simulation: I manually triggered a "Missing Evidence" status to simulate a control failure.

Reporting: Generated a Compliance Status Report to visualize how one failed internal control impacts the overall ISO 27001 compliance percentage.

🧠 Skills Demonstrated
GRC Tooling: Hands-on configuration of eramba workflows, dashboarding, and report generation.

Audit Readiness: Understanding the importance of an "Audit Trail" and the lifecycle of evidence.

Risk Mitigation: Identifying how automated maintenance prevents "Control Decay."

Regulatory Knowledge: Mapping technical IT operations to ISO 27001:2022 standards.
