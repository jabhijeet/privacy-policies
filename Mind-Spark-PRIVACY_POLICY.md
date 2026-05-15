# Privacy Policy for Mind Spark IQ Test

**Last Updated:** April 19, 2026

## 1. Introduction

Mind Spark IQ Test ("we", "our", or "the App") respects your privacy. This policy
explains what the App collects, where that data goes, and the choices you have.

By using the App you consent to the practices described here. If you do not
agree, do not use the App.

## 2. Age Requirement

**The App is intended for users aged 5 and above.** If a user is under 5, they
may not use the App. Parents or guardians are responsible for supervising use by
children in the 5–12 age band, including the decision to share age for
age-appropriate item generation.

## 3. Information We Collect

### 3.1 Information you enter
- **Age (required)** – used solely to tune the difficulty and reading level of
  generated questions. Stored locally on the device.
- **Name (optional)** – used only for greeting; never transmitted off-device.
- **Country (optional)** – used to bias item cultural neutrality.
- **Language, purpose, question-count preferences** – local preferences.

### 3.2 Quiz data
- The questions generated for a session, your answers, elapsed time, computed
  scores, and the session history. All kept **on-device** in local preferences
  and platform secure storage.

### 3.3 Approximate location via IP (optional)
- On launch the App makes a **single HTTPS request to `https://ipapi.co/json/`**
  to pre-fill the country field from your IP address. The response is not stored
  beyond the current session. You can edit or clear the country field at any
  time. This call can be avoided by simply editing the country manually — the
  App does not require geolocation.

### 3.4 Voice features
- If you enable voice input/output, speech recognition and TTS run through the
  platform's on-device speech APIs where available. Audio is not uploaded by
  the App. Platform providers (Apple / Google) may process speech under their
  own policies.

### 3.5 What we do NOT collect
- No account, login, or user ID.
- No tracking or advertising identifiers.
- No analytics or crash-reporting SDK ships with the App.
- No race, ethnicity, gender, medical, financial, or biometric data.

## 4. Where Data Goes

### 4.1 On-device only (default)
Everything above is stored locally. API keys you enter are kept in the
platform secure keystore (iOS Keychain / Android EncryptedSharedPreferences /
Windows DPAPI / macOS Keychain / Linux libsecret).

### 4.2 LLM provider you choose (opt-in, required for generation)
To generate a quiz the App sends a **single request** to the Large Language
Model (LLM) provider you configure (OpenAI, OpenRouter, Anthropic, Google
Gemini, HuggingFace, Ollama, or a custom endpoint). That request contains:

- The generation prompt (system + user message).
- **Your age** – included to calibrate difficulty for the age group.
- **Your country** – included only if you provided one, used as a
  cultural-neutrality hint.
- A random session seed and theme palette.
- The requested number of items and difficulty.

The request does **NOT** contain your name, IP address (beyond what the
network layer inherently reveals to the provider), answers, scores, or history.

Your answers, scores, and results are evaluated entirely **on-device** and are
never sent to an LLM or to any server operated by us.

Each provider has its own privacy policy and data-retention practices. Review
them before configuring the provider:

- OpenAI: https://openai.com/policies/privacy-policy
- OpenRouter: https://openrouter.ai/privacy
- Anthropic: https://www.anthropic.com/legal/privacy
- Google Gemini (AI Studio): https://policies.google.com/privacy
- HuggingFace: https://huggingface.co/privacy
- Ollama (local): runs on your own machine; no third-party transfer.

If you do not want any data to leave your device, configure an Ollama endpoint
running on your own machine.

### 4.3 Email (opt-in per send)
If you tap "Email Results" the App hands the result body to your device's
default email client via the system compose sheet. We do not operate an email
relay and cannot see the address you send to.

## 5. Security

- API keys are held in the OS secure keystore (Keychain / Keystore / DPAPI),
  not in plain preferences.
- Network requests use HTTPS.
- Response size from the LLM provider is bounded to 2 MB and timed out at 60 s
  (120 s when streaming).

No system is absolutely secure; we use reasonable industry practice for a
client-only app.

## 6. Your Choices and Rights

- **Uninstall**: removes every piece of data the App has stored about you.
- **Clear data** (Android Settings → Apps → Mind Spark → Storage → Clear Data):
  deletes preferences, history, and stored API keys.
- **Delete a provider config**: Settings → LLM Provider → clear fields.
- **Skip country lookup**: edit the Country field before starting a quiz.
- **Opt out of LLM use**: do not configure a provider; the App will prompt you
  and decline to start a quiz rather than fall back to any off-device service.

Depending on where you live (e.g., EU/UK GDPR, California CCPA), you may have
additional rights (access, correction, erasure, portability, objection).
Because the App is client-only and we do not receive your data, honoring these
rights typically means using the on-device controls above. For anything we
cannot resolve on-device, contact us (Section 9).

## 7. Children

We collect age because the App needs it to generate age-appropriate items.
For users identified as under 13, we strongly recommend that a parent or
guardian configure the LLM provider and supervise use. Because no data leaves
the device to us (all learning data stays local; the LLM request includes only
age and country), we believe this model minimizes risk for child users.

If you are a parent or guardian and you want a child's data removed, uninstall
the App or use the system Clear Data option — that is the complete and
authoritative deletion path.

## 8. Changes to This Policy

We may update this policy. Meaningful changes will update the "Last Updated"
date and, where appropriate, be surfaced inside the App on next launch.

## 9. Contact

**Contact:** Please refer to the developer contact details provided in the application's Google Play Store listing.
