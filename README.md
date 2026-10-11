# PocketProof — prototype project

This is a **working local-first UI prototype**, not a finished production app or a ready APK.

## Included in this prototype
- PocketProof branding with shield/check mint icon inspired by the supplied screenshot
- Save receipt, warranty, document, insurance, vehicle and subscription records
- Optional small photo/PDF attachment (browser storage limits apply)
- Search, category filters, upcoming dates and home dashboard
- Export/import local JSON backup
- Settings, demo local PIN, privacy notes and sample premium pricing
- Offline use after the web app files are available on the device

## Important limitations — read before real users
- No real user accounts, email verification, password reset or server-side account recovery.
- The demo PIN is a convenience gate only; it does NOT encrypt records/files or replace Android Keystore/biometrics.
- Data is stored in browser localStorage, which can be cleared by the browser/OS and is not suitable for highly sensitive documents.
- Reminder dates are shown in-app; reliable background notifications require native Android implementation and device testing.
- Receipt OCR, automatic detail extraction, encrypted cloud backup, family sharing, real subscription billing and ad network are not connected.
- Subscription prices are examples for testing, not active products or guaranteed revenue.
- Do not use this prototype to store passwords, payment-card data, or sensitive identity documents.

## Run locally
Open `www/index.html` in a modern browser. Some mobile browsers restrict local file features; serve it locally or wrap it with Capacitor for more reliable app behavior.

## Next engineering stages
1. Build and test Android wrapper on a clean build environment.
2. Implement encrypted file storage and Android Keystore-based lock.
3. Add reliable local notifications and file-provider handling.
4. Add tested backup/recovery flow with user-held recovery key; cloud recovery requires a backend.
5. Add consent, privacy policy, data deletion, export, subscription billing and store compliance.
6. Security review and real-device QA before collecting real user documents or payments.
