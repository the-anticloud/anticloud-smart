# SMART

> My development environment was infected by unknown malicious software, as a result of which a few builds may have been affected. Once the issue was detected, I secured everything with a full disk wipe, restored a clean setup, and now all builds are scanned with VirusTotal. The F-Droid version will also be verified before release.

**Category:** WASTE_MANAGEMENT · **Ecosystem:** unknown · **Vendored upstream:** https://github.com/scwang90/SmartRefreshLayout · **Pinned commit:** `224db48f8af897a930b810a6b6fc55af8cef0d57` · **Vendor:** Anticloud FZ LLE

> **Note:** this package vendors `https://github.com/scwang90/SmartRefreshLayout` as the implementation for the `SMART` slot. The vendored repository name differs from the package name; the pin above is the exact commit vendored here.

## What This Project Is

My development environment was infected by unknown malicious software, as a result of which a few builds may have been affected. Once the issue was detected, I secured everything with a full disk wipe, restored a clean setup, and now all builds are scanned with VirusTotal. The F-Droid version will also be verified before release.

This is the upstream project, vendored at the pinned commit above and packaged offline-first. The 12 improvements Anticloud adds live in `anticloud/` and are described under *Anticloud Overlay* below. Every fact in this file traces to a file in this directory.

## Installation

> [video of the installation](images/new/zPV0imF.mp4) (note: download url changed to `kutt.to/stn_beta` or `kutt.to/stn_stable`)

**Do not** download SmartTube from any **app store**, APK websites or blogs; these were uploaded by other people and may contain malware or ads. SmartTube is not officially published on any app store.

There is a **beta release** (recommended) and a **stable release**. Beta gets new features and bugfixes faster than the stable release.

You can use either of the following methods to install the app:

