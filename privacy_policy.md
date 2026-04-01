# Privacy Policy — TianJi (FirebaseApi iOS)

**Status:** Draft for App Store / in-app display — **have qualified counsel review** before publication.  
**Effective date:** [Insert date]  
**Last updated:** March 25, 2025  

Replace all bracketed placeholders (`[…]`) with your final legal name, contacts, and URLs.

---

## 1. Introduction

This Privacy Policy describes how **[Legal Entity Name]** (“**we**,” “**us**,” or “**our**”) collects, uses, stores, and shares information when you use **TianJi** (the mobile application distributed under bundle identifier `com.nexazenith.FirebaseApi`, together with related backend services, the “**App**”).

By using the App, you agree to this Privacy Policy. If you do not agree, please do not use the App.

## 2. Scope

The App is a **BaZi (Four Pillars)** chart and reading tool. It combines on-device storage with **Google Firebase** backend services and, for certain features, **AI-assisted text generation** on our servers. This policy covers:

- Information processed **on your device**
- Information sent to **our Firebase project** (Authentication, Cloud Functions, Firestore, and related infrastructure)
- **Subprocessors** we rely on (e.g., Google, OpenAI) as described below

This policy does **not** govern third-party websites or services that we do not control.

## 3. Information We Collect

### 3.1 Information you provide

When you create or manage **charts** or request **readings**, you may enter or store data such as:

- **Name** or label for a chart (and optional initials)
- **Date of birth**, **time of birth**, **timezone**, and **gender** (used for chart calculation)
- **Chart and reading content** derived from or related to that input (including structured BaZi data, narrative text, and exports)

You are responsible for the accuracy of the information you enter.

### 3.2 Information stored on your device

The App stores much of your content **locally** using **Apple Core Data**, including:

- Saved charts and associated metadata (for example, validation flags and timestamps)
- Saved readings, including raw responses, formatted content, PDFs where generated, favorites, and archive state

**Keychain** may be used for security-sensitive device identifiers related to **entitlements** (for example, chart-slot or installation-correlation identifiers), consistent with iOS best practices.

**User preferences** (for example, disclaimer acceptance, language settings, or internal counters used to sync state) may be stored in **UserDefaults** or similar on-device storage.

Data stored only on your device is **not** accessible to us unless it is transmitted to our backend as described in this policy or you choose to share it yourself (for example, by exporting or sharing a file).

### 3.3 Information processed on our servers (Firebase)

When you use online features (such as generating or validating a chart, generating readings, or synchronizing purchase-related slot state), the App communicates with **Firebase**. Depending on the feature, our servers may process:

- A **Firebase Anonymous Authentication** identifier (Firebase UID)
- **App version** and a **device installation correlation identifier** (`userUUID`) we use to help with support and entitlement consistency across reinstall or restore
- **Aggregated ledger fields** written to **Firestore** (for example, counts and limits related to saved charts and purchased capacity, sync timestamps, and server-maintained compensation fields we do not allow the client to set)
- **Payloads required to perform the operation**, which typically include birth-related inputs and/or structured BaZi chart data derived in the App or on the server, plus reading parameters (tier, language, category, etc.)

We design Cloud Functions to receive only what is needed to fulfill a request. You should assume that **birth data and chart-derived data are considered sensitive personal information**; treat the App accordingly.

### 3.4 AI processing (OpenAI)

Some readings or validations are produced using **large language models** via **OpenAI** (or comparable providers we may use in the future), called **only from our server environment** (not with your API keys). For those requests, our backend may send **prompt text** that includes chart-related context and structured data sufficient to generate the reading or validation output.

**OpenAI’s use of API data** is governed by OpenAI’s policies applicable to enterprise/API use. We do not intentionally send unrelated device contacts, photos, or location trails for these features; the substantive content is tied to the chart and reading you requested.

### 3.5 Automatic / technical data

Like most mobile apps that use Firebase and cloud infrastructure, Google and we may process certain **technical and operational** data when you use the App, such as:

- IP address and request metadata (via Firebase/Google infrastructure)
- Diagnostic, stability, or usage data if enabled in our Firebase/Google configuration (for example, if Analytics or Crashlytics components are linked in your build)

The exact telemetry products depend on your **Firebase project configuration** and ** Xcode dependency graph**. For Google’s practices generally, see Google’s privacy documentation for Firebase and Google Analytics.

## 4. How We Use Information

We use information to:

