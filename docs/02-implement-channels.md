# Domain 2: Implement Channels (30–35%)

## 2.1 Voice Channel Provisioning & Management
The voice channel integrates Azure Communication Services with Microsoft Dynamics 365 Contact Center.

### Voice Telephony Infrastructure
1. **Phone Number Acquisition**:
   - Direct purchase via Microsoft Azure Communication Services (ACS) (Toll-Free, Geographic/DID).
   - Bring Your Own Carrier (BYOC) via Direct Routing with Certified Session Border Controllers (SBC).
2. **Calling Profiles**:
   - **Inbound Calling Profiles**: Associate phone numbers with operating hours, music on hold, automated greetings, and default routing workstreams.
   - **Outbound Calling Profiles**: Configure outbound CLI (Caller ID), country dialing restrictions, and representative dialing permissions.
3. **Third-Party IVR Integration**:
   - Leverage the **CCaaS SDK API** to route external telephony streams into Dynamics 365 Unified Routing.
   - Configure SIP header data passing to transfer caller context and authentication tokens to representatives.

---

## 2.2 Digital & Chat Channels
- **Chat Widgets**:
  - Embedding JavaScript chat widgets into external websites, portals, and Power Pages.
  - Proactive Chat: Triggering chat prompts based on page dwell time, URL patterns, or cart abandonment.
  - Pre-Chat Surveys: Capturing customer intent, account numbers, and issue categories before routing.
- **Live Chat SDK & Mobile Messaging SDK**:
  - Integrating custom chat interfaces into native iOS/Android applications.
  - Authentication settings (OAuth 2.0 / OpenID Connect) to authenticate logged-in portal users and prevent session spoofing.
- **Social & SMS Channels**:
  - Apple Messages for Business, WhatsApp Business, SMS (via ACS / TeleSign / Twilio), and Custom Messaging APIs.

---

## 2.3 Proactive Outbound Engagement & Workforce Management (WFM)
- **Proactive Outbound Campaigns**:
  - Outbound dialers: *Preview* (agent reviews before dial), *Progressive* (dials when agent becomes available), *Predictive* (AI algorithm predicts agent availability).
  - Workstreams and trigger rules for automated SMS/email customer notifications.
- **Workforce Management (WFM)**:
  - Shift planning, scheduling, capacity forecasting, and integrating third-party WFM platforms (e.g., Verint, NICE).

---

## 2.4 References
- [Voice channel in Dynamics 365 Contact Center](https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/voice-channel-overview)
- [Configure Chat Channel & Live Chat SDK](https://learn.microsoft.com/en-us/dynamics365/contact-center/administer/add-chat-widget)
