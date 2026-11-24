# Privacy Policy for CCCompanion

**Extension Name:** CCCompanion  
**Target Version:** 5.1.72  
**Publisher:** Tayseer Al-Tufaif  
**Contact:** [t_tufaif@hotmail.com](mailto:t_tufaif@hotmail.com)  
**Last Updated:** November 24, 2026  
**Live Policy Page:** [https://tal-tufaif.github.io/privacy-policy/](https://tal-tufaif.github.io/privacy-policy/)

---

### Summary
CCCompanion functions 100% locally in your browser. It does not operate remote servers, does not transmit user data across networks, and shares zero information with third parties. All user macros and templates stay securely stored on your local machine.

---

### 1. Overview & Single Purpose
CCCompanion is a specialized clinical workflow automation extension built for healthcare professionals and care coordinators operating within the Saudi Ministry of Health (MOH) **Raqeem Health Information System** (`moh.raqeem.sa`, `raqeem.anat.sa`) and the **Wasfaty** electronic prescription platform (`wasfaty.sa`).

**Single Purpose:** To streamline repetitive outpatient clinical documentation tasks by assisting clinicians with visit note templating, ICD-10 diagnosis code shortcuts, and electronic prescription navigation directly within their active medical record sessions.

---

### 2. User Data Collection
In accordance with the Chrome Web Store User Data Policy, this section comprehensively discloses what data is collected and what data is not collected:

#### A. What Data Is Collected Locally
* **User Configuration & Macro Presets:** Custom text templates, ICD-10 note shortcuts, and UI display preferences that you explicitly create and save in the extension options page. This information is stored exclusively on your local device.

#### B. What Data Is NOT Collected
* **No Personally Identifiable Information (PII):** CCCompanion does not collect or transmit names, national IDs, email addresses, phone numbers, ages, or personal identities.
* **No Protected Health Information (PHI) / Clinical Records:** CCCompanion does not collect, record, log, or transmit patient medical histories, clinical diagnoses, vital signs, prescriptions, or encounter records.
* **No Authentication Credentials:** CCCompanion does not intercept, read, or store passwords, OTP tokens, MFA codes, or portal credentials.
* **No Browsing History or Web Activity:** CCCompanion does not track or collect web browsing history, visited URLs outside the designated institutional portals, clicks, mouse tracking, or keystroke logs.
* **No Financial or Payment Information:** CCCompanion does not handle financial transactions, credit cards, or billing information.
* **No Location Data:** CCCompanion does not access or store GPS, IP location, or geographical tracking data.

---

### 3. Data Handling & Usage
This section outlines how user information is handled, processed, and utilized:
* **Sole Purpose Processing:** All user-configured templates are utilized solely to fulfill the extension's narrow single purpose—enabling quick insertion of clinical notes into active form fields when initiated by the clinician.
* **In-Memory Processing:** Any dynamic text manipulated during an active clinical encounter is processed purely in volatile browser memory and is discarded immediately once the browser tab or session is closed.
* **No External Server Processing:** CCCompanion does not maintain an external API, database, or backend server. No calculations or data parsing occur on external infrastructure.
* **No Commercial Profiling or Advertising:** Stored data and templates are never used for marketing, advertising, ad targeting, credit evaluation, or personalized profiling.

---

### 4. Data Storage, Retention, and Deletion
This section explains where data resides, how long it is retained, and how users maintain complete control over deletion:
* **Storage Location:** All saved configuration settings, macro templates, and shortcut preferences reside strictly on the user's local device via the standard Chromium local storage API (`chrome.storage.local`).
* **Data Retention Period:** Data is retained locally on your computer for as long as you keep the extension installed and wish to maintain your custom templates.
* **User Deletion & Control:**
  * Users can modify, clear, or delete individual templates and presets at any time via the extension's built-in **Options** page.
  * Uninstalling CCCompanion immediately and permanently deletes all locally stored extension data and preferences from your browser.
  * Clearing browser cache/extension storage through browser settings will also wipe all saved configuration data.

---

### 5. Data Sharing & Third Parties
> **All parties the user data will be shared with: NONE.**

CCCompanion does not transfer, sell, rent, license, or disclose user data to any external parties under any circumstances. Specifically:
* **No Third-Party Sharing:** Zero user data, configuration data, or clinical text is shared with third-party companies, vendors, or services.
* **No Ad Networks or Brokers:** We do not sell or monetize user information to data brokers, ad networks, or commercial entities.
* **No Analytics or Tracking SDKs:** CCCompanion does not embed Google Analytics, Mixpanel, telemetry beacons, tracking pixels, or third-party marketing SDKs.

---

### 6. Permissions and Scoped Use
CCCompanion requests only the minimum necessary permissions required to operate:
* **Host Permissions (`moh.raqeem.sa`, `raqeem.anat.sa`, `wasfaty.sa`):** Restricted strictly to injecting clinical automation content scripts into designated institutional healthcare portals to assist clinicians with form filling. No data is extracted or transmitted outside these origins.
* **Storage (`chrome.storage.local`):** Required to preserve user-customized clinical note presets and options locally on the device.
* **Context Menus (`contextMenus`):** Enables right-click context menu shortcuts for quick template insertion inside the Raqeem interface.
* **Tabs (`tabs`):** Used exclusively to detect existing hospital portal tabs and open the local extension configuration (`options.html`) page.

---

### 7. Remote Code and Security Practices
* **Zero Remote Code:** In strict compliance with Chrome Web Store and Microsoft Edge policies, CCCompanion does not load, fetch, or execute any remote code, eval() statements, dynamic external scripts, or remote WebAssembly. All executable code is packaged locally within the published extension archive.
* **Volatile Memory Only:** Clinical form interactions happen entirely within the active DOM session. No copies of clinical consultations or patient files are written to disk.

---

### 8. Compliance with Store Developer Policies
This privacy policy complies with the **Google Chrome Web Store Developer Program Policies** (including the User Data FAQ, Prominent Disclosure, and Limited Use requirements) and the **Microsoft Edge Add-ons Developer Policies**.

---

### 9. Contact & Support
If you have any questions, inquiries, or feedback regarding CCCompanion or this Privacy Policy, please contact:
* **Developer / Publisher:** Tayseer Al-Tufaif
* **Email:** [t_tufaif@hotmail.com](mailto:t_tufaif@hotmail.com)
* **Live Policy URL:** [https://tal-tufaif.github.io/privacy-policy/](https://tal-tufaif.github.io/privacy-policy/)
