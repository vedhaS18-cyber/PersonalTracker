# Privacy and data handling

This page describes **Personal Tracker v1.5.0**, which appears on your phone as
**Expense Tracker**. It covers the Android app distributed through this repository.
It does not describe the separate practices of GitHub, your bank, Gmail or a cloud
storage provider.

## Payment notifications

Automatic capture is optional. You grant Android notification access and choose
which apps to capture from. Your default SMS app is preselected during first setup;
you can also select Gmail and other supported sources. Notifications from
unselected apps are discarded. The app does **not** read your SMS or email inbox,
connect to your bank account or request your bank login.

Saved payment information can include the amount, payee, payment method, bank name,
date and time, your purpose label, source app and review status. These records are
personal financial information. Full notification bodies and raw account or card
numbers are not retained. Hashed identifiers help avoid duplicate records.

Recognised payments briefly enter a private queue on your phone before saving.
This contains parsed payment fields and hashed identifiers, not complete messages
or emails. Saved or intentionally skipped entries leave the queue. Interrupted
saves are retried while the app runs and when you next open it.

Capture status keeps limited recent diagnostic results and connection events, plus
the last successful save time and duration. It does not include notification
bodies, titles, email addresses or amounts. These diagnostics stay on your phone
and are not uploaded.

## Storage and permissions

- The app has no account system, app server, advertising or app analytics SDK.
- It does not request location permission or attach a location to payments.
- Notification permission lets it show purpose prompts and reminders. Enabled
  reminders are rescheduled after a restart or a time change.
- Camera, photo selection and backup folders use Android's permission and file
  selection flows.
- Payment databases and managed receipts are stored in the app's private storage.
- Automatic Android cloud backup and device transfer of app storage are disabled.
- There is no additional app-specific database encryption, PIN or biometric lock.
  Protect your phone with its own screen lock.

On Android 13 and later, the app disables its preview screenshot in the recent-apps
screen. You can still take ordinary screenshots. Notification actions that change
records require the phone to be unlocked.

## Receipt scanning

**Scan receipt** uses Google's ML Kit document scanner through Google Play services.
A notice appears before first use. Google states that scanning and image processing
happen on the device and that input images and resulting scans are not sent to its
servers. Google Play services may download scanner components, receive updates and
send scanner performance and usage metrics to Google. See
[Google's ML Kit privacy information](https://developers.google.com/ml-kit/terms).

The scanner dependency adds Internet and network-state permissions. The app does
not upload payment records or receipt images to an app server. **Camera without
cropping** and direct **Gallery** attachment remain available without opening the
scanner.

You can scan up to 10 pages in one session or crop existing gallery photos inside
the scanner. **Original** is the default for a new bill. **Filters** optionally
enables on-device readability filters; the selection stays with that draft. The
app does not enable automatic stain or shadow cleaning.

Only the processed pages you accept are copied into private draft storage and
then saved with the bill. Unprocessed originals are not separately retained by the
app. Your original gallery files are independent of these copies. If some pages
fail to import, successful pages remain and the app reports the failed pages.

Unsaved scans and camera photos are kept outside Android's disposable cache.
Temporary draft copies are removed after saving, removing a photo or discarding
the form. If the app is abruptly terminated, inactive draft photos become eligible
for cleanup after 30 days when a bill form is next opened. Photos in active forms
are protected, and restored forms renew their retention window. Saved bill
receipts do not expire. Diagnostic errors describe the operation, failure type and
photo number, not receipt content or file locations.

## Backups, exports and sharing

Spending and Claims are separate. A Claims backup does not include Spending.
Claims backups go to a folder you choose. Spending has its own JSON backup and
restore option; its backups contain payment details and purposes and are **not
password-encrypted by the app**. Restoring Spending merges validated records and
does not restore notification permissions.

Generated documents can be shared through Android. A cloud folder, document
provider or recipient you select may transmit or store these files independently.
Backups and exported documents can be read by anyone who gains access to them.

Uninstalling the app or clearing its storage removes local records and managed
receipts. Back up both Spending and Claims before doing this. External backups and
exports are separate copies; uninstalling the app does not delete them.

## Deletion and retention

Payment records remain until you delete them or remove app storage. **Delete
payment** removes the record but retains minimal hashed identifiers to prevent the
same notification from recreating it.

**Delete all spending data** clears local payment history, pending captures up to
the deletion time, deletion identifiers and capture diagnostics. It retains a
capture cutoff and your notification choices so older alerts do not repopulate
your history. Claims are unaffected. The limit of 50,000 payments stops new
inserts; it does not automatically delete older history.

Delete external backups and exports separately through the app or provider holding
them. Copies you have already shared cannot be recalled by Personal Tracker.

## Questions and reports

For ordinary questions, use the
[public issue tracker](https://github.com/vedhaS18-cyber/PersonalTracker/issues).
Anything posted there is public. Do not post real financial records, notification
screenshots, receipts, account numbers or other personal information. Use invented
examples or carefully redacted details.

For a security concern involving private information, follow
[SECURITY.md](SECURITY.md) instead of opening a public issue. There is no dedicated
support email at present.
