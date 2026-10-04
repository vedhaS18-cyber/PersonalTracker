# Personal Tracker — Android downloads

Remember what you spent money on, keep receipts and prepare expense claims. The app appears on your phone as **Expense Tracker**. Spending and Claims have separate records.

**[Download v1.5.0 APK](https://github.com/vedhaS18-cyber/personal-tracker-downloads/releases/download/v1.5.0/personal-tracker-v1.5.0.apk)** · [Latest release](https://github.com/vedhaS18-cyber/personal-tracker-downloads/releases/latest) · [Privacy](PRIVACY.md) · [Help](SUPPORT.md)

Anyone can download without a GitHub account. This repository contains public downloads and user documentation; the app's development repository and source history remain private. GitHub's automatic “Source code” archives contain this documentation, not the Android app source.

## Install or update

1. Use an Android phone running **Android 8.0 or newer**. Download the `.apk` file above, not the source-code ZIP or TAR archive.
2. Open the APK. If Android asks, allow your browser or file manager to install this app. You can turn that installation permission off afterwards. Keep Play Protect enabled.
3. Open **Expense Tracker**. For automatic payment capture, enable notification access from the app's Spending settings and select the payment-alert apps you want it to check. This is optional; manual entry works without capture access.
4. For future updates, install the newer official APK over the existing app. **Do not uninstall first:** uninstalling or clearing storage removes local records. Use the separate Spending and Claims backup options before changing phones.

If Android says the app conflicts with an existing installation, stop and read [installation help](SUPPORT.md). Do not delete your current installation to work around the warning.

## What it does

- Saves recognised payment notifications from selected apps, including bank alerts shown by Messages and Gmail; it does not read your SMS or email inbox.
- Lets you add a purpose, review payments, filter by bank and record expenses manually.
- Organises receipts in independent expense claims and generates claim documents.
- Accepts image and PDF receipts. The optional scanner crops receipts, supports up to 10 pages per session and can crop gallery photos. Original is the default, with Filters available as an opt-in.

The optional scanner needs compatible Google Play services and may download its module on first use. Ordinary camera capture and direct Gallery attachment remain available. Read the [scanner privacy information](PRIVACY.md) before using it.

## Before relying on your records

Notification capture depends on what Android and the selected apps deliver. Alerts can be incomplete, late or missed, including Gmail alerts. Check important totals against your bank/card records and correct missing entries manually. This app does not connect to your bank, make payments or verify reimbursement eligibility.

Records are kept on your device. The app has no account-based recovery service. Exported backups contain financial information and are not password-encrypted by this app; choose their location carefully. See [privacy and deletion](PRIVACY.md).

This is a GitHub-distributed build, not a Google Play release. It retains the existing preview signing identity so current users can update without losing their installation. Its debugging flag is off. Permanent Play Store signing and any migration plan remain separate work.

## Verify the download

The release includes the APK, a SHA-256 checksum, a verification record and a third-party licence/notice ZIP accompanying the app. [Verification instructions and release identity](docs/verification.md) explain how to compare them. Download only from this repository's Releases page; a renamed or modified copy elsewhere is not an official update.

The APK was built on 20 September 2026. Public distribution began on 5 October 2026 using identical bytes. See the [release notes](CHANGELOG.md) and [testing limits](docs/verification.md).

## Help and security reports

Use [Help](SUPPORT.md) for installation and non-sensitive bug reports. Report security problems through [private vulnerability reporting](https://github.com/vedhaS18-cyber/personal-tracker-downloads/security/advisories/new), not a public issue. Never post real bank alerts, receipts, account details or backup files.

The app source is not offered under an open-source licence by this repository. [Third-party components retain their own licences and terms](THIRD_PARTY_NOTICES.md); their notices accompany the APK in the release's notice ZIP. Public availability does not imply that modified copies are official or endorsed.
