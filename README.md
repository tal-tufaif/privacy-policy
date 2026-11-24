# Privacy Policy for CCCompanion

**Extension Name:** CCCompanion  
**Version:** 5.1.72  
**Publisher:** Tayseer Al-Tufaif  
**Contact:** [t_tufaif@hotmail.com](mailto:t_tufaif@hotmail.com)  
**Last Updated:** November 24, 2026  
**Live Policy Page:** [https://tal-tufaif.github.io/privacy-policy/](https://tal-tufaif.github.io/privacy-policy/)

---

### Overview
CCCompanion is a clinical workflow automation extension for healthcare professionals using authorized Saudi Ministry of Health (MOH) and Eastern Health Cluster (EHC) clinical systems. This Privacy Policy discloses exactly what user data is collected, accessed, handled, stored, and shared—including local browser storage and user-initiated submissions to authorized institutional clinical portals.

---

### 1. Single Purpose & Authorized Portals
CCCompanion's single purpose is to streamline repetitive outpatient clinical documentation, e-prescription reorders, and care-coordination workflows directly inside authorized institutional portals:
* **Raqeem Health Information System (HIS):** `https://moh.raqeem.sa/*`, `https://raqeem.anat.sa/*`
* **Wasfaty E-Prescription Portal:** `https://pp.wasfaty.sa/*`, `https://wasfatypp.moh.gov.sa/*`
* **Eastern Health Cluster (EHC) Clinical Forms / REDCap:** `https://tforms.ehc.med.sa/*`, `https://*.ehc.med.sa/*`
* **Authorized Institutional Analytics Dashboards:** `http://taamanalytics.ehc.med.sa/*`, `https://taamanalytics.ehc.med.sa/*`, `https://metabase.ehcdhn.online/*`, `https://app.powerbi.com/*`

---

### 2. User Data Collection

#### A. Data Categories Accessed, Processed, or Collected
* **Personally Identifiable Information (PII):** 10-digit Saudi National IDs / Iqama numbers detected when a clinician highlights/right-clicks an ID or triggers a quick-search/follow-up action from a patient chart or authorized BI dashboard, strictly to locate the patient record in Raqeem or attach a follow-up note in EHC REDCap.
* **Health Information:** Active consultation context displayed inside Raqeem HIS (vital signs, lab results, ICD-10 diagnosis codes, patient weight for pediatric dosing, and Wasfaty e-prescription reference IDs), clinician-selected medication reorder lists transferred to Wasfaty, and clinician-entered TBC follow-up note data (`note`, `text`, `tot`, `date`).
* **Website Content:** Active DOM text, table structures, form inputs, and same-origin portal API responses (Raqeem XHR responses for Wasfaty IDs) strictly on the authorized portals listed in Section 1.
* **User Configuration & Custom Macro Presets:** Custom ICD-10 note templates and feature toggles configured by the user in `options.html`.

#### B. Data Categories NOT Collected
* **No Authentication Credentials:** Does not read, store, or collect passwords, PINs, OTPs, or login credentials.
* **No Financial or Payment Information:** Does not collect credit card or payment data.
* **No Location Data:** Does not collect GPS or IP geolocation data.
* **No General Web Browsing History or Personal Communications:** Does not track browsing outside authorized portals or access emails/chats.
* **No User Activity Tracking / Telemetry:** Does not log keystrokes, mouse movements, or analytics.

---

### 3. Data Handling & Usage
* **In-Page Clinical Formatting & Assistance:** Clinical vitals, lab tables, summary column tidying, ICD-10 macro insertion, and weight-based dosage checks execute locally in browser memory.
* **Quick Patient Lookup:** Passes a selected National ID locally to fill the Raqeem Registration search input in the clinician's authenticated tab.
* **Cross-Tab Wasfaty Order Handoff:** Temporarily stages selected medication queues in `chrome.storage.local` (`ccc_wasfaty_order_queue`), populates the Wasfaty portal form (`pp.wasfaty.sa` / `wasfatypp.moh.gov.sa`), and clears the queue upon completion.
* **User-Initiated Institutional TBC Note Submission:** Only when the clinician explicitly clicks *Save & Submit* in the TBC Note modal, the extension transmits the National ID, follow-up note code, optional remarks, TOT indicator, and date via HTTPS `POST` directly to the authorized institutional EHC REDCap API (`https://tforms.ehc.med.sa/api/`).
* **Prohibited Uses:** Data is never used for advertising, marketing, creditworthiness evaluation, data brokering, or AI model training.

---

### 4. Data Storage, Retention, and Deletion
* **Local Device Storage (`chrome.storage.local` & `localStorage`):** Presets and feature toggles remain stored locally until edited/deleted via `options.html` or until the extension is uninstalled. Temporary Wasfaty queues (`ccc_wasfaty_order_queue`) are automatically deleted after transfer completion.
* **Institutional Server Storage (EHC REDCap):** TBC follow-up notes explicitly submitted by clinicians reside in the Eastern Health Cluster REDCap database (`tforms.ehc.med.sa`) under EHC/Saudi MOH institutional governance. The developer does not operate an independent external backend database.

---

### 5. Data Sharing & All Third Parties
**Comprehensive List of All Parties User Data May Be Shared With or Transferred To:**
1. **Eastern Health Cluster (EHC) / Saudi Ministry of Health Institutional REDCap System (`https://tforms.ehc.med.sa/`):** Receives user-submitted TBC clinical follow-up note records (`national_id`, note code, remarks, TOT flag, date) exclusively when explicitly submitted by a clinician.
2. **Authorized Clinical Portals Operated by the User's Institution (`moh.raqeem.sa`, `raqeem.anat.sa`, `pp.wasfaty.sa`, `wasfatypp.moh.gov.sa`):** User-initiated actions populate form inputs directly within the clinician's authenticated tabs.
3. **Commercial Third Parties, Advertisers, Data Brokers, Analytics Vendors, or Unrelated External Servers:** **NONE.**

---

### 6. Permissions & Host Access Justification
* **`storage`:** Saves custom clinical presets locally and temporarily stages Wasfaty medication reorder queues between Raqeem and Wasfaty tabs.
* **`contextMenus`:** Adds right-click shortcuts ("Search in Raqeem" and "Fill TBC Note") for selected National IDs.
* **`tabs`:** Detects or opens authorized Raqeem and Wasfaty tabs for patient lookups and e-prescription handoff.
* **Host Permissions & Content Scripts:** Required to inject workflow UI helpers on Raqeem and Wasfaty, capture selected National IDs on authorized BI dashboards (`taamanalytics.ehc.med.sa`, `metabase.ehcdhn.online`, `app.powerbi.com`), handle EHC survey popups (`*.ehc.med.sa`), and submit user-initiated TBC notes to `tforms.ehc.med.sa/api/`.

---

### 7. Security & User Consent
* **Prominent Disclosure & Affirmative Consent:** Data handling is prominently disclosed in the Chrome Web Store listing and this Privacy Policy. External transmissions and lookups execute only upon explicit clinician interaction.
* **Transport Encryption:** Transmissions to `https://tforms.ehc.med.sa/api/` are encrypted via HTTPS/TLS with `credentials: 'omit'`.
* **No Remote Code:** Zero remote code execution or external scripts.

---

### 8. Chrome Web Store Limited Use Compliance
The handling and use of all user data received or processed by CCCompanion strictly adheres to the **Chrome Web Store User Data Policy**, including the **Limited Use** requirements, as well as the Microsoft Edge Add-ons Developer Policies.

---

### 9. Contact & Inquiries
* **Developer / Publisher:** Tayseer Al-Tufaif
* **Email:** [t_tufaif@hotmail.com](mailto:t_tufaif@hotmail.com)
* **Live Policy URL:** [https://tal-tufaif.github.io/privacy-policy/](https://tal-tufaif.github.io/privacy-policy/)