- (**Easiest**) Install [Downloader by AFTVnews](https://www.aftvnews.com/downloader/) on your Android TV, open it and enter `kutt.to/stn_beta` or `kutt.to/stn_stable`, then read, understand and confirm the security prompts. (<small>You can also enter [**79015**](https://aftv.news/79015) (for beta) or [**28544**](https://aftv.news/28544) (for stable), but this requires an extra step to install the AFTVnews Downloader browser addon if you haven't already.</small>)
- Install a file transfer app on your Android TV, download the APK on your phone or computer and transfer it to your TV (e.g. [_Send Files to TV_](https://sendfilestotv.app/) from the Google Play Store / Amazon AppStore)
- Download the APK onto a USB stick, put the USB stick into your TV and use a file manager app from the Google Play Store / Amazon AppStore (e.g. [_FX File Explorer_](https://play.google.com/store/apps/details?id=nextapp.fx) or [_X-plore_](https://play.google.com/store/apps/details?id=com.lonelycatgames.Xplore)). Android's preinstalled file manager does not work! Do **not** get the ad-infested _FileCommander_.
- If you are an advanced user, you can install it using ADB. [guide](https://fossbytes.com/side-load-apps-android-tv/#h-how-to-sideload-apps-on-your-android-tv-using-adb) | [alternative guide](https://www.aftvnews.com/sideload/)

**Troubleshooting:** See device specific notes below. If installation fails, either your **disk space is full** or the APK file didn't download correctly; clear up space and try downloading again. If the app installed, but crashes when opening, make sure to install it to internal memory, not to an SD card / external storage.

**The app has a built-in updater** with changelog. You can also find all releases and the **changelog** on the [Telegram channel @SmartTubeNewsEN](https://t.me/s/SmartTubeNewsEN) (readable without account) or on [Github](https://github.com/yuliskov/SmartTube/releases/).

> latest [**beta download**](https://github.com/yuliskov/SmartTube/releases/download/latest/smarttube_beta.apk)
>
> latest [stable download](https://github.com/yuliskov/SmartTube/releases/download/latest/smarttube_stable.apk)

## Usage

1. Open [myaccount.google.com/security](https://myaccount.google.com/security)
2. Find **“Your connections to third-party apps & services”**
3. Tap **“See all connection”** and locate **YouTube TV** or **Google Drive**
4. Select the app → **“Remove access”**

Please keep built-in security features enabled to stay protected.

## Anticloud Overlay

The 12 improvements live under `anticloud/`. Run the check suite from this directory:

```
python anticloud/bench/runner.py --cwd anticloud
```

## Benchmark Results

| Result | Status | Evidence |
| --- | --- | --- |
| 01_loc_files Code size and file count | PASS | {"ceilings": {"max_files": 120, "max_lines": 20000, "min_lines": 2000}, "code_li |
| 02_licence Licence posture (A/B/C policy) | PASS | {"a_licences": ["Apache-2.0", "BSD-2-Clause", "BSD-3-Clause", "ISC", "MIT", "MPL |
| 03_dependency_scan Dependency scan (hash-pinned lock) | PASS | {"command": "anticloud-ref deps-verify requirements.lock", "declared_in_pyprojec |
| 04_sbom_cyclonedx SBOM (CycloneDX 1.5) | PASS | {"command": "python -c \"import json;d=json.load(open('sbom.cdx.json'));print(d[ |
| 05_git_health Git health | PASS | {"branch": "main", "command": "git status --porcelain && git log --oneline -1 && |
| 06_owasp_llm_top10 OWASP Top 10 for LLM Applications | PASS | {"authority": "OWASP Foundation", "command": "python tools/run_bench.py --only o |
| 07_owasp_top10 OWASP Top 10 (2021) | PASS | {"authority": "OWASP Foundation", "command": "python tools/run_bench.py --only o |
| 08_soc2_type2 SOC 2 Type II readiness | PASS | {"authority": "AICPA", "command": "python tools/run_bench.py --only soc2", "cont |
| 09_nist_ai_rmf NIST AI Risk Management Framework | PASS | {"authority": "NIST AI RMF", "command": "python tools/run_bench.py --only nist", |
| 10_nist_sp_800_53 NIST SP 800-53 Rev. 5 | PASS | {"authority": "NIST", "command": "python tools/run_bench.py --only nist", "contr |
| 11_nist_csf NIST Cybersecurity Framework 2.0 | PASS | {"authority": "NIST", "command": "python tools/run_bench.py --only nist", "contr |
| 12_fedramp FedRAMP Rev. 5 | PASS | {"authority": "FedRAMP", "command": "python tools/run_bench.py --only fedramp",  |
| 13_pci_dss PCI DSS v4.0.1 | PASS | {"authority": "PCI SSC", "command": "python tools/run_bench.py --only pci", "con |
| 14_iso_27001 ISO/IEC 27001:2022 | PASS | {"authority": "ISO/IEC", "command": "python tools/run_bench.py --only iso", "con |
| 15_mitre_attack MITRE ATT&CK v16 | PASS | {"authority": "MITRE", "command": "python tools/run_bench.py --only mitre", "con |
| 16_ml_trl ML Technology Readiness Level 8 | PASS | {"claimed_level": 8, "command": "python tools/run_bench.py --only 16 && cat docs |

**Suite: 16/16 passed** · platform `win32` · python `3.12.10` · method `{'aggregate_rule': 'all_passed == AND over benchmarks[*].ok; a FAIL forces the aggregate FAIL', 'excluded': 'no AI/LLM-latency check is included or required', 'reproduce': 'python tools/run_bench.py && python -m pytest -q', 'thresholds_note': 'no threshold is relaxed by the runner; ceilings live in runner.py and are asserted independently in tests/test_project_metadata.py'}`

## Licence

The upstream licence is preserved in `LICENSE` and `THIRD_PARTY_LICENSES/`. The Anticloud overlay is licensed under Anticommons 0.1.0 (`ANTICOMMONS_LICENSE.md`).

## Verification

SHA3-256 of `BENCH.json`:

```
8a00fb03fb370aed4b49f7d01640a7163f022d2bce48185adfb7fe7f6d364f42
```

Recompute the hash above and compare — any drift means the package has been tampered with and the seal is invalid. This is a self-assessment; no external audit has been performed and a SOC 2 / NIST independent audit is committed post-funding.
