# Domain 4: Configure Work Distribution (10–15%)

## 4.1 Unified Routing Engine Architecture
Unified Routing is a two-stage routing service that optimizes work allocation across all voice and digital channels.

### Stage 1: Workstream & Work Classification
1. **Workstream Configuration**:
   - Channel type binding (Voice, Chat, Messaging, Record).
   - Context variables definition (e.g., `CustomerTier`, `AccountBalance`, `Urgency`).
2. **Work Classification Rules**:
   - Logical condition rules mapping payload data to priority and severity.
   - **Machine Learning (ML) Skill Finder**: Natural language processing models that extract customer sentiment and intent to attach required representative skills.
   - **Intent-Based Routing**: Maps customer messages to categorized business intents.

---

## 4.2 Stage 2: Prioritization, Queues & Assignment Methods

### Assignment Methods Comparison
| Assignment Method | Mechanism | Ideal Use Case |
| :--- | :--- | :--- |
| **Highest Capacity** | Assigns to the representative with the most remaining available capacity units. | High-volume transactional chat and email queues. |
| **Round Robin** | Distributes items sequentially among qualified available agents. | Equal lead distribution or general support tiers. |
| **Skills-Based Routing (Exact Match)** | Requires the representative to possess 100% of assigned skills and proficiency levels. | Specialized technical support, medical/legal compliance. |
| **Skills-Based Routing (Closest Match)** | Relaxes non-mandatory skill requirements if no exact match is available. | Minimizing customer wait times during peak volume. |
| **Preferred Representative Routing** | Directs customer to their assigned account manager or previous case owner. | High-touch VIP account management. |

---

## 4.3 Overflow, Fallback & Diagnostics
- **Overflow Triggers**: Exceeding max queue wait time, max work item count, or operating hours expiration.
- **Overflow Actions**: Transfer to fallback queue, offer customer callback, redirect to voicemail, or trigger automated bot triage.
- **Conversation Diagnostics**: Built-in visual diagnostic tool that details every step of the routing rule execution for troubleshooting.

---

## 4.4 References
- [Unified Routing Overview in Dynamics 365](https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/overview-unified-routing)
- [Configure skills-based routing](https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/set-up-skills-based-routing)
