# Third-party licences and notices

Personal Tracker v1.5.0 uses third-party software and the Inter font. Their
copyrights, licences, notices and applicable terms remain in force. Publishing the
APK does not relicense those components or make this app's private source code
open source.

The [`licenses/`](licenses/) directory supplies upstream licence and notice text
alongside the download documentation. Keep these materials with any permitted
redistribution. The original APK has not been rebuilt or modified for this public
download. Some dependency notices are not embedded in that APK, so the companion
materials on this page are part of its distribution.

## Runtime libraries and font

| Component | Licence / accompanying notices |
| --- | --- |
| Inter font | [SIL Open Font License 1.1 and copyright](licenses/Inter-OFL-1.1.txt); also embedded in the APK |
| AndroidX, Jetpack Compose, Kotlin and Kotlinx, Dagger/Hilt, Coil, Accompanist, OkHttp/Okio and related Android runtime libraries | [Apache License 2.0](licenses/Apache-2.0.txt); additional supplied notices appear below and in Google's scanner bundle |
| Apache POI 5.5.1, including OOXML and OOXML Lite | [Licence and subcomponent terms](licenses/poi-5.5.1-LICENSE.txt), [NOTICE](licenses/poi-5.5.1-NOTICE.txt); the individual OOXML artefact copies are retained in `licenses/` |
| Apache Commons Codec 1.20.0 | [Licence](licenses/commons-codec-1.20.0-LICENSE.txt), [NOTICE](licenses/commons-codec-1.20.0-NOTICE.txt) |
| Apache Commons Collections 4.5.0 | [Licence](licenses/commons-collections4-4.5.0-LICENSE.txt), [NOTICE](licenses/commons-collections4-4.5.0-NOTICE.txt) |
| Apache Commons Math 3.6.1 | [Licence](licenses/commons-math3-3.6.1-LICENSE.txt), [NOTICE](licenses/commons-math3-3.6.1-NOTICE.txt) |
| Apache Commons IO 2.21.0 | [Licence](licenses/commons-io-2.21.0-LICENSE.txt), [NOTICE](licenses/commons-io-2.21.0-NOTICE.txt) |
| Apache Commons Compress 1.28.0 | [Licence](licenses/commons-compress-1.28.0-LICENSE.txt), [NOTICE](licenses/commons-compress-1.28.0-NOTICE.txt) |
| Apache Commons Lang 3.18.0 | [Licence](licenses/commons-lang3-3.18.0-LICENSE.txt), [NOTICE](licenses/commons-lang3-3.18.0-NOTICE.txt) |
| Apache Log4j API 2.25.5 | [Licence](licenses/log4j-api-2.25.5-LICENSE.txt), [NOTICE](licenses/log4j-api-2.25.5-NOTICE.txt), [upstream dependency notice](licenses/log4j-api-2.25.5-DEPENDENCIES.txt) |
| Apache XMLBeans 5.3.0 | [Licence](licenses/xmlbeans-5.3.0-LICENSE.txt), [NOTICE](licenses/xmlbeans-5.3.0-NOTICE.txt) |
| SparseBitSet 1.3 | [Apache License 2.0](licenses/Apache-2.0.txt); [upstream project](https://github.com/brettwooldridge/SparseBitSet) |
| CurvesAPI 1.08 | [BSD licence and Graph Builder copyright](licenses/curvesapi-1.08-LICENSE.txt), copied from the [upstream 1.08 release](https://github.com/virtuald/curvesapi/blob/1.08/license.txt) |
| Jakarta Inject API 2.0.1 | [Licence](licenses/jakarta.inject-api-2.0.1-LICENSE.txt), [NOTICE](licenses/jakarta.inject-api-2.0.1-NOTICE.md) |
| Public Suffix List data used by OkHttp 4.12.0 | [Packaged notice](licenses/okhttp-4.12.0-NOTICE.txt), [Mozilla Public License 2.0](licenses/MPL-2.0.txt); source information below |

The dependency names above describe libraries used by this build, not a claim
that every feature of every library is used. Upstream licence files can include
notices for their own subcomponents and build tools; they are preserved verbatim,
not presented as an inventory of separate app features.

## Google document scanner and Play services

The optional scanner uses
`com.google.android.gms:play-services-mlkit-document-scanner:16.0.0` and its
runtime dependencies. Google's SDK distribution includes its own
[third-party licence bundle](licenses/google-document-scanner-16.0.0-third_party_licenses.txt)
and [index](licenses/google-document-scanner-16.0.0-third_party_licenses.json).
These files are reproduced unchanged from the SDK artefact. Their inclusion does
not imply that every item named in Google's bundle is separately packaged or used
by Personal Tracker.

Google's SDK is subject to the [ML Kit terms](https://developers.google.com/ml-kit/terms),
which incorporate the [Google APIs Terms of Service](https://developers.google.com/terms).
Applicable Google Play services terms also remain in force. These components are
not relicensed under the common Apache licence above. Google processes scanner
usage and performance metrics; see the app's
[privacy information](https://github.com/vedhaS18-cyber/personal-tracker-downloads/blob/main/PRIVACY.md).

## Public Suffix List source

OkHttp includes a compiled copy of Public Suffix List data under MPL 2.0. Its
upstream notice is included above. The list's source and licence are available
from the [Public Suffix List project](https://publicsuffix.org/list/) and
[source repository](https://github.com/publicsuffix/list). The exact compiled
resource used by OkHttp 4.12.0 is available in
[OkHttp's 4.12.0 source tree](https://github.com/square/okhttp/tree/parent-4.12.0/okhttp/src/main/resources/okhttp3/internal/publicsuffix).
Personal Tracker does not modify this resource. The MPL rights for this data are
not restricted by the app's private-source status.

## Provenance and scope

[`licenses/PROVENANCE.json`](licenses/PROVENANCE.json) identifies the artefacts and
archive entries used for the copied notice files. CurvesAPI's licence comes from
its upstream 1.08 tag; MPL 2.0 comes from
[Mozilla's published licence text](https://www.mozilla.org/en-US/MPL/2.0/).
The Inter notice matches the APK asset. Upstream texts retain their original
wording and formatting.

This is a distribution notice collection for v1.5.0, not a legal certification,
an exhaustive software bill of materials or a security audit. It covers the
identified runtime notice gap without including the private app source, signing
keys, user receipts or development history. Future app builds must review their
own changed dependencies and notice requirements.
