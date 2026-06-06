# GymRhythm Privacy Policy

**Effective date:** 2026-06-05

## 1. Introduction

Hi, and thanks for using GymRhythm. This Privacy Policy explains what data we collect when you use the GymRhythm iOS app and any related services (we'll just call all of it "GymRhythm" or "the app" from here on), why we collect it, who we share it with, and what rights you have over it.

We've tried to keep this readable. If anything is unclear, email us at riccardo.mewis@gmail.com and we'll explain.

## 2. Data Controller

GymRhythm is built and operated by an individual sole developer:

- **Name:** Nikolas Mewis
- **Location:** Munich, Germany
- **Contact:** riccardo.mewis@gmail.com

For the purposes of the EU General Data Protection Regulation (GDPR), Nikolas Mewis is the "data controller" for your personal data. For users in California, the equivalent term is "business."

## 3. What information we collect

We try to collect as little as possible. Here's what we do collect, grouped by category.

### Account and identity

When you create an account, we need a way to recognize you next time you open the app. We use Firebase Authentication for this, and you can sign in with an email and password, Google, or Apple. If you sign in with Apple, we also store a one-time authorization code in your device's Keychain so we can fully revoke the Apple sign-in if you ever delete your account.

- Email address
- Firebase Authentication user ID (a random string used as your account key)
- Sign-in provider (email, Google, or Apple)
- Display name (the name you choose to show in the app; may come from your Apple or Google sign-in if you use those providers)
- Apple authorization code (only if you sign in with Apple, stored locally in the iOS Keychain)

### Profile and fitness data

These are the things you tell us about yourself during onboarding or later in your profile. They power your personalized stats, your weekly goal, and your progress over time. You can change or clear most of this from the Profile screen.

- Name
- Weight (in kg and lbs)
- Height (in cm and inches)
- Birthdate and age
- Gender
- Weekly workout goal
- Whether you describe yourself as a beginner, returner, or experienced lifter, and whether your goal is to lose weight, build muscle, stay consistent, etc., so we can pick the right onboarding copy and in-app messaging for you
- Where you heard about GymRhythm
- Whether you've used other fitness apps before
- Weight and height history snapshots (so you can see changes over time)

Most profile fields beyond name and basic sign-in details are **optional** — see Section 5a for what's required vs. optional.

### Location data

GymRhythm's main differentiator is automatic workout detection: when you walk into your gym, we want the app to notice and log it for you. To do that, we let you save one or more gym locations and we use a small **geofence** around each one. We do not record a trail of where you go.

- Saved gym name, address, and coordinates
- The radius you've chosen for each gym's geofence (default 100m)
- Your current iOS location permission status (so we can show the right setup prompts)
- Your current location, used **in memory only**, to check whether you've entered or left a gym geofence; we don't write this to disk and we don't upload it

We only ask for "Always" location access **after** you've decided to use the auto-detection feature, and you can change this any time in iOS Settings. If you deny location access, the app still works — you'll just need to log workouts manually.

### Workout activity

Every time you complete a workout (whether automatically or manually), we save a record of it so you can see your history and streaks.

- Session start time, end time, and duration
- XP earned for the session
- Which saved gym the workout was attributed to
- Session status (completed, skipped, etc.) and source (auto-detected, manual, or routine)
- Your routine schedule rules (which days and times you plan to train) and any time-bound exceptions
- XP and level progression, and daily XP claim records (used to prevent farming exploits)
- Daily consistency snapshots used to compute streaks and habit metrics

### Subscription and purchase data

If you subscribe to GymRhythm Premium, we work with RevenueCat to validate your subscription with Apple and remember your entitlement across devices.

- Whether you currently have a Premium subscription
- Your RevenueCat customer info: subscription status, renewal/expiry dates, transaction history, and your Firebase Auth user ID used as the RevenueCat customer ID

Apple processes the actual payment. We never see your card details.

### App usage and diagnostics (only if you opt in)

These two categories are **off by default**. You'll see a consent question during onboarding, and you can change your answer any time in Settings.

If you turn on **Product analytics**, we collect:

- Screens you view, and roughly how long you spend on each
- Button taps and key in-app events (for example, completing a workout)
- User properties like your level, premium status, weekly goal, age group, gender, goal type, and acquisition source — used for cohort segmentation, not advertising

If you turn on **Crash reporting**, we collect:

- Stack traces from crashes and non-fatal errors
- "Breadcrumbs" — a short log of which screens you visited before the crash
- App version and device model
- Custom crash keys that mirror the user properties above (level, premium status, weekly goal, age group, gender, goal type, acquisition source) so we can correlate crashes with cohorts. Because these keys are attached to your account, Crash Data is **linked to you** when crash reporting is enabled.

Both are gated by your consent toggle and stop collecting the moment you turn them off.

**Anonymous onboarding metrics.** When you first set up GymRhythm, we collect anonymous funnel events — which onboarding step you're on, how long you spent on it, and which category you selected (e.g., "tiktok" as a source, "general fitness" as a goal). These events are NOT linked to any user account or identifier — they're stripped of your user ID, email, name, weight, height, and birth date. They exist only to help us understand where the onboarding flow loses people so we can fix it. You can opt out anytime via Profile → Data & Privacy → Anonymous onboarding metrics.

### Your feedback

If you submit a suggestion through the in-app Feedback screen, we store it so we can read it and act on it.

- Suggestion title and description (whatever you typed)
- Category you picked
- A link back to your account so you can edit or delete it later

You can delete your own suggestions from the Feedback screen.

### Notification preferences

So we send you the right amount of nudges and not more.

- Notification level (essential, balanced, or all-in)
- A couple of onboarding progress flags (whether you've finished onboarding, and whether you've reached the login screen) so we know which screens to show you next
- Your analytics and crash-reporting consent choices and whether you've answered the consent question yet

## 4. How we use your information

We use your data for the following purposes:

- **Provide the workout tracking service** — let you log workouts, view your history, and use the core features of the app.
- **Save your progress across devices** — sync your workouts and settings so you can pick up where you left off.
- **Count your workouts toward streaks** — track consistency, streaks, and progress over time.
- **Geofence your gym for automatic check-ins** — detect when you arrive at your gym so the app can start a workout for you automatically.
- **Process your subscription** — manage your paid subscription, including renewals and refunds via Apple and our payment processor.
- **Fix bugs** — if you opt in, send us crash reports so we can diagnose and fix problems.
- **Understand product usage** — if you opt in, collect anonymous analytics so we can improve the app.

Analytics and crash reporting are **off by default**. You choose whether to enable them, and you can change your mind any time in Settings.

## 5. Legal basis under GDPR

If you're in the EU, the European Economic Area (EEA), or the UK, GDPR requires us to tell you the legal basis we rely on for each purpose. Here's the breakdown:

- **Performance of a contract (Art. 6(1)(b) GDPR)** — for the core app functionality you signed up for: account management, storing your workouts, location-based auto check-ins, and processing your subscription. Without this data, the app can't do its job.
- **Consent (Art. 6(1)(a) GDPR)** — for analytics and crash reporting. These are opt-in via Settings. You can withdraw your consent at any time, and we'll stop the collection going forward.
- **Legitimate interests (Art. 6(1)(f) GDPR)** — for security and abuse prevention, including rate limiting and Firebase App Check. Our legitimate interest is keeping the service reliable and protecting it (and you) from abuse. We've weighed this against your rights and believe it's proportionate.
- **Anonymous onboarding metrics: Legitimate interests (Art 6(1)(f))** — improving the app's onboarding flow. Because these events carry no identifier, there is no privacy impact requiring consent.

### 5a. Is providing this data required?

Article 13(2)(e) GDPR requires us to tell you whether providing your data is mandatory and what happens if you don't. Here's the plain-English version:

- **Required to create an account (contractual requirement):** an email address or a sign-in identifier from Apple or Google, plus the Firebase Authentication user ID we generate. Without these we can't create an account for you, and without an account the app's sync, history, and subscription features won't work.
- **Required only if you subscribe (contractual requirement):** the RevenueCat / Firebase user ID used to look up your Premium entitlement. Without it we can't process or restore your subscription.
- **Required only if you enable auto check-in (optional feature):** "Always" location permission plus at least one saved gym. If you deny location access or don't save a gym, auto check-in is unavailable but manual workout logging remains fully available.
- **Optional in all cases:** display name, full name, weight, height, birthdate, gender, weekly workout goal, identity stage (beginner / returner / experienced), goal type (e.g., lose weight, build muscle), where you heard about us, whether you've used other fitness apps, and weight/height history. If you leave these blank, the app still works — you'll just see less personalized stats, messaging, and onboarding.
- **Always opt-in:** product analytics and crash reporting. If you don't consent, we collect neither, and the app behaves the same way for you.

## 6. Third parties we share data with

We use a small number of third-party "sub-processors" to run the app. They process data on our behalf, under contract, for the purposes listed above.

### Authentication

| Provider | What they do for us | What data they receive | Privacy policy |
|---|---|---|---|
| Firebase Authentication (Google) | Creates and manages your account, handles sign-in and password recovery | Email, password hash, display name, authentication tokens | [policies.google.com/privacy](https://policies.google.com/privacy) |
| Google Sign-In SDK | Lets you sign in with your Google account | Google account email, ID token, access token (used only to exchange for a Firebase credential) | [policies.google.com/privacy](https://policies.google.com/privacy) |
| Sign in with Apple | Lets you sign in with your Apple account | An anonymized Apple user ID, an authorization code (stored locally in the Keychain for account-deletion revocation), and your email **only** if you choose to share it | [apple.com/privacy](https://www.apple.com/privacy) |

### Cloud storage

| Provider | What they do for us | What data they receive | Privacy policy |
|---|---|---|---|
| Cloud Firestore (Google) | Stores your account data in the cloud so it syncs across devices | All user data: profile (name, weight, height, birthdate, gender, goals), saved gym locations, workout sessions, routines, XP claims, metrics history, consistency history, feedback submissions, and your location-permission status | [policies.google.com/privacy](https://policies.google.com/privacy) |

### Product analytics (only if you opt in)

| Provider | What they do for us | What data they receive | Privacy policy |
|---|---|---|---|
| Firebase Analytics (Google) | Helps us understand which features get used so we can prioritize improvements | Screen views, custom events, user properties (level, premium status, weekly goal, gender, goal type, acquisition source, age group, streak) and session duration — **only when analytics consent is on** | [policies.google.com/privacy](https://policies.google.com/privacy) |

### Crash reporting (only if you opt in)

| Provider | What they do for us | What data they receive | Privacy policy |
|---|---|---|---|
| Firebase Crashlytics (Google) | Captures crashes and non-fatal errors so we can fix them | Stack traces, breadcrumbs, custom crash keys that mirror your user properties (level, premium status, weekly goal, age group, gender, goal type, acquisition source), app version, device model — **only when crash-reporting consent is on**. Because these keys are tied to your account, this data is linked to you. | [policies.google.com/privacy](https://policies.google.com/privacy) |

### App integrity

| Provider | What they do for us | What data they receive | Privacy policy |
|---|---|---|---|
| Firebase App Check (Google) | Confirms requests to our backend come from a genuine copy of the app, not a bot or tampered build | An attestation token (DeviceCheck on iOS 13, App Attest on iOS 14+, or a debug token in development) | [policies.google.com/privacy](https://policies.google.com/privacy) |

### Subscriptions

| Provider | What they do for us | What data they receive | Privacy policy |
|---|---|---|---|
| RevenueCat | Validates your Premium subscription with Apple, restores purchases on new devices, and tracks entitlements | Your Firebase Auth user ID (as the RevenueCat app user ID), subscription purchase data, entitlements, subscription dates, and transaction history | [revenuecat.com/privacy](https://www.revenuecat.com/privacy) |

### Maps

| Provider | What they do for us | What data they receive | Privacy policy |
|---|---|---|---|
| MapKit and Apple Maps | Powers gym search, geocoding, reverse geocoding, and the map display when you pick a gym | Your search queries (gym names), your current location, and coordinates for reverse geocoding | [apple.com/privacy](https://www.apple.com/privacy) |

We do **not** sell your personal information, and we do not share it with advertisers.

## 7. International data transfers

Some of our sub-processors (notably Firebase/Google, Apple, and RevenueCat) process data on servers located in the United States and other countries outside the EU/EEA.

Where data is transferred outside the EU/EEA, we rely on the European Commission's **Standard Contractual Clauses (SCCs)** and any additional safeguards our sub-processors have put in place (for example, Google's and Apple's published Data Processing Addenda). If you'd like more detail on a specific transfer, email us.

## 8. How long we keep your data

- We keep your account data for as long as you have an account with us.
- When you delete your account (in-app: Settings -> Delete Account), your Firebase Authentication record and your Firestore data are **wiped immediately**.
- Any residual server logs (for example, crash logs or security logs) are purged within **30 days** of account deletion.

You don't need to email us to delete your data — the in-app button does it for you. But you can email us as a backup if anything goes wrong.

## 9. Your rights

### If you're in the EU/EEA or UK (GDPR)

You have the right to:

- **Access** the personal data we hold about you.
- **Rectify** inaccurate data.
- **Erase** your data ("right to be forgotten").
- **Port** your data to another service in a machine-readable format.
- **Restrict** processing in certain circumstances.
- **Object** to processing based on legitimate interests.
- **Withdraw consent** at any time (for analytics/crash reporting), without affecting the lawfulness of past processing.
- **Lodge a complaint** with a supervisory authority. Our lead authority is the **Bayerisches Landesamt für Datenschutzaufsicht (BayLDA)** in Germany, but you can complain to the supervisory authority in your country of residence.

### If you're in California (California Consumer Privacy Act / California Privacy Rights Act, "CCPA/CPRA")

You have the right to know what we collect, to delete it, to correct it, and to not be discriminated against for exercising these rights.

**We do not sell your personal information.** We do not "share" it for cross-context behavioral advertising. There is no "Do Not Sell or Share My Personal Information" link because there's nothing to opt out of.

### How to exercise your rights

- **Delete your account and data:** Settings -> Delete Account, inside the app.
- **Toggle analytics or crash reporting consent:** Settings, inside the app.
- **Disable anonymous onboarding metrics** via Profile → Data & Privacy.
- **Anything else (access, rectification, portability, questions):** email riccardo.mewis@gmail.com.

We'll respond within 30 days.

## 10. Security

We take reasonable steps to protect your data:

- Data in transit is encrypted using **TLS**.
- Data at rest is stored in **Firebase** (Google Cloud), which encrypts data at rest by default.
- Sensitive credentials (such as authentication tokens) are stored in the **iOS Keychain** on your device.
- Access to backend services is protected by **Firebase App Check** and standard authentication.

No system is 100% secure, and we won't pretend otherwise. If a breach affects your data, we'll notify you and the relevant authorities in line with our GDPR obligations.

## 11. Children

GymRhythm is **not directed at children under 13**. We do not knowingly collect personal data from children under 13. If you believe a child has provided us with personal data, please email riccardo.mewis@gmail.com and we'll delete it.

## 12. Cookies and tracking technologies

We keep this simple:

- We **don't use cookies** (GymRhythm is a native iOS app, not a website).
- We **don't use IDFA** (Apple's advertising identifier).
- We **don't do cross-app or cross-site tracking**.
- Because of the above, we don't show an **App Tracking Transparency** prompt — there's nothing to track across apps.

## 13. Automated decision-making and profiling

GymRhythm does **not** engage in automated decision-making, including profiling, that produces legal effects concerning you or similarly significantly affects you within the meaning of **Article 22 GDPR**.

The cohort segmentation described in Section 3 (used for product analytics if you have opted in, and mirrored into crash keys if you have opted in to crash reporting) is used only to inform product improvements and bug fixes. It does not determine pricing, entitlements, access to features, or any other outcome that produces legal or similarly significant effects on you.

## 14. Changes to this policy

We may update this policy from time to time. When we do, we'll update the "Effective date" at the top.

If the changes are **material** (for example, a new sub-processor, a new category of data, or a new purpose), we'll notify you in-app before the changes take effect.

## 15. Contact

Questions, requests, or complaints about this policy or your data?

Email: **riccardo.mewis@gmail.com**

We read everything and we'll get back to you.
