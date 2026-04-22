# Privacy Policy for Smart Task Manager

**Last Updated:** April 15, 2026

## Introduction

Smart Task Manager ("we", "our", or "the Extension") is committed to protecting your privacy. This Privacy Policy explains how we collect, use, and safeguard your information when you use our Chrome browser extension.

## Information We Collect

### 1. Information You Provide Directly

- **Task Data:** Task titles, descriptions, dates, times, priorities, statuses, and any images you attach to tasks.
- **User Preferences:** Theme settings, notification preferences, and display options.
- **Account Information:** If you choose to sign in with Google, we receive your name, email address, and profile picture from Google.

### 2. Information Collected Automatically

- **Local Storage Data:** We store your tasks and settings locally in your browser using Chrome's storage API.
- **Sync Data:** If you enable cloud sync, your tasks and settings are synchronized to Google Firebase/Firestore under your authenticated account.

### 3. Information We Do NOT Collect

- We do **not** collect browsing history
- We do **not** collect website content
- We do **not** collect passwords or financial information
- We do **not** use analytics or tracking services
- We do **not** sell or share your data with third parties for advertising

## How We Use Your Information

We use the collected information solely for:

1. **Providing Core Functionality:** Storing and displaying your tasks, settings, and preferences.
2. **Cloud Synchronization:** If enabled, syncing your data across devices using your Google account.
3. **Notifications:** Sending task reminders and alerts based on your notification settings.
4. **Image Search:** When you search for task images, queries are sent to the image provider you configure (Pexels, Pixabay, or Unsplash) using your own API key.

## Data Storage and Security

### Local Storage
- All task data is stored locally in your browser using Chrome's `chrome.storage.local` API.
- Data remains on your device and is not transmitted unless you enable cloud sync.

### Cloud Storage (Optional)
- If you sign in with Google and enable sync, your data is stored in Google Firebase/Firestore.
- Data is encrypted in transit using HTTPS/TLS.
- Access is restricted to your authenticated Google account only.
- Firebase security rules ensure only you can read/write your own data.

### Data Retention
- Local data persists until you clear it manually or uninstall the extension.
- Cloud data persists until you delete it or delete your synced data through the extension settings.

## Third-Party Services

### Google Sign-In & Firebase
When you use Google Sign-In and cloud sync:
- We use Google Identity Services for authentication
- We use Google Firebase/Firestore for cloud storage
- Google's Privacy Policy applies: https://policies.google.com/privacy

### Image Search Providers
When you search for images, your search queries are sent to:
- **Pexels** (if configured): https://www.pexels.com/privacy-policy/
- **Pixabay** (if configured): https://pixabay.com/service/privacy/
- **Unsplash** (if configured): https://unsplash.com/privacy

You must provide your own API key for these services.

## Permissions Explained

Our extension requests the following Chrome permissions:

| Permission | Purpose |
|------------|---------|
| `storage` | Store tasks, settings, and preferences locally |
| `identity` | Enable Google Sign-In for cloud sync |
| `notifications` | Display task reminders and alerts |
| `alarms` | Schedule notification reminders |
| `sidePanel` | Display the task manager in Chrome's side panel |
| `tabs` | Open the welcome page on first install |

## Your Rights and Choices

You have the right to:

1. **Access Your Data:** View all your tasks and settings within the extension.
2. **Export Your Data:** Use the Settings → Export Tasks feature to download your data as JSON.
3. **Delete Your Data:** 
   - Clear local data via Settings → Clear All Tasks
   - Remove cloud data by deleting synced tasks or signing out
4. **Disable Sync:** Use the extension without signing in (local-only mode).
5. **Uninstall:** Removing the extension deletes all local data.

## Data Sharing

We do **not** share, sell, rent, or trade your personal information with third parties.

Your data may be processed by:
- **Google Firebase:** Only if you enable cloud sync (covered by Google's privacy policy)
- **Image Providers:** Only the search queries you explicitly submit

## Children's Privacy

This extension is not intended for children under 13. We do not knowingly collect information from children under 13.

## Changes to This Privacy Policy

We may update this Privacy Policy from time to time. We will notify you of any changes by updating the "Last Updated" date at the top of this document.

## Contact Us

If you have questions about this Privacy Policy or our data practices, please contact us at:

- **Email:** pream.webapps@gmail.com

---

By using Smart Task Manager, you agree to this Privacy Policy.
