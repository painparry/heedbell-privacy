# Privacy Policy for Heedbell

**Last Updated:** November 1, 2026  
**Effective Date:** November 1, 2026

**Heedbell** ("we", "our", or "us"), developed by **Magicsoft Labs**, is an offline-first subscription and trial reminder manager for Android (Application ID: `com.heedbell.app`).

Your privacy is fundamental to the design of Heedbell. This Privacy Policy explains our practices regarding your data when you use the Heedbell mobile application.

---

## Short Summary: The Privacy Promise

- **No Account Required:** You do not need to register, provide an email address, or sign in to use Heedbell.
- **Offline-First:** All your subscriptions, trial details, billing cycles, notes, and payment methods are stored locally on your device in a private SQLite database.
- **No Tracking or Advertising:** We do not track you. We do not use third-party analytics SDKs, advertising networks, crash-reporting trackers, or tracking cookies.
- **No Developer Servers:** We do not operate remote backend servers that collect or store your personal subscription records.
- **You Own Your Data:** You can export, back up, and completely erase your data at any time directly within the application.

---

## 1. Information We Do NOT Collect

We do not collect, transmit, or store on any external server:
- Personal Identifiable Information (PII) such as your name, email, phone number, or physical address;
- Financial credentials, bank account numbers, credit card details, or banking passwords;
- Details of your individual subscriptions, active trials, amounts paid, or renewal cycles;
- Identifiers such as Android Advertising ID (AAID), device fingerprint, or IMEI;
- Geolocation data.

---

## 2. Information Stored Locally on Your Device

Heedbell operates as an offline-first tool. All information entered by you is saved directly on your local device storage inside the app's sandboxed database:
- **Subscription Records:** Service names, custom icons/colors, prices, billing frequencies, renewal dates, reminder schedules, and free trial end dates;
- **User Categories & Labels:** Custom categories, tags, payment method labels (e.g., "PayPal", "Card"), and cancellation notes/links;
- **Application Preferences:** Theme selection (Light/Dark/AMOLED/Accent color), main display currency, and notification timings;
- **Local Backup Archives:** If you create a backup, an archive file (`.json` or `.csv`) is saved locally to a folder of your choice using the Android Storage Access Framework (SAF).

We have no access to this local data.

---

## 3. Network Communications and Third-Party Services

Heedbell requires minimal internet connectivity (`android.permission.INTERNET`) strictly for two features:

### A. Exchange Rates (Multi-Currency Support)
If you track subscriptions in multiple currencies, Heedbell periodically downloads public foreign exchange rates:
- **Primary Source:** Frankfurter API (`https://api.frankfurter.dev`)
- **Secondary Fallback:** Currency API (`https://cdn.jsdelivr.net` and `https://currency-api.pages.dev`)
- **What is sent:** Standard anonymous HTTP GET requests for public rate tables (e.g. `USD`, `EUR`).
- **What is NOT sent:** No user identifiers, device IDs, subscription names, or monetary amounts are ever sent in these requests.
- The exchange rate providers only see standard web protocol metadata (such as your IP address) necessary to fulfill the HTTP response, in accordance with their respective privacy policies.

### B. In-App Purchases (Heedbell Pro)
Heedbell offers an optional one-time purchase ("Heedbell Pro") through the official **Google Play In-App Billing** system:
- All payment transactions are processed entirely by **Google LLC** through Google Play Services.
- We never see, receive, or store your credit card information, bank details, or billing address.
- Google Play provides Heedbell with an anonymous cryptographic purchase token and order entitlement ID solely to verify whether your Pro license is active on your device.
- For more details on how Google processes payment data, please review the [Google Play Privacy Policy](https://policies.google.com/privacy).

### C. External Cancellation & Service Links
Heedbell allows you to save direct cancellation URLs (e.g., a link to an account management page). Tapping "Open cancel page" launches your device's default web browser. Any interaction with external websites is governed by the respective third party's privacy policy.

---

## 4. Device Permissions Used

Heedbell requests only the minimum Android permissions necessary to function:
- **`POST_NOTIFICATIONS` (Android 13+):** Used solely to display local reminder notifications before your trials end or subscriptions renew.
- **`INTERNET`:** Required to download public exchange rates and verify Google Play purchases.
- **`RECEIVE_BOOT_COMPLETED`:** Required to reschedule your local notification alarms after your device restarts.
- **`SCHEDULE_EXACT_ALARM` / `USE_EXACT_ALARM` (or inexact battery-optimized alarms):** Used to trigger reminders accurately at the time you chose.

We do NOT request access to:
- Contacts or phone state;
- Precise or coarse location;
- Camera, microphone, or photos;
- Broad device storage (we use system Storage Access Framework for backups).

---

## 5. Data Retention, Backup, and Deletion

### Data Retention
Because your data is stored exclusively on your device, it remains on your device until you choose to delete it or uninstall the app.

### Data Export (Portability)
You can export your complete subscription database at any time in open JSON or CSV formats via **Settings → Backup and Export**.

### Complete Data Deletion
You have complete control to wipe all data at any moment:
1. **Within the App:** Go to **Settings → Delete all data** and confirm. This immediately wipes all subscriptions, payment logs, custom categories, and preferences from the local database.
2. **Via Android Settings:** Go to **Android Settings → Apps → Heedbell → Storage → Clear Data**, or simply uninstall the application. All local sandboxed files and databases are permanently deleted by the operating system.

---

## 6. Children's Privacy

Heedbell is a general audience productivity tool and is not directed at children under the age of 13 (or under 16 in the European Union). We do not knowingly solicit or collect information from children.

---

## 7. Compliance with Global Privacy Regulations

### European General Data Protection Regulation (GDPR)
Under the GDPR, you have the right to access, rectify, port, and erase your personal data. Because Heedbell does not collect your data on remote servers, you can exercise these rights directly on your device at any time:
- **Access & Portability:** Export your records via JSON/CSV export.
- **Rectification:** Edit any subscription or category within the app.
- **Erasure:** Tap "Delete all data" in Settings or uninstall the app.

### California Consumer Privacy Act (CCPA / CPRA)
Heedbell does not "sell" or "share" personal information as defined by the CCPA/CPRA. We do not engage in targeted advertising, profiling, or cross-context behavioral tracking.

---

## 8. Changes to This Privacy Policy

We may update this Privacy Policy from time to time. Any changes will be posted on this page with an updated "Last Updated" date. We encourage you to review this policy periodically.

---

## 9. Contact Us

If you have any questions, feedback, or concerns regarding this Privacy Policy or your data, please contact:

**Developer:** Magicsoft Labs  
**Email:** [apple.developer.lab@gmail.com](mailto:apple.developer.lab@gmail.com)  