- Generate, validate, and display **BaZi charts** using traditional computational rules and our **TianJi** analysis/narrative engine (including server-side libraries)
- Generate and deliver **readings** and related HTML/PDF outputs
- Maintain **anonymous accounts**, **rate limits**, **entitlements**, and **ledger** consistency
- Improve reliability, security, and product quality
- Comply with law and enforce our **Terms of Use**

We do **not** use the App to provide medical, legal, financial, or other regulated professional advice. See the **Terms of Use & Disclaimer** for limitations.

## 5. Legal Bases (if applicable)

If the **GDPR** or similar law applies, we typically rely on:

- **Performance of a contract** (providing the App and purchased digital content you request)
- **Legitimate interests** (security, fraud prevention, improving the service, sync and support correlation), balanced against your rights
- **Consent** where required (for example, certain analytics or marketing, if we add them and ask explicitly)

Laws vary by region; contact us if you need jurisdiction-specific information.

## 6. Sharing of Information

We share information with:

- **Google Firebase / Google Cloud** (hosting, authentication, database, and functions) — see [Google’s Firebase Privacy information](https://firebase.google.com/support/privacy)
- **OpenAI** (when our Cloud Functions call their API to generate text)
- **Apple** (App Store transactions, device and account context governed by Apple’s policies)
- **Professional advisers** (lawyers, accountants) or **authorities** when required by law or to protect rights and safety

We do **not** sell your personal information for money. If we use advertising partners in the future, we will update this policy.

## 7. Retention

- **On-device data** remains until you delete it, uninstall the App, or erase device storage.
- **Server-side data** is retained for as long as needed to operate the App, comply with law, resolve disputes, and enforce agreements. Anonymous Firebase UIDs and Firestore documents may persist until we run maintenance or deletion routines.
- **Logs** (if any) are retained for a limited operational period unless law requires longer storage.

Specific retention schedules may be tightened as the product matures; material changes will be reflected in this policy or in-app notice where appropriate.

## 8. Security

We use industry-standard measures appropriate to the service: encryption in transit (HTTPS), access controls on backend resources, and server-side handling of secrets (for example, **OpenAI keys are not embedded in the App binary**). No method of transmission or storage is 100% secure.

## 9. Children’s Privacy

The App is **not directed to children** under 13 (or the minimum age required in your region). We do not knowingly collect personal information from children. If you believe we have, contact us and we will take appropriate steps.

## 10. International Transfers

If you use the App from outside the country where our Firebase project is hosted, your information may be processed in **the United States** or other regions where Google Cloud, OpenAI, or we operate. We rely on appropriate safeguards where required (for example, standard contractual clauses).

## 11. Your Rights and Choices

Depending on your location, you may have rights to **access**, **correct**, **delete**, **export**, **object to**, or **restrict** certain processing, and to **withdraw consent** where processing is consent-based.

**Practical limitations:** Because the App uses **anonymous Firebase accounts** tied to a device installation, we may not be able to verify identity to the same degree as an email-password service. Deleting the App or requesting account-level deletion workflows (if we offer them) may be necessary to remove server-side identifiers we can associate with your usage.

**iOS controls:** You can uninstall the App, clear local data, limit tracking preferences via Apple settings, and control network access.

To exercise rights, contact us at **[privacy@example.com]** (replace with your address). We will respond within the timeframe required by applicable law.

## 12. California / U.S. State Privacy Notices (summary)

If a U.S. state privacy law applies, you may have additional rights (for example, to opt out of certain “sales” or “sharing” and to appeal decisions). We describe categories of data above. Contact **[privacy@example.com]** for requests. We do not discriminate for exercising rights.

## 13. Changes to This Policy

We may update this Privacy Policy from time to time. We will post the updated version with a new “Last updated” date and, where appropriate, provide notice in the App or by email if we have a direct relationship with you.

## 14. Contact

**[Legal Entity Name]**  
[Street address]  
[City, region, postal code]  

**Privacy inquiries:** [privacy@example.com]  
**General support:** [support@example.com] (align with `SettingsSupportConstants` in the App)

---

### Document control

- **Product name:** TianJi  
- **iOS bundle ID:** `com.nexazenith.FirebaseApi`  
- **Backend (observed in codebase):** Firebase Auth (anonymous), Cloud Functions, Firestore (`users/{uid}` ledger), TianJi library in Functions, OpenAI via server-side `llmService`.
