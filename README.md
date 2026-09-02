# The Telephone Society (TTS)

**The Telephone Society** is a privacy-first, time-based venue reward system designed to drive customer engagement and capture localized venue analytics without sacrificing user anonymity.

---

## 🎯 Core Principles

* **Zero PII (Personally Identifiable Information):** No user personal data, real names, phone numbers, or email addresses are ever collected or stored.
* **Ephemeral Location Verification:** Session validity relies on momentary physical presence without continuous or intrusive background tracking.
* **Strict Tenant Data Isolation:** Venues access only high-level, aggregated analytics for their own location. Cross-venue tracking and individual visit path analyses are strictly blocked.
* **Low-Friction Onboarding:** Physical access points (front windows/entryways) allow self-serve check-ins without disrupting venue operations or staff workflows.
* **Secure Secrets Management:** All API keys, environment variables, and backend credentials must remain strictly outside source control.

---

## ⏱️ Dynamic Dwell Thresholds & Enforced System Floors

To ensure analytical integrity and prevent gaming, session verification enforces tiered minimum time floors based on business category. Venue partners can customize their threshold above the system floor to fit their specific operational dynamics.

| Venue Category | System Minimum Floor | Recommended Partner Default | Typical Max Threshold |
| :--- | :--- | :--- | :--- |
| **Coffee / Grab & Go** | 5 Minutes | 10–15 Minutes | 30 Minutes |
| **Casual Dining / Bars** | 15 Minutes | 30–45 Minutes | 90 Minutes |
| **Fine Dining / Clubs** | 30 Minutes | 60–90 Minutes | 180 Minutes |
| **Event Spaces / Arenas**| 45 Minutes | 90–120 Minutes | 240+ Minutes |

---

## 🏗️ Architecture & Tech Stack

* **Front End:** Custom landing experience deployed via Carrd with embedded JavaScript modules.
* **Back End:** Lightweight Python API (`verification_engine.py`) for session management, dynamic threshold validation, and time-reward verification.
* **Deployment & Hosting:** Cloud-managed hosting (Render / Railway) with CI/CD integration directly from GitHub.
* **Version Control:** Managed via GitHub with strict secret-scanning and privacy guardrails.

---

## 📊 Business Intelligence & Analytics Boundary

| Metric Category | Venue Partner Access | Privacy Enforcement |
| :--- | :--- | :--- |
| **Hourly Traffic Trends** | Aggregated hourly/daily volume | $k$-Anonymity thresholds applied (suppressed if < 5 sessions) |
| **Dwell Time** | Average session duration per hour | No individual timestamps or exact visit logs exposed |
| **Reward Claims** | Total rewards generated/redeemed | Ephemeral, single-use validation tokens |
| **User Identifiers** | **BLOCKED** | Zero PII architecture |
| **Individual Logs** | **BLOCKED** | Non-exportable raw event data |
| **Cross-Venue Paths**| **BLOCKED** | Multi-venue session linking prohibited |

---

## 📁 Repository Structure

```text
├── README.md               # Project overview, architectural principles & dwell floors
├── DATA_PRIVACY.md         # Detailed data isolation and privacy guidelines
├── verification_engine.py  # Core session verification and telemetry validation logic
└── backend/                # Python API services and database integrations
