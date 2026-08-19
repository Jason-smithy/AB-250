# Domain 6: Manage Contact Center Analytics (10–15%)

## 6.1 Supervisor Experience & Live Monitoring
- **Ongoing Conversations Dashboard**: Live visibility into active conversations across all queues, channels, and agent statuses.
- **Supervisor Actions**:
  - *Monitor*: Silently read/listen to live interactions without notifying customer or representative.
  - *Whisper*: Send internal guidance messages visible only to the representative.
  - *Join*: Enter the conversation as an active participant.
  - *Transfer*: Force-reassign the conversation to another representative or queue.
- **Quality Evaluation Agent**: Automated AI-driven evaluation scoring conversation compliance, tone, sentiment, and resolution effectiveness.

---

## 6.2 Reporting & Power BI Analytics
Dynamics 365 Contact Center provides out-of-the-box embedded Power BI reports:

| Report Category | Key Performance Indicators (KPIs) |
| :--- | :--- |
| **Real-Time Analytics** | Active Conversations, Available Capacity, Average Wait Time (AWT), Abandonment Rate, Service Level Agreement (SLA) adherence. |
| **Historical Analytics** | Average Handle Time (AHT), Customer Satisfaction (CSAT), First Contact Resolution (FCR), Conversation Volume Trends, Sentiment Trends. |
| **Bot Analytics** | Bot Deflection Rate, Escalation Rate to Human Agents, Unhandled Intent Rate, User Engagement Drop-off. |
| **Custom KPI Authoring** | Editing reports directly via the embedded Power BI web editor or building custom data models in **Power BI Desktop**. |

---

## 6.3 Azure Application Insights & Telemetry
- **Conversation Diagnostics in Application Insights**: Exporting real-time event logs, SDK exceptions, WebRTC latency, and routing decisions.
- **Custom KQL Queries**: Querying telemetry using Azure Monitor / Kusto Query Language (KQL) to monitor service availability and API throughput.

---

## 6.4 References
- [Contact center analytics and insights](https://learn.microsoft.com/en-us/dynamics365/contact-center/analytics-insights/overview)
- [Supervisor dashboards and monitoring](https://learn.microsoft.com/en-us/dynamics365/contact-center/analytics-insights/ongoing-conversations)
