<div align="center">
  <img src="resources/icon.png" alt="INBOX.EU Mail" width="160" />
  <h1>INBOX.EU Mail</h1>
  <p><strong>Desktop email for INBOX.EU and other secure IMAP/SMTP accounts.</strong></p>
  <p><sub>Windows · Apple Silicon macOS · Linux</sub></p>
</div>

INBOX.EU Mail brings your email accounts, attachments and unfinished messages into
one desktop workspace. Use a unified view or work with each mailbox separately,
with a local mail cache and direct connections to your email provider.

## Download

- **Windows 10/11 x64** — [Microsoft Store](https://apps.microsoft.com/detail/9MXZ1TBVHRK6).
- **macOS 13 Ventura or newer, Apple Silicon** — signed and Apple-notarized
  [DMG](https://github.com/INBOKSS/inboxeu-mail-releases/releases).
- **Linux x64** — [AppImage and DEB](https://github.com/INBOKSS/inboxeu-mail-releases/releases).
  AppImage requires FUSE 2; DEB is for compatible Debian/Ubuntu systems.

The links show the currently published versions. Microsoft Store and direct-download
The links show the currently published versions. Microsoft Store and direct-download
releases can become available at different times. Production packages offer
INBOX.EU and Other IMAP/SMTP accounts, with INBOX.EU selected by default. A compatible
account with secure IMAP/SMTP access is required. Signing in with a Google or
Microsoft account is not available in these releases; a Gmail mailbox can be
added as Other IMAP/SMTP with a Google app password.

## Works with your mail provider

INBOX.EU Mail is built for [INBOX.EU](https://www.inbox.eu), and it also works
with **any other provider that offers secure IMAP/SMTP access** — your
company's mail server, the mailbox that came with your web hosting, or another
email service (Gmail included, with a Google app password).

- **INBOX.EU** — enter your address and password; the server settings are
  already built in.
- **Other IMAP/SMTP** — enter your email address and choose **Find mail
  settings**. The app looks up the servers, ports, encryption and username
  for you, the same way Thunderbird does:
  1. your provider's own configuration (`autoconfig.<domain>` and
     `<domain>/.well-known/autoconfig`, HTTPS only);
  2. DNS SRV records for IMAP and mail submission ([RFC 6186](https://www.rfc-editor.org/rfc/rfc6186));
  3. Mozilla's Thunderbird ISPDB, the public database of mail providers;
  4. for a custom domain, the same lookups for the provider that hosts its
     mail (found through the domain's MX record).

  Only the domain is used for these lookups — never your full address or
  password. When settings are found, you only add your name and password;
  **Edit server settings** shows everything that was filled in. If nothing is
  found, or you prefer, **Enter settings manually** opens every field.

- **Secure by design** — connections use SSL/TLS or required STARTTLS only,
  never an unencrypted fallback. Certificates are checked against the built-in
  roots plus your operating system's certificate store, so company servers
  trusted on your computer work too. Both servers are tested before an
  account is saved, with plain-language explanations when something fails
  (wrong port, security mode, certificate or password).
- **Helpful about special cases** — Gmail and Google Workspace mailboxes get
  guidance for Google app passwords; Outlook.com and Microsoft 365 mailboxes
  are recognized and explained (Microsoft accepts only its own sign-in, which
  is not supported yet); Proton (needs the paid Bridge) and Tuta (no IMAP/SMTP)
  are explained instead of failing with an unclear error.
- **Change it later** — an Other IMAP/SMTP account's servers, ports, security
  and username can be edited in Settings and are verified again before saving.

## Highlights

- **Several accounts, one workspace** — INBOX.EU and other IMAP/SMTP accounts
  side by side, with a unified view across accounts and folders.
- **Keep conversations moving** — minimize several new messages, replies and
  forwards to a bottom dock while you browse; nothing is lost on quit.
- **Write with context** — rich text, tables, inline pictures, Word/Excel paste,
  spelling and a signature for each account.
- **Catch the small mistakes** — a forgotten-attachment reminder, a size check
  against your provider's limit and a seven-second Undo Send.
- **Find the file** — every attachment across your accounts in one Files view,
  with in-app previews for images, PDF, Word, Excel and text.
- **Know who really wrote** — the app checks DKIM, SPF and DMARC itself and
  loads remote images only from people you correspond with.
- **Private by default** — mail is cached on your device, credentials stay in
  the operating system's secure storage, and there is no analytics or tracking.

## Features

### Accounts

- INBOX.EU and Other IMAP/SMTP accounts, with automatic settings discovery
  ([above](#works-with-your-mail-provider)).
- Several accounts at once: a unified **All** view, or each account with its
  own folder tree. Provider badges identify every account at a glance.
- Choose which folders of each account appear in **All**.
- Email addresses are checked before connecting; custom domains and plus
  addresses are supported.
- Every account works independently: a slow or offline mailbox never delays
  reading mail in another one.
- A changed password is not retried over and over (which could lock your
  account): the app pauses that account and offers **Update password**.
- Settings > Data shows the storage each account uses; **Clear cache**
  downloads mail again and keeps your signature, login and settings.
- Removing an account also removes its local mail and preferences.

### Reading mail

- Three-pane layout with resizable columns, a collapsible folder sidebar and
  an expanded reading mode.
- Compact or comfortable rows and your choice of list order; the list never
  jumps under you while new mail arrives or you read and flag messages.
- Inbox rows show the sender; Sent and Drafts show the recipients.
- **Sender check** — DKIM, SPF and DMARC are verified on your device. Verified
  senders are marked; a forged sender gets a red shield and a warning.
- **Remote images only from people you know** — tracking images load by
  default only from people you have written to, and only when the message
  really comes from them. Spam and forged mail always hide them. You can show
  images for one message, or choose always/never in Settings.
- Calendar invitations show event details for every account; responding and
  the calendar link are available on INBOX.EU accounts.
- Attached emails (`.eml`) open in the app with their own attachments and can
  be answered or forwarded; Outlook's `winmail.dat` opens too.
- Right-click text to copy or search, links to open or copy, and images in a
  message to save or forward.
- **Print** with a preview, or save as PDF; **Download** a message as `.eml`;
  **View source** with every header.
- The message header scrolls away while the action toolbar stays pinned, so
  the message gets the most room.

### Organizing

- **Search** downloaded mail by words, `"exact phrases"` and `OR`, across
  subject, people and message text, in any language. Search one folder or
  **All**, combined with a label filter.
- **Labels** — mark messages Important on every account; INBOX.EU accounts
  add up to ten named, colored labels, usable as one-click filters.
- **Multi-select like a file manager** — Ctrl/Cmd-click, Shift-click,
  Shift+arrow keys, Page Up/Down, Home/End and Ctrl/Cmd+A. Mark, move or
  delete the selection, or drag it onto a folder.
- **Folders** — create, rename, empty and delete your own folders on INBOX.EU
  accounts; set the folder order for accounts on other servers. System folders
  stay protected and deleted mail goes to Trash first.
- Emptying a folder waits a few seconds with **Undo**; Shift+Delete deletes
  permanently after a confirmation.

### Writing

- Rich-text composer with fonts, lists, links, tables (pick the size from a
  grid, edit rows and columns, drag column widths) and inline pictures that
  stay small without visible quality loss.
- **Paste from Word and Excel** keeps formatting, lists, tables and supported
  pictures (native Excel picture recovery is Windows-only).
- **Several messages in progress** — minimize compositions to a bottom dock;
  each keeps its own sending account, text and attachments. Quitting saves
  unfinished messages to each account's Drafts.
- Drafts are saved to your mail server and open straight in the composer.
- **A signature per account**, with formatting, pictures and fonts pasted from
  Outlook or Word.
- **Spelling** with suggestions in the subject, body and signature editor;
  dictionaries for your languages download on request and then work offline.
- Recipient suggestions from the people you write to most.
- Attach files with the picker or by dragging them in. The estimated message
  size is checked against your provider's sending limit before you send.
- **Forgotten attachment check** — "attached", "pielikumā", "во вложении",
  "anbei" and similar words without a file ask before sending.
- **Undo Send** — every message waits seven seconds with Undo; **Send now**
  skips the wait.
- Forward keeps the original attachments; replies start with the cursor in the
  message.
- Typed smileys such as `:)` and `<3` become emoji; Ctrl+Z restores the text.
- Choose the default font size for new messages.

### Attachments and files

- **Files** — browse attachments from all your accounts, filter by type and
  group by sender, with a preview beside the message details.
- In-app previews for images (with a full-window gallery), PDF (with
  selectable text), Word and Excel overviews without Office installed, and
  text files. **Download all** saves every attachment at once.
- Print image and PDF attachments through a print dialog.
- **Electronic signatures** — signed PDFs and EDOC/ASiC containers show the
  signers, certificate and timestamp checks and qualified status. This is
  document inspection, not a signing service.

### On your desktop

- Desktop notifications for new mail; a sign-in code in the notification can
  be copied directly.
- **Default mail app** — email links in your browser and other apps open a new
  message here, with recipients and subject filled in.
- **New message** from the Windows taskbar jump list, the macOS Dock or the
  tray icon, even while the window is closed to the tray.
- Optional start at sign-in (Windows and macOS).
- Light and dark themes that follow your system, or the one you choose.
- Search and Settings in the title bar, leaving more room for mail.
- Window size, position and pane widths are remembered separately for each
  screen setup and switch over when you dock or undock.
- Full keyboard navigation with visible focus.

### Sync, privacy and security

- Live updates with IMAP IDLE plus light background checks; changes made in
  webmail or on your phone appear by themselves.
- Mail actions taken offline wait and are sent when the connection returns.
- Downloaded mail, search data and settings stay on your device; messages,
  drafts and actions synchronize with your provider. No analytics or
  third-party tracking.
- Passwords and tokens are kept in the operating system's secure storage.
- Remote images load through a guarded local loader that sends no cookies or
  mailbox credentials.
- Updates: the Microsoft Store updates the Windows app; other packages check
  for new versions and install a verified download from Settings > About.
- Updates keep your accounts, settings and mail cache in place.

## Screenshots

Explore 23 views of INBOX.EU Mail. Click any thumbnail to see it at full size.
These screenshots use an invented demo mailbox; signature results are illustrative.

<p align="center"><a href="screens/showcase-01-inbox-three-pane.png"><img src="screens/showcase-01-inbox-three-pane.png" width="900" alt="Your inbox, with room to read" /></a></p>

### Mail and layouts

|                                                                                                                                                                                                                                                 |                                                                                                                                                                                                                                     |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <a href="screens/showcase-02-compact-inbox.png"><img src="screens/showcase-02-compact-inbox.png" width="430" alt="Compact rows, with label filters in the sidebar" /></a><br /><sub>Compact rows, with label filters in the sidebar</sub>       | <a href="screens/showcase-03-expanded-reader.png"><img src="screens/showcase-03-expanded-reader.png" width="430" alt="Expand a message for focused reading" /></a><br /><sub>Expand a message for focused reading</sub>             |
| <a href="screens/showcase-04-collapsed-sidebar.png"><img src="screens/showcase-04-collapsed-sidebar.png" width="430" alt="Collapse the sidebar and resize your workspace" /></a><br /><sub>Collapse the sidebar and resize your workspace</sub> | <a href="screens/showcase-21-all-accounts-inbox.png"><img src="screens/showcase-21-all-accounts-inbox.png" width="430" alt="Browse mail across accounts and folders" /></a><br /><sub>Browse mail across accounts and folders</sub> |

### Everyday tools

|                                                                                                                                                                                                                                                       |                                                                                                                                                                                                                                                         |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <a href="screens/showcase-05-labels-and-colours.png"><img src="screens/showcase-05-labels-and-colours.png" width="430" alt="Organise mail with named, coloured labels" /></a><br /><sub>Organise mail with named, coloured labels</sub>               | <a href="screens/showcase-06-search-and-filters.png"><img src="screens/showcase-06-search-and-filters.png" width="430" alt="Search words and phrases, then narrow by label" /></a><br /><sub>Search words and phrases, then narrow by label</sub>       |
| <a href="screens/showcase-07-bulk-mail-actions.png"><img src="screens/showcase-07-bulk-mail-actions.png" width="430" alt="Select several messages and act together" /></a><br /><sub>Select several messages and act together</sub>                   | <a href="screens/showcase-08-rich-text-reply.png"><img src="screens/showcase-08-rich-text-reply.png" width="430" alt="Reply all with rich text and the original formatting" /></a><br /><sub>Reply all with rich text and the original formatting</sub> |
| <a href="screens/showcase-09-calendar-invitation.png"><img src="screens/showcase-09-calendar-invitation.png" width="430" alt="Read meeting details and respond to invitations" /></a><br /><sub>Read meeting details and respond to invitations</sub> | <a href="screens/showcase-22-account-signatures.png"><img src="screens/showcase-22-account-signatures.png" width="430" alt="Create a formatted signature for each account" /></a><br /><sub>Create a formatted signature for each account</sub>         |

### Attachments and Files

|                                                                                                                                                                                                                                                                                 |                                                                                                                                                                                                                                                                                           |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <a href="screens/showcase-10-message-attachments.png"><img src="screens/showcase-10-message-attachments.png" width="430" alt="Image thumbnails, document cards and Download all" /></a><br /><sub>Image thumbnails, document cards and Download all</sub>                       | <a href="screens/showcase-11-image-gallery.png"><img src="screens/showcase-11-image-gallery.png" width="430" alt="Open images in a full-window gallery" /></a><br /><sub>Open images in a full-window gallery</sub>                                                                       |
| <a href="screens/showcase-12-files-browser.png"><img src="screens/showcase-12-files-browser.png" width="430" alt="Browse attachments across your accounts" /></a><br /><sub>Browse attachments across your accounts</sub>                                                       | <a href="screens/showcase-13-files-filters-and-groups.png"><img src="screens/showcase-13-files-filters-and-groups.png" width="430" alt="Filter file types and group by sender" /></a><br /><sub>Filter file types and group by sender</sub>                                               |
| <a href="screens/showcase-14-files-image-preview.png"><img src="screens/showcase-14-files-image-preview.png" width="430" alt="Preview an image beside its message and file details" /></a><br /><sub>Preview an image beside its message and file details</sub>                 | <a href="screens/showcase-15-pdf-preview.png"><img src="screens/showcase-15-pdf-preview.png" width="430" alt="Read PDF attachments without leaving the app" /></a><br /><sub>Read PDF attachments without leaving the app</sub>                                                           |
| <a href="screens/showcase-16-office-document-preview.png"><img src="screens/showcase-16-office-document-preview.png" width="430" alt="Local Word and Excel overviews, without installed Office" /></a><br /><sub>Local Word and Excel overviews, without installed Office</sub> | <a href="screens/showcase-17-electronic-signature-details.png"><img src="screens/showcase-17-electronic-signature-details.png" width="430" alt="Inspect signers, certificate checks and qualified status" /></a><br /><sub>Inspect signers, certificate checks and qualified status</sub> |

### Appearance

|                                                                                                                                                                                                                                                                 |                                                                                                                                                                                                                                                   |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <a href="screens/showcase-18-appearance-preferences.png"><img src="screens/showcase-18-appearance-preferences.png" width="430" alt="Choose your theme, row density and list direction" /></a><br /><sub>Choose your theme, row density and list direction</sub> | <a href="screens/showcase-19-dark-inbox.png"><img src="screens/showcase-19-dark-inbox.png" width="430" alt="The same workspace in a dark theme" /></a><br /><sub>The same workspace in a dark theme</sub>                                         |
| <a href="screens/showcase-20-dark-files-preview.png"><img src="screens/showcase-20-dark-files-preview.png" width="430" alt="Dark Files browser with document preview" /></a><br /><sub>Dark Files browser with document preview</sub>                           | <a href="screens/showcase-23-dark-image-gallery.png"><img src="screens/showcase-23-dark-image-gallery.png" width="430" alt="View image attachments comfortably in the dark" /></a><br /><sub>View image attachments comfortably in the dark</sub> |

## Updates

Supported release builds check for newer published packages and offer
Settings > About > Check for updates. Store builds open Microsoft Store. Other
packages download and verify their matching installer: a Mac DMG opens for dragging
to Applications, a DEB opens in the package installer, and an AppImage replaces
itself and restarts. Windows updates are also managed by Microsoft Store.

This repository hosts public downloads, screenshots and the verified
`updates.json` catalog. It does not contain the source checkout or private
build credentials. Versions are advertised separately for each platform and
package format, only after publication checks.

## Privacy and support

Downloaded mail, search data and settings are cached on your device. Messages,
drafts and mail actions synchronize with your provider. Saved credentials use
operating-system secure storage; the client includes no analytics or third-party
tracking SDKs. External images in received mail can still contact their hosts.

- [Privacy Policy](https://help.inbox.eu/privacy-policy)
- [INBOX.EU Help](https://help.inbox.eu)
- [INBOX.EU](https://inbox.eu)
