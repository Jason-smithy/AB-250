# Domain 5: Configure Representative Experience (15–20%)

## 5.1 Workspace Customization & App Profile Manager
Creating optimized multi-session experiences for contact center agents.

### Core Configuration Elements
- **Experience Profiles**: Assign custom workspace layouts, productivity panes, and channel providers to specific user personas.
- **Session Templates**: Define anchor tabs (e.g., Customer Summary form) and additional application tabs opened upon session acceptance.
- **Application Tab Templates**: Configure custom entity forms, Power BI dashboards, web resources, or external URLs loaded inside agent sessions.
- **Agent Inbox**: Unified multi-session inbox supporting custom filtering, priority sorting, and conversation views.
- **Notification Templates**: Sound alerts, banner notifications, auto-accept behaviors, and timeout durations.

---

## 5.2 Productivity Tools & Automation
- **Agent Scripts**:
  - Step-by-step guidance scripts providing conversational prompts.
  - **Slugs**: Dynamic parameters inserted at runtime (e.g., `{customer_name}`, `{case_title}`).
- **Macros**:
  - Deterministic action sequences (e.g., open sub-grid, auto-populate fields, execute cloud flow, resolve case).
  - Configured using the Macro Designer with built-in connector actions.
- **Microsoft Teams Swarming**:
  - Native integration allowing representatives to swarm complex cases with subject matter experts (SMEs) across Teams channels while keeping case context linked.

---

## 5.3 Knowledge Management & JavaScript APIs
- **Internal & External Knowledge Search**: Grounding agent knowledge in Dataverse knowledge articles and external federated search endpoints.
- **Omnichannel JavaScript API (`Microsoft.Omnichannel.*`)**: Programmatically controlling sessions, retrieving conversation metadata, setting custom presences, and broadcasting events.

---

## 5.4 References
- [App Profile Manager Documentation](https://learn.microsoft.com/en-us/dynamics365/app-profile-manager/)
- [Configure Agent Scripts & Macros](https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/agent-scripts)
