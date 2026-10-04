# Verify v1.5.0

This public download reuses the existing signed APK without rebuilding or changing it. The public repository tag identifies the download documentation, not the private app source commit embedded in the APK.

| Item | Expected value |
| --- | --- |
| File | `personal-tracker-v1.5.0.apk` |
| Size | 22,988,538 bytes |
| SHA-256 | `33c5ad8fe56265673025c83dcf961153134df0c288c108a6b584faf975d86237` |
| Version | 1.5.0, version code 22 |
| Package | `com.everyday.expense.debug` |
| Launcher name | Expense Tracker |
| Minimum Android | 8.0 / API 26 |
| Target Android API | 36 |
| APK debugging | Disabled |
| Signing certificate SHA-256 | `ecbf1f5b7ffc487131abc723bcb23fee47ad51a9140646fa9e9cf2839570c71a` |
| Embedded private source revision | `486f38dd23f8a18267618d8fa815a94155ebcb92` |

## Compare the file

On Windows, open PowerShell in your download folder and run:

```powershell
Get-FileHash -Algorithm SHA256 .\personal-tracker-v1.5.0.apk
```

On macOS:

```sh
shasum -a 256 personal-tracker-v1.5.0.apk
```

On Linux:

```sh
sha256sum personal-tracker-v1.5.0.apk
```

The result must match the APK hash above and the release's `.apk.sha256` file. A checksum detects different bytes; use it from this official page rather than trusting a checksum supplied by an unknown mirror. Android also verifies the signing identity when updating an existing installation.

## What was verified for the app build

The 20 September 2026 build passed 114 local unit tests in 25 suites with zero failures, errors or skips. Full DeviceTest lint reported zero errors and 45 existing warnings. App compilation, instrumented-test source compilation and APK assembly passed. Instrumented tests were compiled, not executed for that update.

The package, version, non-debuggable status, signing certificate and embedded source revision were checked. The APK passed 16 KB ZIP alignment and checks of all four packaged 64-bit native libraries. Independent code review covered batch import, failures, cancellation, cleanup, draft migration and filter defaults.

No new emulator or physical-phone testing is claimed for this publication. Real-paper scanning, glare/low light, actual filters and gallery crops, EXIF/PDF handling, older Android and process termination during scanning remain device checks. This is not a complete security audit, a guarantee of notification coverage or a Play Store submission.

## Public distribution checks

The APK, checksum and original verification text are copied as unchanged release assets. A fourth asset provides the accompanying third-party licence and notice texts. Publication checks compare uploaded and downloaded files with the verified local bytes, check access without GitHub credentials and confirm the development repository remains private. The completed publication result is recorded in [publication.md](publication.md).

The original verification attachment mentions a source/tag commit and historical CI results. Those refer to the private app build, not a public build workflow. This downloads repository has no app build workflow.
