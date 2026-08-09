# Privacy Policy for Smart Task Manager

**Last Updated:** August 9, 2026

## Introduction

Smart Task Manager ("we", "our", or "the Extension") is committed to protecting your privacy. This Privacy Policy explains how we collect, use, and safeguard your information when you use our Chrome browser extension.

## Information We Collect

### 1. Information You Provide Directly

- **Task Data:** Task titles, descriptions, dates, times, priorities, statuses, and any images you attach to tasks.
- **Note Data:** Note titles and body text, folders, tags, reminders, and the notes' creation and edit times. Note bodies are free text, so they contain whatever you choose to write in them.
- **Saved Web Content:** When you explicitly save something to Notes, the extension stores the text you selected — or the readable text of the page when nothing is selected — together with the page title and address. This happens only when you ask for it (see [Saving a Page to Notes](#saving-a-page-to-notes)).
- **User Preferences:** Theme settings, notification preferences, and display options.
- **Account Information:** If you choose to sign in with Google, we receive your name, email address, and profile picture from Google.

### 2. Information Collected Automatically

- **Local Storage Data:** We store your tasks and settings locally in your browser using Chrome's storage API. Notes and note folders are stored on your device in your browser's IndexedDB database, because a saved article can be far larger than the `chrome.storage` quota allows.
- **Sync Data:** If you enable cloud sync, your tasks, notes, note folders and settings are synchronized to Google Firebase/Firestore under your authenticated account. A note you saved from a web page syncs along with its saved text, page title and address.

### 3. Information We Do NOT Collect

- We do **not** collect browsing history
- We do **not** read, monitor, or transmit the content of the pages you browse.
  A page is read **only** at the moment you explicitly save it, or a selection
  from it, to Notes — and what is read is saved to your own notes and sent
  nowhere else (see [Saving a Page to Notes](#saving-a-page-to-notes)).
  Displaying a reminder on the page you are viewing reads nothing at all
  (see [Showing Reminders on the Page You Are Viewing](#showing-reminders-on-the-page-you-are-viewing))
- We do **not** record or store audio. Voice input is transcribed by Chrome and only the
  resulting text reaches the extension (see [Voice Input](#voice-input-optional))
- We do **not** collect passwords or financial information
- We do **not** use analytics or tracking services
- We do **not** sell or share your data with third parties for advertising
- We do **not** operate any server of our own. Apart from optional Google sign-in
  and sync, and image searches you explicitly perform, the extension makes no
  network requests

## How We Use Your Information

We use the collected information solely for:

1. **Providing Core Functionality:** Storing and displaying your tasks, notes, settings, and preferences.
2. **Cloud Synchronization:** If enabled, syncing your data across devices using your Google account.
3. **Notifications:** Sending task and note reminders based on your notification settings.
4. **Image Search:** When you search for task images, queries are sent to the image provider you configure (Pexels, Pixabay, or Unsplash) using your own API key.
5. **AI Task Creation:** If you enable it and supply your own Google AI API key, the sentence you type is sent to Google to be turned into a task. Only that sentence — never your task list. See [AI Task Creation](#ai-task-creation-optional).

## Data Storage and Security

### Local Storage
- Tasks, settings and preferences are stored locally in your browser using Chrome's `chrome.storage.local` API.
- Notes and note folders are stored locally in your browser's IndexedDB database.
- Data remains on your device and is not transmitted unless you enable cloud sync.

### Cloud Storage (Optional)
- If you sign in with Google and enable sync, your data is stored in Google Firebase/Firestore.
- Data is encrypted in transit using HTTPS/TLS.
- Access is restricted to your authenticated Google account only.
- Firebase security rules ensure only you can read/write your own data.

### Data Retention
- Local data persists until you clear it manually or uninstall the extension.
- Deleting a note moves it to a Trash you can restore from. Notes in the Trash
  are permanently deleted automatically **30 days** after you delete them, or
  immediately if you choose "Delete forever" or "Empty trash".
- Cloud data persists until you delete it or delete your synced data through the extension settings. Deleting a note permanently on one device removes it from your other synced devices.

## Third-Party Services

### Google Sign-In & Firebase
When you use Google Sign-In and cloud sync:
- We use Google Identity Services for authentication
- We use Google Firebase/Firestore for cloud storage
- Google's Privacy Policy applies: https://policies.google.com/privacy

### Google Gemini (AI Task Creation)
Only if you enable AI task creation and supply your own API key. The sentence
you type is sent to Google's Gemini API from your browser; we never see it.
Google's Privacy Policy applies: https://policies.google.com/privacy

### Image Search Providers
When you search for images, your search queries are sent to:
- **Pexels** (if configured): https://www.pexels.com/privacy-policy/
- **Pixabay** (if configured): https://pixabay.com/service/privacy/
- **Unsplash** (if configured): https://unsplash.com/privacy

You must provide your own API key for these services.

## Voice Input (optional)

You can dictate a task instead of typing it, using the microphone button beside
Quick Add.

**The transcript is never submitted for you.** It appears in the text field so
you can read and correct it first, and you then choose whether to add it with
the ordinary "+" or draft it with AI. Speech recognition mishears, and a task
created from a misheard sentence is one you would only discover when the
reminder fired.

**Your voice is sent to Google.** Transcription uses Chrome's built-in speech
recognition, which streams the audio to Google's speech service to be turned
into text. That is the browser doing it, not this extension — but it is your
voice leaving your device, so it is stated here plainly rather than buried.

**This extension does not record, store or transmit audio itself.** It receives
only the text Chrome hands back. Nothing is kept.

**The microphone permission.** Chrome grants microphone access to a whole
extension, not to one of its screens, and a side panel cannot reliably display
that prompt. The first time you use voice input, a tab opens asking for
permission; once granted it applies to the extension and is not asked again.
You can withdraw it at any time from `chrome://settings/content/microphone`.

**If you never press the microphone button, no audio is captured at all.**

## AI Task Creation (optional)

You can optionally have a sentence turned into a task by Google's Gemini API —
typing "remind me about the GTS call at 5pm" and getting back a task titled
"GTS call", timed and with a reminder set.

This is **off by default** and requires you to supply your own Google AI API
key in **Settings → AI Task Creation**. Without a key the feature does not
appear.

**What is sent, and when.** Only the single sentence you typed, and only at the
moment you press the AI button next to Quick Add. Pressing the ordinary "+"
never sends anything: that path uses a parser that runs entirely on your
device. If the AI asks a clarifying question, your answer to that question is
sent as well.

**What is never sent.** Your task list, your other tasks, your profile, your
settings, and anything from any web page. The extension sends one sentence per
request and nothing else.

**Who receives it.** Google, under the API key you supplied, governed by the
terms of the Google AI service you obtained that key from and by
[Google's Privacy Policy](https://policies.google.com/privacy). We do not
receive, store, or see the text — the request goes from your browser directly
to Google. We operate no server in this path.

**Cost and quota** are between you and Google, against your own key.

**Turning it off.** Switch off "Enable AI drafting" in Settings, or clear the
API key. The button disappears and no request can be made.

## Saving a Page to Notes

You can save the page you are reading — or just the text you have selected on it
— as a note. This is available from the right-click menu ("Save selection to
Notes" / "Save page to Notes") and from a keyboard shortcut.

**It reads the page only when you ask.** Nothing is read in the background, and
nothing is read from tabs you have not acted on. The extension uses Chrome's
`activeTab` permission, which Chrome grants for a single tab, in response to
your action, and which expires. This is deliberately narrower than broad website
access: the extension does **not** request the `tabs` permission, and cannot
reach a page you did not explicitly save from.

**What is saved.** The text you selected, or the page's readable text if you
selected nothing; the page title; the page address; and the time you saved it.
All of it goes into your note, on your device.

**What is not saved.** Passwords, form contents, cookies, and anything on any
page you did not explicitly capture.

**Where it goes.** Into your notes. If you have enabled cloud sync it
synchronises to your own Firestore account like any other note. It is never sent
to us, and we operate no server in this path.

**The note is yours to edit or delete** like any other, including the saved text
and the link back to the original.

## Showing Reminders on the Page You Are Viewing

The extension can show a reminder as a small overlay on the web page you are
currently reading, instead of only as a Chrome notification. This is **off by
default**.

**What this requires.** Displaying anything on a page requires Chrome's
permission to access that page. That permission is *optional*: it is **not
requested when you install the extension**, and the extension does not have it
unless you turn the feature on in **Settings → Reminder Assistant** and accept
Chrome's prompt.

**What it does.** When a reminder is due, and only at that moment, the extension
places its own overlay onto the active tab. The overlay is isolated from the
page in a closed shadow root, so the page cannot see it and it does not alter
the page.

**What it does not do.** The overlay does not read the page. It does not access
page text, form fields, cookies, credentials, or anything you type. Nothing from
the page is stored or transmitted anywhere.

**The one thing we read.** Before showing a reminder, the extension checks the
address of the active tab to determine whether Chrome permits an overlay there
at all — Chrome forbids it on `chrome://` pages and the Chrome Web Store, for
example. This check happens inside the extension, the address is not stored, and
it is never transmitted.

**Turning it off.** Switch the feature off in Settings, or revoke access at any
time from `chrome://extensions` → Smart Task Manager → Details → Site access.
Reminders continue to work as Chrome notifications.

## Spoken Reminders

If you enable the voice option, reminder text is passed to your browser's
built-in speech engine (the standard Web Speech API) to be read aloud. The
extension does not record audio, does not use a microphone, and sends nothing to
us. Which voices are available, and whether any of them are processed by your
browser or operating system vendor, is determined by your browser and platform,
not by this extension.

## Diagnostics

**Settings → Diagnostics** contains a switch that writes extra detail about
reminder delivery to your browser's developer console, to help diagnose a
reminder that did not appear. It is off by default, the output stays on your
device, and nothing is transmitted or stored by us.

## Permissions Explained

### Permissions requested at install

| Permission | Purpose |
|------------|---------|
| `storage` | Store your tasks, settings, and preferences on your device |
| `unlimitedStorage` | Allow your notes to exceed Chrome's default storage quota. A saved article can be large, and without this the browser may discard your notes under disk pressure. It grants access to nothing |
| `identity` | Google Sign-In, only if you choose to enable cloud sync |
| `notifications` | Show reminder notifications |
| `alarms` | Schedule reminders so they fire even when the panel is closed |
| `sidePanel` | Show the extension in Chrome's side panel |
| `contextMenus` | Add "Save selection to Notes" and "Save page to Notes" to the right-click menu |
| `activeTab` | Read the current tab's selected text, title and address so it can be saved as a note — only when you invoke the save. Chrome grants this for one tab, in response to your action, and it permits no background access to any site |
| `scripting` | Two uses, both in the tab you are looking at and both started by you: reading the page you are saving to Notes (under `activeTab`), and placing a reminder overlay on a page (under the separate, optional permission below). It grants no access to any site on its own |

### Website access requested at install

| Sites | Purpose |
|-------|---------|
| `api.pexels.com`, `images.pexels.com`, `pixabay.com`, `api.unsplash.com`, `images.unsplash.com` | Used only when you search for a task image, and only with an API key you supply yourself |

### Website access that is optional and off by default

| Sites | Purpose |
|-------|---------|
| `http://*/*`, `https://*/*` | Displaying reminders on the page you are viewing. **Not requested at install.** Requested only if you enable the feature in Settings, and revocable at any time from `chrome://extensions`. See [Showing Reminders on the Page You Are Viewing](#showing-reminders-on-the-page-you-are-viewing) for exactly what this does and does not allow. |

The extension does **not** request the `tabs` permission. Where it needs to read
the tab you are looking at — only to save it to a note, and only when you ask —
it uses `activeTab`, which is granted per action rather than standing.

## Your Rights and Choices

You have the right to:

1. **Access Your Data:** View all your tasks and notes within the extension.
2. **Export Your Data:** Use the Settings → Export feature to download your tasks as JSON. *Note export is not yet available;* notes can be copied from the editor, and remain in your own Firestore account if you have enabled cloud sync.
3. **Delete Your Data:**
   - Delete individual notes — to the Trash, and then permanently
   - Clear everything on this device via Settings → Clear All Data, which deletes both tasks and notes
   - Remove cloud data by deleting your synced data or signing out
4. **Disable Sync:** Use the extension without signing in (local-only mode).
5. **Withdraw Page Access:** Turn off the on-page reminder overlay in Settings, or
   revoke website access from `chrome://extensions` → Smart Task Manager →
   Details → Site access. Reminders continue to work as Chrome notifications.
6. **Uninstall:** Removing the extension deletes all local data, including notes.

## Data Sharing

We do **not** share, sell, rent, or trade your personal information with third parties.

Your data may be processed by:
- **Google Firebase:** Only if you enable cloud sync (covered by Google's privacy policy)
- **Image Providers:** Only the search queries you explicitly submit

## Children's Privacy

This extension is not intended for children under 13. We do not knowingly collect information from children under 13.

## Changes to This Privacy Policy

We may update this Privacy Policy from time to time. We will notify you of any changes by updating the "Last Updated" date at the top of this document.

## Chrome Web Store Compliance

This extension complies with the [Chrome Web Store Developer Program Policies](https://developer.chrome.com/docs/webstore/program-policies/). Specifically:

- We request only permissions necessary for the extension's core functionality.
- Broad website access is **optional**, is not requested at install, is used solely to
  display reminders you have explicitly enabled, and can be revoked at any time without
  losing reminder functionality.
- We do not use user data for purposes unrelated to the extension's single stated purpose.
- We do not sell user data to third parties.
- We do not use or transfer user data for determining creditworthiness or lending purposes.

## Contact Us

If you have questions about this Privacy Policy or our data practices, please contact us at:

- **Email:** pream.webapps@gmail.com

---

By using Smart Task Manager, you agree to this Privacy Policy.
