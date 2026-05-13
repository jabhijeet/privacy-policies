# Privacy Policy for BabySteps

**Last Updated: May 13, 2026**

At BabySteps, we are committed to protecting your privacy and ensuring you have complete ownership of your baby's data. This Privacy Policy explains our "Privacy-by-Design" architecture and how your data is handled.

## 1. Core Philosophy: You Own Your Data
BabySteps is a **Local-First** application. This means:
- All data you enter (logs, feeding times, growth metrics, photos) is stored directly on your mobile device.
- We do not host your data on our servers.
- There is no centralized database where we (the developers) can access your information.

## 2. Encryption and Security
We take security seriously. All sensitive data is protected using industry-standard measures:
- **Local Encryption**: Personal health and routine data are encrypted on your device using **AES-256 encryption** before being saved.
- **Secure Key Storage**: Encryption keys are stored in the platform's secure enclave (iOS Keychain / Android Keystore) and never leave your device.

## 3. Google Drive Synchronization
The application offers an optional synchronization feature using your own Google Drive account.
- **Consent**: Sync only happens if you explicitly sign in and grant permission.
- **Scope**: The app uses the `https://www.googleapis.com/auth/drive.file` scope. This means it can **only** access the specific files and folders it creates. It cannot see your other documents, photos, or data.
- **Direct Path**: Data is transferred directly between your device and Google's servers. It never passes through any servers owned by the developers of BabySteps.

## 4. No Third-Party Tracking
BabySteps is built without tracking:
- **No Analytics**: We do not use third-party analytics (like Google Analytics or Firebase Analytics) to track your behavior.
- **No Advertising**: We do not include any advertising SDKs or data-selling mechanisms.
- **No Telemetry**: No crash reports or usage data are sent to us unless you explicitly opt-in to a support request.

## 5. Partner Sharing
If you choose to share a baby's profile with a partner:
- The sharing is facilitated through Google Drive's native permission system.
- Access is granted only to the specific folder created by the app.

## 6. Data Deletion
Since you own the data:
- **Local Deletion**: Deleting a record in the app or uninstalling the app removes the data from your device.
- **Cloud Deletion**: You can permanently delete your backup data at any time by deleting the `BabySteps_Sync` folder from your Google Drive account.

## 7. Contact Us
If you have any questions about this Privacy Policy, please contact us at:
[Your Support Email Here]

---
*BabySteps - Privacy-First Newborn Tracking*
