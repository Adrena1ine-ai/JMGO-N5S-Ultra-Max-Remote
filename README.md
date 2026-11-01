# JMGO N5S Ultra Max Remote

Unofficial user-maintained remote controls and localized quick-settings APK
for **JMGO N5S Ultra Max** with exact Android Build.MODEL **KD11CN**.

This repository is intentionally **separate** from projects for N5, N3
and other N5S firmware families. It contains release APKs, checksums and
model-specific OTA manifests. It is **not** an OEM firmware distribution.

## Updates

The modified Settings application contains the native
**System / Check panel updates** entry. Its OTA client reads only stable
GitHub Releases in this repository:

- Channel: n5sum
- Model: KD11CN
- Package: com.jmgo.setting.clone
- Manifest asset: n5sum-update.json
- Version tag: n5sum-vMAJOR.MINOR-codeNNNN
- APK asset prefix: JMGO_N5SUM_REMOTE_

The updater validates the model, package, tag, versionCode, HTTPS release
address, APK size, SHA256 and certificate before offering the native
JMGO Android installer with user confirmation. It does not install firmware,
remove application data or silently bypass user consent.

## Versions

Version 3696 (V96.4, four V97.2 feature transfers) is currently a
**pre-release** pending real screen checks for the localized network
destinations, first-frame weekday date and MEMC interaction on KD11CN.
Pre-releases are not returned by the stable releases/latest OTA endpoint.

Never install these APKs on another model (including N5, N3 and KD11AX)
without a separate compatibility review.

## Source and provenance

Private development, controlled patches and build tests are maintained
on server57 in a local Git repository. No private signing key or device
credentials are published here.
