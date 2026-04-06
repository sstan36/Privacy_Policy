# Privacy Policy — TianJi (Firebase iOS)

**Controller:** **Michael Tan** (“**we**,” “**us**,” “**our**”)  
**App:** TianJi — Your Destiny is unfolding…  
**Product type:** BaZi (Four Pillars) chart application for iOS  
**Bundle identifier:** `com.nexazenith.FirebaseApi`  

**Published copy (this policy online):** [HTML (recommended)](https://sstan36.github.io/Privacy_Policy/privacy_policy.html) · [Markdown source](https://sstan36.github.io/Privacy_Policy/privacy_policy.md)  

**Effective date:** 30 March 2026  
**Last updated:** 5 April 2026  

This Privacy Policy explains what information is processed when you use our App, how we use it, and your choices. **Privacy laws vary by region.** Before you rely on this document for compliance or litigation, consider **having qualified counsel review** the final version.

---

## Framework and references (Singapore and Apple)

**Singapore (PDPA).** Where the Personal Data Protection Act 2012 applies to our activities, we intend to comply with its rules on collection, use, and disclosure of personal data, subject to exceptions in the Act. Official overview: [PDPC — Personal Data Protection Act](https://www.pdpc.gov.sg/overview-of-pdpa/the-legislation/personal-data-protection-act). We also have regard to PDPC’s [Advisory Guidelines on Key Concepts in the PDPA (PDF, 17 May 2022)](https://www.pdpc.gov.sg/-/media/files/pdpc/pdf-files/advisory-guidelines/ag-on-key-concepts/advisory-guidelines-on-key-concepts-in-the-pdpa-17-may-2022.pdf) when describing purpose, consent, and protection. PDPC materials are authoritative; this Policy is app-specific notice.

**Further reading (non-authoritative).** [SingaporeLegalAdvice.com — Drafting a comprehensive privacy policy for a Singapore website](https://singaporelegaladvice.com/law-articles/drafting-comprehensive-privacy-policy-singapore-website/) (educational). [Law Society of Singapore — Privacy Policy](https://www.lawsociety.org.sg/privacy-policy/) is cited only as an example of PDPA-style structuring; we are not affiliated.

**Apple.** The App is on the App Store. We follow applicable Apple program, review, and privacy-label requirements. See [Apple Privacy Policy](https://www.apple.com/legal/privacy/) and [App Store Review Guidelines](https://developer.apple.com/app-store/review/guidelines/). If the App Store listing or Apple rules conflict with this document, the listing and Apple’s published requirements govern for distribution.

---

## Summary (plain language)

- **What the App does today:** The App is built around **BaZi (Four Pillars) chart generation** and related features we ship in the store build. **Narrative or generative “reading” features are not part of the current public product** described in detail here; if we add them later, we will update this Policy and App Store disclosures first.
- **No ads, no sale of personal data:** We **do not** show third-party ads. We **do not** sell personal information. We **do not** use your information for **cross-app or cross-website tracking** for advertising.
- **No analytics or crash reporting (current):** We **do not** use **Firebase Analytics**, **Crashlytics**, or other third-party **analytics or crash reporting** services in the App **at this time**.
- **No push ads stack:** We **do not** use **Firebase Cloud Messaging**, **Remote Config** for ad/mar-tech style targeting, **AdMob**, or similar advertising or tracking SDKs.
- **Backend:** We use **Firebase Cloud Functions**, **Firestore**, **Firebase App Check** with **Apple App Attest** (on supported devices), **Firebase Anonymous Authentication** (pseudonymous ID per installation for backend calls), and **Google Secret Manager** (or the same project’s **server-side secret/parameter system**) so **secrets stay off the device**.
- **Minimal processing:** We process information **only** to operate the App (charts, optional purchases, security, reliability, and support **you** start). We **do not** ask for contacts, your photo library, or precise location **for chart features**.
- **Support diagnostics (optional):** If you choose **Contact support** in Settings, you may send a short **on-device diagnostic log** and basic device/app metadata **only in that email**. We design the log **not** to include birth details, raw chart JSON, or similar content unless **you** put them in the email body. See **Support diagnostics and email** below.

If anything in this Policy conflicts with the **App Store listing**, in-app disclosures, or **Apple’s requirements**, treat the listing and Apple’s rules as controlling for distribution and **reconcile any mismatch with qualified counsel**.

---

## 1. Who we are

This Privacy Policy applies to **Michael Tan** and the TianJi iOS application and its use of **Google Firebase and Google Cloud** as described below (and **Apple** for the App Store, StoreKit, and platform services).

**Contact details** appear in **Section 16 (Contact us)**.

---

## 2. Scope

The App lets you create and manage **BaZi charts** using traditional computational methods, with **online backend support** where a feature needs it. **This policy covers:**

- Information processed **on your device**
- Information processed through our **current backend** (see **Backend services** below)
- Information you **voluntarily email** to us through **Contact support**

It does **not** cover third-party sites or services we do not control.

### Backend services (current production)

We use **only** these parts of Firebase / Google Cloud for the live App:

| What | Role |
|------|------|
| **Firebase Cloud Functions** | Runs **server-side** logic when you call the backend (for example chart-related requests). **Secrets** needed for those calls (such as API keys) are kept in **Google Secret Manager** or another **Google Cloud server-side secret/parameter store**, **not** in the App binary. |
| **Firestore** | Stores **data the product needs on the server** (for example fields related to chart limits, purchases or entitlements, sync or bookkeeping fields the server maintains). **Only** what the App sends and what the backend writes for these purposes is stored here. |
| **Firebase App Check** | Uses **Apple App Attest** on real devices (where available) so our backend can treat traffic as more likely to come from the **genuine App**, which **reduces abuse and unauthorised API use**. |
| **Firebase Anonymous Authentication** | Gives your installation a **pseudonymous Firebase user ID** so Cloud Functions and Firestore rules can run **without** you creating a username or password. |

We **do not** use **Firebase Analytics**, **Crashlytics**, **Remote Config**, **Firebase Cloud Messaging** (push), **AdMob**, or other Firebase products **beyond** what is listed above **in the current release**.

---

## 3. Categories of information we process

We align our descriptions with how **Apple** and common privacy laws refer to “personal information” or “personal data.” **Information you enter** to generate a chart (for example **birth date, birth time, timezone, and gender**) is **personal information** because it identifies or relates to a person. We process it **only** as described here.

### 3.1 Information you provide (chart inputs)

When you create or edit a chart, you may enter:

- An optional **label or name** for the chart
- **Date of birth**, **time of birth**, **timezone**, and **gender** (needed for BaZi calculation)
- Notes or labels you choose to store **locally** with the chart

Avoid entering unnecessary sensitive information; you are responsible for accuracy.

### 3.2 Information stored on your device

The App uses **Apple frameworks** to store data **on your device**, including:

- **Core Data:** Saved charts and related metadata (for example validation flags or timestamps if the App stores them)
- **Keychain:** Identifiers related to **entitlements** (for example chart-slot or installation-correlation identifiers)
- **UserDefaults** (or similar): Preferences such as disclaimer acceptance, language, or internal counters

Unless that data is **sent to our servers** as described below—or you export or share it yourself—we **cannot access** purely on-device content.

### 3.3 Information processed on our servers

When you use **backend-linked** features (for example **generating** a chart or keeping **purchase-related** entitlements in sync), the App sends requests to **Cloud Functions** and may read or write **Firestore** as the product requires. Processing may include:

- Your **Firebase Anonymous Authentication** user ID and related session/App Check data needed to **authorise** the request
- **App version** and an **installation correlation identifier** where we need it for **support** or **consistent entitlements** after reinstall
- **Firestore fields** described in **Section 2** (limits, entitlements, timestamps, integrity fields)
- **Request payloads** needed for the operation—typically **birth-related inputs** and/or **structured BaZi data** produced by calculation

**Chart inputs and outputs are sensitive.** We use **encryption in transit (HTTPS)** and restrict access using **reasonable admin and cloud controls**.

### 3.4 Technical and security data

When you use online features, **Google Cloud / Firebase** will process ordinary **technical metadata** needed to deliver the service: for example **IP address**, **timestamps**, **request headers**, **TLS information**, and **operational logs** tied to Cloud Functions, Firestore, and App Check.

**We do not** use **Firebase Analytics**, **Crashlytics**, or other **Firebase** products to collect **product analytics** or **crash reports** **in the current App**. We **do not** use **cookies** or mobile ad IDs for **advertising** or **cross-app profiling**.

---

## 4. Support diagnostics and email (user-initiated)

You may use **Settings → Contact support** (when present) to **open an email** to us. **Nothing is sent automatically.** You decide whether to tap send.

**What the email may include (by design):**

- **Device and app metadata** the composer adds for troubleshooting (for example device model, iOS version, app version, locale)
- A **short excerpt** of an **on-device diagnostic log** for recent errors

**What belongs out of the log:** We intend **not** to write **raw chart JSON**, **birth dates or times**, **prompt text**, or similar **chart-identifying content** into this log. Entries should be **short technical lines** (for example error domain, code, short message) so we can debug **without** unnecessary personal detail.

**If you need to share sensitive chart data** to resolve a bug, do that **only** if you **choose** to type or attach it in the email. We will use **only** what you send **to answer** your support request, subject to normal support and legal retention.

---

## 5. How we use information

We use information to:

- **Generate, display, and store** BaZi charts (including **server-side** steps that run in **Cloud Functions** when you use online features)
- Keep **anonymous sign-in**, **rate limits**, **entitlements**, and **server-side records** consistent where those features exist
- **Protect** the backend (**App Check** / **App Attest**, abuse patterns)
- **Run** and **maintain** the service (for example outages, misconfiguration, **security**)
- **Respond** to support requests **you** send
- **Comply with law** and our **Terms of Use**

Charts and metadata are **not** medical, legal, financial, or other professional advice. See **Terms of Use & Disclaimer** in the App.

---

## 6. Generative AI and readings

**Today’s public App** is focused on **BaZi chart generation** and supporting mechanics we describe above. **We do not** ship **separate narrative “AI reading”** or **generative chat** products in this Policy as **live features**. If we **later** turn those on in a **public** build, we will **update this Policy** and **App Store privacy answers** (and in-app notice where needed) **in the same release window**, not before promising them here.

---

## 7. Legal bases (EEA / UK–style laws)

Where **GDPR** or similar laws apply, we typically rely on:

- **Performance of a contract** (providing the App and features you request, including paid items)
- **Legitimate interests** (security, fraud and abuse prevention, reliable operation, correlating support with technical context), balanced against your rights
- **Consent** where the law requires it for a specific processing activity

Contact us if you need jurisdiction-specific information.

---

## 8. Sharing and subprocessors

We share information with:

| Recipient | Role |
|-----------|------|
| **Google (Firebase / Google Cloud)** | **Cloud Functions**, **Firestore**, **App Check**, **Anonymous Authentication**, and **Secret Manager** (or equivalent server secret storage) as described in **Section 2**. See [Firebase Privacy and Security](https://firebase.google.com/support/privacy). |
| **Apple** | App distribution, **App Store** purchases, **StoreKit**, **App Attest** (via Apple’s platform for App Check) — see [Apple’s Privacy Policy](https://www.apple.com/legal/privacy/). |
| **Professional advisers or authorities** | When required by law or to protect rights and safety |

We **do not sell** personal information. We **do not** share it for **cross-context behavioural advertising**.

---

## 9. Retention

- **On-device data:** Stays on the device until **you delete charts or app data in the App**, **uninstall** the App, or **erase** the device. We **cannot** delete your **local-only** files from our side.
- **Server-side data (Firestore / related):** Kept only as long as needed to **provide** the service, meet **legal** duties, resolve disputes, and enforce agreements. We may run **deletion or cleanup** on anonymous IDs and Firestore documents according to those needs.
- **Support emails:** May be kept for a **reasonable period** to finish the thread and for **internal quality**, unless law requires longer.

---

## 10. Security

We use measures appropriate to the risk: **HTTPS**, **access controls** on cloud resources, **Firebase App Check** to reduce abuse, and **server-only** storage of sensitive credentials in **Secret Manager** (or the same kind of **managed secret system**) so they are **not embedded in the client** for server operations. **No method of storage or transmission is completely secure.**

---

## 11. Children’s privacy

The App is **not directed to children** under **13** (or the higher age required in your region). We do **not knowingly** collect personal information from children. If you believe we have, contact us and we will take appropriate steps.

---

## 12. International transfers

If you use the App from outside the region where our Firebase project is hosted, data may be processed in the **United States** and other regions where **Google Cloud** operates. Where required, we rely on appropriate mechanisms (for example **standard contractual clauses**).

---

## 13. Your rights and choices

Depending on where you live, you may have rights to **access**, **correct**, **delete**, **export**, **object to**, or **restrict** processing, and to **withdraw consent** where processing is consent-based.

**On-device data:** Delete charts or reset data **in the App**, or **uninstall**. That removes local copies from **your** device; it **does not**, by itself, erase **Firestore** rows your user ID may still have.

**Server-side data:** Email **tianjisupport@gmail.com** from an address you can receive mail at. Describe your request (**delete my server-side records**, **access**, etc.). Because we use **anonymous Firebase accounts**, we may ask for **reasonable information** (for example your support email thread, approximate purchase date, or other non-sensitive cues) to match your request to the right **anonymous ID**. Where **deletion** is possible, we will **delete or anonymise** relevant Firestore records and related server data we **control**, subject to **legal** retention needs.

**iOS:** You can uninstall the App and use system **privacy** and **network** settings Apple provides.

We will respond within the time **applicable law** requires where that applies.

---

## 14. California and other U.S. state privacy notices (summary)

Under certain **U.S. state** privacy laws, you may have rights such as **access**, **deletion**, **correction**, **opt-out of sale/sharing**, and **appeal**. We **do not sell** personal information and **do not** use **cross-context behavioural advertising** as described in those laws for our App. For requests, contact **tianjisupport@gmail.com**. We **do not discriminate** against you for exercising these rights.

**Categories** of personal information are in **Section 3**. **Purposes** are in **Section 5**.

---

## 15. Changes to this Policy

We may update this Privacy Policy to reflect product, legal, or operational changes. We will revise the **“Last updated”** date and, where appropriate, provide **notice in the App** or by other lawful means.

---

## 16. Contact us

**Michael Tan**  
Singapore  

**Privacy & support:** tianjisupport@gmail.com (same address as `SettingsSupportConstants.supportEmailAddress` in the App)

---

### Document control

- **Product name:** TianJi  
- **Platform:** iOS (SwiftUI); backend: **Cloud Functions**, **Firestore**, **App Check** (App Attest on device), **Firebase Anonymous Auth**, **Secret Manager** / server secrets; **no** Analytics, Crashlytics, Remote Config, FCM, AdMob **in current release**.  
- **Launch scope:** Chart generation and related shipped features; **no** live generative “reading” product in this Policy.  
- **Support:** `SupportDiagnosticLog`, `SupportDiagnosticsBridge`, `SupportEmailComposer` — user-initiated email only; log excludes sensitive chart content **by design**; user may still type sensitive data in the email body.  
- **Canonical Markdown:** `FirebaseApi/docs/privacy_policy.md`. Mirror HTML/MD (+ `index.html`) to **Privacy_Policy** repo. **Pages URL:** `https://sstan36.github.io/Privacy_Policy/privacy_policy.html`. In-app: `SettingsSupportConstants.privacyPolicyURL` / `privacyPolicyURLString` (use `.html`).
