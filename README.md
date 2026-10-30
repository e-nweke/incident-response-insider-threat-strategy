# Incident Response – Insider Threat Detection & Forensic Data Collection Strategy

A consultancy-style report produced for the Intrusion Detection and Response module of my MSc Cybersecurity at Coventry University. The brief: advise a defense/security-sector client on detecting insider-threat reconnaissance, building a forensically sound data collection strategy, choosing between SIEM platforms, and running through a hypothetical insider-led data exfiltration incident.

> This is an analytical/consultancy report, not a hands-on build — the deliverable was a written strategy and recommendation, not a deployed system. Figures below are reproduced from that report.

## Scenario

The client is assumed to operate in defense and security-sector product development, serving government departments, multinational firms and foreign agencies — a high-value target for insider threats and advanced persistent threats (APTs). The assumed network spans multiple client subnets, Wi-Fi access points, server farms and a core backbone behind a single internet gateway.

![Assumed client network architecture](./figures/fig1_network_architecture.jpg)

## Detecting insider-threat reconnaissance

Covers the behavioural and technical indicators that distinguish an insider probing for exfiltration opportunities from normal activity — unusual access-pattern changes, off-hours authentication, abnormal data-staging behaviour, and the log sources needed to catch it early (authentication logs, DLP alerts, endpoint telemetry, file-access auditing).

## Data collection strategy for forensic analysis

A structured approach to what to collect, from where, and why — balancing investigative value against operational disruption and the need to preserve forensic integrity (chain of custody, order of volatility, minimizing evidence contamination).

![Data collection strategy for forensic analysis](./figures/fig5_data_collection.jpg)

## SIEM platform comparison: Splunk vs Elastic Stack

A comparison of Splunk Enterprise Security + SOAR against Elastic Security for insider-threat detection and automated response, weighing deployment cost, scalability, automation capability and ease of use.

![Splunk vs Elastic comparison](./figures/fig4_splunk_vs_elastic.jpg)

| Feature | Splunk | Elastic Stack |
|---|---|---|
| Deployment Type | Commercial, enterprise-managed solution | Open-source, highly customizable |
| Cost | Higher (subscription-based licensing) | Lower (open-source with optional support) |
| Automation & SOAR | Integrated automation and orchestration features | Customizable via plugins and scripts |
| Scalability | Excellent for enterprise-scale environments | Highly scalable with modular components |
| Ease of Use | User-friendly dashboards, prebuilt content | Requires expertise for full customization |

## Incident response exercise: insider-led data exfiltration

A walk-through of a hypothetical insider-led exfiltration incident, identifying the forensic data sources needed, gaps in existing visibility, and forensically sound collection practices (write-blocking, hashing, documented chain of custody) — plus how the response would adapt if the activity showed signs of a broader APT campaign rather than a lone insider.

![Incident response process flowchart](./figures/appendixA_ir_flowchart.jpg)

## Cost-effectiveness analysis

A justification of the recommended investment across equipment, human resources and operational-impact categories, weighing upfront cost against long-term resilience and breach-risk reduction.

![Cost justification](./figures/fig7_cost_justification.jpg)

| Category | Investment | Benefit |
|---|---|---|
| Hardware | Sensors, packet capture devices, storage appliances | Improved visibility and forensic capability |
| Software | SIEM licenses, endpoint monitoring agents | Enhanced threat detection and log correlation |
| Human Resources | Analyst training, certifications | Skilled workforce for efficient incident response |
| Operational Impact | Temporary disruptions during implementation | Long-term resilience and reduced breach risk |

## Topics covered
Insider threat detection, forensic readiness, chain of custody, SIEM/SOAR platform evaluation (Splunk Enterprise Security, Elastic Security), incident response lifecycle (detection → analysis & triage → containment → eradication → recovery → post-incident review), APT considerations, cost-benefit analysis for security investment.

## Evidence
Full-size figures and supporting tables are in [`figures/`](./figures).

## Disclaimer
This report was produced as academic coursework based on an assumed client scenario. It does not describe a real organisation's network or incident.
