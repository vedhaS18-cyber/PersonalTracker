# Security policy

## Reporting a vulnerability privately

Please use
[GitHub's private vulnerability reporting form](https://github.com/vedhaS18-cyber/personal-tracker-downloads/security/advisories/new)
to report a suspected security problem. You will need a GitHub account. Reports
submitted through this form are private to the repository's security reporting
process until deliberately published.

Do not describe an exploitable vulnerability, disclose personal data or attach
credentials in a public issue. If the private form is unavailable, open a public
issue that says only that you need a private security contact, without including
the vulnerability details. There is no dedicated security email at present.

Include the app version, affected Android version, steps to reproduce and the
possible impact. Use invented data and a device or test environment you own or
have permission to use. Remove private information from logs and screenshots.
Do not include full receipt collections, payment backups, real bank alerts,
passwords or signing keys.

## Supported releases

Security fixes are intended for the latest release on this repository's
[Releases page](https://github.com/vedhaS18-cyber/personal-tracker-downloads/releases/latest).
Older versions do not have a separate maintenance commitment. Reports are handled
on a best-effort basis; a specific response or fix timeline is not guaranteed.

## Download and update safety

- Obtain the APK from this repository's Releases page. Avoid APKs repackaged by
  unrelated sites.
- Use the supplied SHA-256 checksum to check that a downloaded file matches the
  release. A matching checksum is an integrity check, not a guarantee that an app
  has no vulnerabilities.
- Android checks signing compatibility when updating an installed app. If an
  update cannot be installed, report the error instead of uninstalling and losing
  local records.
- Keep your phone and Android security updates current. Use a screen lock.
- Protect exported backups and receipts. The app does not password-encrypt
  Spending backups and does not provide a separate app lock.

This repository distributes the existing signed GitHub APK. It is not a Google
Play listing, and download availability does not imply Google review or approval.
See [PRIVACY.md](PRIVACY.md) for the app's data handling and its limits.
