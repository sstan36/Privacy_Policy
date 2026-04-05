# Privacy Policy — TianJi (Firebase iOS)

**Controller:** **Michael Tan** (“**we**,” “**us**,” “**our**”)  
**App:** TianJi — Your Destiny is unfolding…  
**Product type:** BaZi (Four Pillars) chart application for iOS  
**Bundle identifier:** `com.nexazenith.FirebaseApi`  

**Published copy (this policy online):** [https://sstan36.github.io/Privacy_Policy/privacy_policy.md](https://sstan36.github.io/Privacy_Policy/privacy_policy.md)  

**Effective date:** 30 March 2026  
**Last updated:** 30 March 2026  

This Privacy Policy explains what information is processed when you use our App, how we use it, and your choices. **Privacy laws vary by region.** Before you rely on this document for compliance or litigation, consider **having qualified counsel review** the final version.

---

## Summary (plain language)

- **Launch focus:** At this time, the App is built around **BaZi (Four Pillars) chart generation**. Features such as narrative readings may be **disabled or removed** from the build you download; only the practices described for **chart generation and core app operation** apply unless we ship and disclose additional features.
- **No ads, no data brokerage:** We **do not sell** personal information. We **do not** use your information for **cross-app advertising** or **behavioural advertising** through data brokers.
- **Minimal processing:** We process information **only** to operate the App (charts, optional purchases, reliability, and support you initiate). We **do not** ask for contacts, your photo library, or precise location for chart features.
- **Support diagnostics (optional):** If you choose **Contact support** in Settings, you may send us a short, **on-device diagnostic log** plus basic device/app metadata. That log is designed **not** to include birth details, chart payloads, or other sensitive content—see **Support diagnostics and email** below.

If anything in this Policy conflicts with the **App Store listing**, in-app disclosures, or **Apple’s requirements**, those sources should be reconciled with counsel before release—

---

## 1. Who we are

This Privacy Policy applies to **Michael Tan** and the TianJi iOS application and its use of **Google Firebase** (and, where applicable, **Apple** services such as the App Store and StoreKit).

**Contact details** appear in **Section 16 (Contact us)**.

---

## 2. Scope and launch product

The App lets you create and manage **BaZi charts** using traditional computational methods, with optional online support through our backend. **This policy covers:**

- Information processed **on your device**
- Information sent to **Firebase** (Authentication, Cloud Functions, Firestore, and related Google Cloud infrastructure as configured for our project)
- Information you **voluntarily email** to us through **Contact support**

It does **not** cover third-party sites or services we do not control.

---

## 3. Categories of information we process

We align our descriptions with how **Apple** and common privacy laws refer to “personal information” or “personal data.” **Information you type in** to generate a chart (for example **birth date, birth time, timezone, and gender**) is **personal information** because it identifies or relates to a person. We process it **only** as described here—not for unrelated marketing dossiers or resale.

### 3.1 Information you provide (chart inputs)

When you create or edit a chart, you may enter:

- An optional **label or name** for the chart
- **Date of birth**, **time of birth**, **timezone**, and **gender** (needed for BaZi calculation)
- Any notes or labels you choose to store **locally** with the chart

You should avoid entering unnecessary sensitive information; you are responsible for the accuracy of what you supply.

### 3.2 Information stored on your device

The App uses **Apple frameworks** to store data **on your device**, including:

- **Core Data:** Saved charts and related metadata (for example, validation flags or timestamps if present in your build)
- **Keychain:** Security-sensitive identifiers related to **entitlements** (for example, chart-slot or installation-correlation identifiers), consistent with iOS practice
- **UserDefaults** (or similar): Preferences such as disclaimer acceptance, language, or internal counters used for app state

Unless that data is sent to our servers as described below—or you export or share it yourself—we **cannot access** purely on-device content.

### 3.3 Information processed on our servers (Firebase)

When you use features that call our backend (for example **generating or validating a chart**, or synchronizing **purchase-related** entitlements), the App communicates with **Firebase**. Depending on the operation, processing may include:

- A **Firebase Anonymous Authentication** identifier (Firebase UID)
- **App version** and a **device installation correlation identifier** used for **support** and **consistent entitlements** after reinstall or restore
- **Firestore** fields needed to operate the product (for example, counts or limits related to charts and purchased capacity, sync timestamps, and fields the server maintains for integrity)
- **Request payloads** needed to perform the operation—typically **birth-related inputs** and/or **structured BaZi data** returned from chart computation

**Chart inputs and outputs are sensitive.** We transmit them over encrypted connections and restrict access on the backend using industry-standard controls.

### 3.4 Automatic / technical data

Like most networked apps, **Google** (Firebase / Google Cloud) and we may process **technical data** when you use the App, such as **IP address**, **request metadata**, and (depending on project configuration) **diagnostics or stability** data **if** those products are linked in a given build. For Google’s practices, see [Firebase Privacy and Security](https://firebase.google.com/support/privacy).

We do **not** intend at launch to use such data for advertising profiling; any material change will be reflected here and, where required, in-app.

---

## 4. Support diagnostics and email (user-initiated)

When something goes wrong, you can use **Settings → Contact support** (if available in your build) to open an email to us. **Nothing is sent automatically**; you choose whether to send the message.

**What may be included when you contact us:**

- **Device and app metadata** our composer adds for troubleshooting (for example, model, iOS version, app version, locale—see your build’s implementation)
- A **recent excerpt** of an **on-device diagnostic log** maintained for support

**What we design the diagnostic log to exclude:** We intend **not** to write **raw chart JSON**, **birth dates/times**, **prompt text**, or similar **identifying or chart content** into this log. Entries are meant to be **short, technical summaries** (for example, error domain, code, and brief description) to help us reproduce issues **without** unnecessary personal detail.

If you **manually** type personal information into the email body, that content is treated as information you provided to us for support and is used **only** to respond to your request, subject to ordinary retention for support and legal compliance.

---

## 5. How we use information

We use information to:

- **Generate, validate (if enabled in your build), display, and store** BaZi charts
- Maintain **anonymous authentication**, **rate limits**, **entitlements**, and **ledger** consistency where those features exist
- **Operate, secure, and improve** the service (for example, fixing outages or abuse patterns)
- **Respond** to support requests you send
- **Comply with law** and enforce our **Terms of Use**

Charts and metadata are **not** a substitute for medical, legal, financial, or other professional advice. See your **Terms of Use & Disclaimer**.

---

## 6. Generative AI and readings

**At launch,** this Policy describes an App centered on **chart generation**. We **do not** describe separate **AI narrative reading** products here. If we later enable readings or other **generative-AI** features in a public build, we will **update this Privacy Policy** and, where required, **App Store privacy answers** and in-app disclosures **before** or **concurrent with** that release.

---

## 7. Legal bases (EEA / UK–style laws)

Where **GDPR** or similar laws apply, we typically rely on:

- **Performance of a contract** (providing the App and features you request, including paid items)
- **Legitimate interests** (security, fraud prevention, improving reliability, support correlation), balanced against your rights
- **Consent** where the law requires it (for example, certain optional analytics, if we add them and ask clearly)

Contact us if you need jurisdiction-specific information.

---

## 8. Sharing and subprocessors

We share information with:

| Recipient | Role |
|-----------|------|
| **Google Firebase / Google Cloud** | Hosting, authentication, database, server logic — see [Firebase Privacy and Security](https://firebase.google.com/support/privacy) |
| **Apple** | App distribution, **App Store** purchases, **StoreKit**, and platform services governed by [Apple’s Privacy Policy](https://www.apple.com/legal/privacy/) |
| **Professional advisers or authorities** | When required by law or to protect rights and safety |

We **do not sell** personal information **for money**. We **do not** share information for **cross-context behavioural advertising** as part of our business model.

---

## 9. Retention

- **On-device data** remains until you delete it, uninstall the App, or erase the device.
- **Server-side data** is kept only as long as needed to run the service, comply with law, resolve disputes, and enforce agreements. Maintenance or deletion routines may apply to anonymous IDs and Firestore documents.
- **Support emails and related logs** may be retained for a **reasonable period** to handle your inquiry and for internal quality assurance, unless law requires longer retention.

---

## 10. Security

We use measures appropriate to the risk, including **encryption in transit (HTTPS)**, access controls for backend resources, and **server-side** handling of secrets (**API keys are not embedded in the client for server-only operations**). **No method of storage or transmission is completely secure.**

---

## 11. Children’s privacy

The App is **not directed to children** under **13** (or the higher age required in your region). We do **not knowingly** collect personal information from children. If you believe we have, contact us and we will take appropriate steps.

---

## 12. International transfers

If you use the App from outside the region where our Firebase project is hosted, data may be processed in the **United States** and other regions where **Google Cloud** operates. Where required, we rely on appropriate mechanisms (for example, **standard contractual clauses**).

---

## 13. Your rights and choices

Depending on where you live, you may have rights to **access**, **correct**, **delete**, **export**, **object to**, or **restrict** processing, and to **withdraw consent** where processing is consent-based.

Because we often use **anonymous Firebase accounts** tied to a device installation, **verifying identity** for account-level requests may be limited compared with email-password services. **Deleting the App**, clearing local data, or contacting us for **server-side deletion** (if we offer a process) may be necessary.

**iOS:** You can uninstall the App, adjust tracking-related settings where Apple provides them, and control network access.

To exercise rights, email **tianjisupport@gmail.com**. We will respond within the time required by applicable law.

---

## 14. California and other U.S. state privacy notices (summary)

Under certain **U.S. state** privacy laws, you may have rights such as **access**, **deletion**, **correction**, **opt-out of sale/sharing**, and **appeal**. We **do not “sell”** personal information in the conventional sense described above. For requests, contact **tianjisupport@gmail.com**. We **do not discriminate** against you for exercising these rights.

**Categories of personal information** we process are described in **Section 3**. **Purposes** are described in **Section 5**.

---

## 15. Changes to this Policy

We may update this Privacy Policy to reflect product, legal, or operational changes. We will revise the **“Last updated”** date and, where appropriate, provide **additional notice in the App** or by other lawful means.

---

## 16. Contact us

**Michael Tan**  
Singapore  

**Privacy & support:** tianjisupport@gmail.com (same address as `SettingsSupportConstants.supportEmailAddress` in the App)

---

### Document control

- **Product name:** TianJi  
- **Platform:** Firebase iOS (SwiftUI app; backend Firebase Auth anonymous, Cloud Functions, Firestore ledger as implemented)  
- **Launch scope (policy alignment):** Chart generation focus; reading/generative-AI features **out of scope** for this revision unless and until shipped and disclosed.  
- **Support logging:** On-device diagnostic log and Contact-support flow per `SupportDiagnosticLog`, `SupportDiagnosticsBridge`, and `SupportEmailComposer` (no chart payloads or birth text in log by design).  
- **Two Git check-ins (keep in sync):** Treat **`FirebaseApi/docs/privacy_policy.md`** as the **canonical** copy (commit to the **FirebaseApi** repo). When you change it, **mirror the same text** into the separate **Privacy_Policy** GitHub repo as root **`privacy_policy.md`** (used for **GitHub Pages** at `https://sstan36.github.io/Privacy_Policy/privacy_policy.md`; that repo also has **`index.html`** at root—do not duplicate that file in FirebaseApi `docs/`). The in-app link is **`SettingsSupportConstants.privacyPolicyURL`**.

