# The Telephone Society (TTS)

**The Telephone Society** is a privacy-first, time-based venue reward system designed to drive customer engagement and capture localized venue analytics without sacrificing user anonymity.

---

## 🎯 Core Principles

* **Zero PII (Personally Identifiable Information):** No user personal data, real names, phone numbers, or email addresses are ever collected or stored.
* **Ephemeral Location Verification:** Session validity relies on momentary physical presence without continuous or intrusive background tracking.
* **Strict Tenant Data Isolation:** Venues access only high-level, aggregated analytics for their own location. Cross-venue tracking and individual visit path analyses are strictly blocked.
* **Secure Secrets Management:** All API keys, environment variables, and backend credentials must remain strictly outside source control.

---

## 🏗️ Architecture & Tech Stack

* **Front End:** Custom landing experience deployed via Carrd with embedded JavaScript modules.
* **Back End:** Lightweight Python API for session management and time-reward verification.
* **Deployment & Hosting:** Cloud-managed hosting (Render / Railway) with CI/CD integration directly from GitHub.
* **Version Control:** Managed via GitHub with strict secret-scanning and privacy guardrails.

---

## 📊 Business Intelligence & Analytics Boundary

| Metric Category | Venue Partner Access | Privacy Enforcement |
| :--- | :--- | :--- |
| **Traffic Trends** | Aggregated hourly/daily volume | $k$-Anonymity thresholds applied |
| **Dwell Time** | Average session duration | No individual time-stamps exposed |
| **Reward Claims** | Total rewards generated/redeemed | Ephemeral, single-use validation tokens |
| **User Identifiers** | **BLOCKED** | Zero PII architecture |
| **Individual Logs** | **BLOCKED** | Non-exportable raw event data |
| **Cross-Venue Paths**| **BLOCKED** | Multi-venue session linking prohibited |

---

## 📁 Repository Structure

```text
├── README.md           # Project overview and architectural principles
├── DATA_PRIVACY.md     # Detailed data isolation and privacy guidelines
└── backend/            # Python API services and session tracking logic
