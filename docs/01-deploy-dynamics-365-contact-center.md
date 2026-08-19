# Domain 1: Deploy Dynamics 365 Contact Center (15–20%)

## 1.1 Overview & Architecture
Deploying Dynamics 365 Contact Center involves provisioning, configuring tenant infrastructure, managing security identities, and orchestrating Application Lifecycle Management (ALM).

### Deployment Topologies
1. **Standalone Contact Center (CCaaS)**:
   - Complete native cloud solution providing voice, digital messaging, unified routing, and AI agents.
   - Built directly on Azure Communication Services (ACS) and Microsoft Dataverse.
2. **Embedded Dynamics 365 Contact Center Mode**:
   - Embeds Dynamics 365 Contact Center representative workspace, omni-channel routing, and Copilot into existing CRM platforms (e.g., Salesforce, ServiceNow).
3. **Copilot for Third-Party CCaaS**:
   - Augments existing telephony platforms (e.g., Cisco, Genesys Cloud, NICE CXone) with Microsoft Copilot generative AI, real-time sentiment, and live call summaries without migrating carrier infrastructure.

---

## 1.2 User Administration, Security & Personas
Dynamics 365 Contact Center utilizes security roles and capacity profiles to control access and work allocation.

### Core Security Roles
| Security Role | Purpose & Permissions |
| :--- | :--- |
| **Contact Center Administrator** | Full administrative rights over workstreams, channels, bots, capacity profiles, and tenant settings. |
| **Contact Center Supervisor** | Monitors ongoing conversations, assigns work items, accesses real-time/historical Power BI dashboards, whispers/joins sessions. |
| **Contact Center Representative** | Accepts assigned customer sessions, executes scripts/macros, interacts with Copilot, resolves work items. |
| **Productivity Tools User** | Grants read/execute access to agent scripts, macros, and smart assist components. |

### Capacity Profiles
- **Units vs Count**: Define work volume consumption per session (e.g., Voice = 100 units, Chat = 30 units from a total representative capacity of 100).
- **Reset Frequency**: Immediate upon session close vs end of workday.
- **Blocking / Non-Blocking**: Configure whether reaching capacity blocks all channels or allows specific priority overrides.

---

## 1.3 Application Lifecycle Management (ALM) & Extensibility
- **Solution Management**: Package workstreams, queues, automated messages, templates, and macros into managed solutions for Dev $\rightarrow$ Test $\rightarrow$ Prod deployment.
- **Health Agent**: Proactively monitors omnichannel configuration health, detects missing routing bindings, and reports configuration drift.
- **Journey Simulation**: Enables administrators to simulate end-to-end customer interactions across voice and digital channels before moving to production.

---

## 1.4 References
- [Official Microsoft Dynamics 365 Contact Center Documentation](https://learn.microsoft.com/en-us/dynamics365/contact-center/)
- [Manage users and capacity profiles in Dynamics 365](https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/capacity-profiles)
