# Public download publication

Published and verified on **5 October 2026**. The app identity and original build
checks are documented in [verification.md](verification.md).

## Files checked

All four draft assets were downloaded and compared with the local publication
files before the release was made live. All four published assets were then
downloaded again **without GitHub credentials, cookies or an Authorization header**.
Every file matched its expected byte count and SHA-256 checksum.

| Asset | Bytes | SHA-256 |
| --- | ---: | --- |
| `personal-tracker-v1.5.0.apk` | 22,988,538 | `33c5ad8fe56265673025c83dcf961153134df0c288c108a6b584faf975d86237` |
| `personal-tracker-v1.5.0.apk.sha256` | 95 | `2e80145c08fbe0af0b319ff1410169184696e31624946ab854e68eaeef6638d2` |
| `personal-tracker-v1.5.0-verification.txt` | 2,416 | `a6d4aa325a7e12021b8f0c0a3ce4c5b019490f8386ed721004aa0b46d6328f3a` |
| `personal-tracker-v1.5.0-third-party-notices.zip` | 156,075 | `9cbff4491d642d27616464508e6a6ab397a43cf80d0d412e9db81e84ecb072e4` |

The first three files are identical to the existing v1.5.0 distribution. The
fourth supplies the third-party notice index and 33 accompanying notice/provenance
files. It does not modify or re-sign the APK. The APK's signature, package, version,
embedded source revision and 16 KB native alignment were rechecked before upload.

## Repository boundaries and settings

- This repository is public; anonymous release downloads succeeded.
- The development repository remains private. No app source tree or development
  Git history was copied here. The public history starts with its own independent
  documentation commit.
- Public release tag `v1.5.0` points to documentation commit
  `5eb893053d8547728ac7d11db695c464cc7873ff`. It does not represent the private
  Android source tree.
- The published release is immutable, and release immutability is enabled.
- GitHub Actions is disabled. No automated app builds run in this repository.
- Secret scanning and push protection are enabled.
- Private vulnerability reporting is enabled.
- Main-branch protection blocks force-pushes and deletion, including for admins.
- The repository owner is the only listed collaborator.

Public documentation and notice links passed a local link check. Review found no
private repository URLs, workstation paths or obvious credentials in the prepared
public files. A limited APK-content check did not find obvious private keys,
receipts or databases. These checks are not an exhaustive security or legal audit.

No app rebuild, emulator run or phone installation was performed for this public
distribution. The app's existing behavior and device-testing limits are unchanged.

## Presentation and repository rename

On **5 October 2026**, the public repository was renamed from
`personal-tracker-downloads` to `PersonalTracker`. The README now includes a
White Frost banner, an Android download button and a concise feature overview.
Installation, privacy, support and signing information remains available.

- The published README was visually checked on GitHub while signed out.
- All four release assets were downloaded anonymously from the renamed repository
  and matched the byte counts and checksums above.
- The old repository URL and old direct APK link both redirected successfully.
- The development repository remained private. An anonymous repository listing
  showed only this public downloads repository.
- Actions remained disabled; secret scanning, push protection, private vulnerability
  reporting and main-branch protection remained enabled. The release stayed immutable.

The APK and release assets were not changed. The immutable third-party notice ZIP
still contains the original privacy-document URL, which continues to redirect.
