# KPPMCH Pregnancy Care

| PROJECT ARCHITECTURE & MATERNAL CARE |
| :--- |
| **Maternal Healthcare Automation & Decision Support System** |
| ![Project Header](https://kppmch-pregnant.vercel.app/og-image.png) |

---

| CLINICAL STRATEGY & NURSING REQUIREMENTS | | |
| :--- | :--- | :--- |
| **Requirement Source** | **Clinical Target** | **Architectural Outcome** |
| **Senior Nursing Staff** | High-Risk Pregnancy Tracking | Automated data capture for proactive maternal monitoring. |
| **Professional Standard** | Continuity of Care | **Asynchronous Operations** ensuring no data loss during tracking. |
| **Maternal Safety** | Real-time Alerting | Logic-based triggers via LINE API for immediate nursing response. |

---

| 1. CORE TECHNICAL ARCHITECTURE | | |
| :--- | :--- | :--- |
| **Category** | **Technology Stack** | **Architectural Role** |
| **Framework** | Next.js 14 (App Router) | High-performance interface for complex clinical data entry. |
| **Logic Layer** | Clean Architecture | **Decoupled Business Logic** to allow easy medical protocol updates. |
| **Interface** | LINE Messaging API | Direct communication channel between patients and nurses. |
| **Data Engine** | GAS Webhook + Sheets | Serverless backend designed for hospital-scale data collection. |

---

| 2. SYSTEM INTEGRITY & DATA FLOW | | |
| :--- | :--- | :--- |
| **Component** | **Technical Implementation** | **Benefit to Nursing Workflow** |
| **Asynchronicity** | Non-blocking GAS calls | Seamless patient registration without system delays. |
| **Validation** | Server-side Data Sanitization | Ensures 100% accuracy of pregnancy-related metrics (e.g., GA, EDD). |
| **Deployment** | Vercel (CI/CD) | Zero-downtime updates for critical healthcare features. |
| **Architecture** | Scalable Modular Design | Ready for future integration with existing HIS/EMR systems. |

---

| 3. SECURITY & CONFIGURATION | |
| :--- | :--- |
| **Variable Key** | **Description / Security Implementation** |
| `LINE_ACCESS_TOKEN` | Authorized Messaging API token for secure patient communication. |
| `LINE_SECRET` | Channel secret validation to prevent unauthorized payload access. |
| `GAS_WEBHOOK_URL` | Secure Google Apps Script endpoint for clinical data storage. |

---

| 4. OPERATIONS & DEPLOYMENT | |
| :--- | :--- |
| **Phase** | **Command / Task** |
| **Setup** | `npm install && cp .env.example .env.local` |
| **Local Run** | `npm run dev` |
| **Maintenance** | Automated CI/CD Pipeline via Vercel |

---

| 5. CONTACT & CREDITS | |
| :--- | :--- |
| **Lead Developer** | Ratchanon Noknoy |
| **Clinical Partner** | Developed with Senior Professional Nursing Standards |
| **LinkedIn** | [linkedin.com/in/ratchanon-noknoy/](https://www.linkedin.com/in/ratchanon-noknoy/) |
| **GitHub** | [github.com/ratchanon-noknoy2318](https://github.com/ratchanon-noknoy2318) |
| **License** | MIT © 2026 |
