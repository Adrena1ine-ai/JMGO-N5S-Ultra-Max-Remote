# JMGO N5S Ultra Max Remote

Unofficial user-maintained remote controls and localized quick-settings APK
for **JMGO N5S Ultra Max** with exact Android Build.MODEL **KD11CN**.

This repository is intentionally **separate** from projects for N5, N3
and other N5S firmware families. It contains release APKs, checksums and
model-specific OTA manifests. It is **not** an OEM firmware distribution.

## Current public beta

**JMGO Settings+ v1.0 Beta** (Android versionCode **3726**), based on the
2026.09.17.2 JMGO Settings app, 17 September 2026.

- Official release label and Android launcher label: **JMGO Settings+ v1.0 Beta**.
- Android System item: **Settings+ проверка обновления**.
- [Download signed APK](https://github.com/Adrena1ine-ai/JMGO-N5S-Ultra-Max-Remote/releases/tag/n5sum-v1.0-code3726).
- Compatible only with **N5S Ultra Max / KD11CN**.
- Keep app data and existing remote bindings on in-place upgrades; same signing certificate.

## Updates

The modified Settings application contains the native
**System → Settings+ проверка обновления** entry. Its OTA client reads the
model-specific manifest from this repository main branch. It supports
controlled prereleases as well as stable GitHub Releases, with cryptographic
APK validation:

- Channel: n5sum
- Model: KD11CN
- Package: com.jmgo.setting.clone
- Manifest: https://raw.githubusercontent.com/Adrena1ine-ai/JMGO-N5S-Ultra-Max-Remote/main/n5sum-update.json
- Version tag: n5sum-vMAJOR.MINOR-codeNNNN
- APK asset prefix: JMGO_N5SUM_REMOTE_

The updater validates the model, package, tag, versionCode, HTTPS release
address, APK size, SHA256 and certificate before offering the native
JMGO Android installer with user confirmation. It does not install firmware,
remove application data or silently bypass user consent.

## Versions

Earlier experimental versions are preserved in GitHub Releases.
The manifest in main points to the current explicitly published channel version. Future releases must update that manifest after uploading assets. This avoids GitHub releases/latest 404 and anonymous API 403 rate limits. A native Android/JMGO installation still requires user confirmation.

Never install these APKs on another model (including N5, N3 and KD11AX)
without a separate compatibility review.

## Source and provenance

Private development, controlled patches and build tests are maintained
on server57 in a local Git repository. No private signing key or device
credentials are published here.
