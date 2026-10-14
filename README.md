# SMART

![license](https://img.shields.io/badge/license-MIT-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![category](https://img.shields.io/badge/category-waste_management-lightgrey)

> Anticloud-hardened packaging of the upstream project `SMART` in category **WASTE MANAGEMENT**. Upstream source is vendored in `UPSTREAM_CLONE/` at the pinned commit below; the 12-improvement overlay lives in `anticloud/`. Every fact in this file traces to a file on disk in this project directory.

**Category:** WASTE MANAGEMENT · **Upstream:** https://github.com/scwang90/SmartRefreshLayout · **Upstream pin:** `224db48f8af897a930b810a6b6fc55af8cef0d57` · **Vendor:** Anticloud FZ LLE

---

## What This Project Does

[<img src="images/badge_fdroid.png" alt="Get it on F-Droid" height="80">](https://f-droid.org/packages/app.smarttube.fdroid/)
[<img src="images/badge_github.png" alt="Get it on GitHub" height="80">](https://github.com/yuliskov/SmartTube/releases)

# Important announcement about the app

My development environment was infected by unknown malicious software, as a result of which a few builds may have been affected. Once the issue was detected, I secured everything with a full disk wipe, restored a clean setup, and now all builds are scanned with VirusTotal. The F-Droid version will also be verified before release.

Public keys may have been compromised, which is why I am sharing this issue. You can download the new version and the new public key below, and instructions for restoring backups are provided.

No extra actions are required since the app uses **one-time connection codes**. These codes have very limited permissions (for example, they cannot change your password). Still, you can revoke them if you want full peace of mind.

# How to revoke access:

1. Open [myaccount.google.com/security](https://myaccount.google.com/security)
2. Find **“Your connections to third-party apps & services”**
3. Tap **“See all connection”** and locate **YouTube TV** or **Google Drive**
4. Select the app → **“Remove access”**

Please keep built-in security features enabled to stay protected.

# SmartTube
  
<!-- <img width="100" src="https://github.com/yuliskov/SmartTube/blob/master/smarttubetv/src/ststable/res/mipmap-nodpi/app_icon.png" alt="logo"/> -->

![The app screenshot](./images/browse_home.png)

SmartTube is a free and open-source media client for Android TVs and TV boxes. It allows you to browse and play content from various public sources in a TV-optimized interface.

### ✅ Features
- Clean interface 
- SponsorBlock integration  
- Adjustable playback speed  
- 8K resolution support  
- 60fps playback  
- HDR compatibility  
- View live chat  
- Customizable buttons  
- Does not require Google Services  
- Helpful international community

### ❌ Limitations
- Not supported on phones and tablets  
- Comment functionality is unstable  
- Voice search and casting performance may be inferior to official apps, depending on your device  

Give it a try!

**Do you have any question?** Ctrl+F or ⌘F this readme first!

[**Installation**](#installation) | [**Official Site**](https://smarttubeapp.github.io) | [**Donation**](#donation) | [**FAQ**](#faq) | [Support / Chat](#support) | [Build](#build) | [Translate the app](https://jtbrinkmann.de/tools/android-strings.xml-translator.html) | [Changelog](https://t.me/s/SmartTubeNewsEN) | [Liability](#liability)

## Device support
> [!IMPORTANT]  
> Starting in October 2025 new Amazon FireTV devices no longer run Android under the hood. SmartTube will **not** be compatible with the Fire Stick 4k Select and newer devices which run Amazon's own VegaOS.

![Device support image](images/new/compatibility.png)
* **Supported:** all Android TVs and TV boxes (incl. All FireTV devices released before Oct. 2025, NVIDIA Shield & Chromecast with Google TV), even older ones with Android 4.3 (Kitkat).
* **Not supported:** Smartphones, non-Android platforms like Samsung Tizen, LG webOS, Apple TV, etc.

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

### Installation

*(excerpt; full text in `UPSTREAM_CLONE/`)*

*Quoted from the upstream `README.md` file in `UPSTREAM_CLONE/`.*
Project-specific facts detected in this directory:

- Ecosystem: **Java / Gradle** (manifests: build.gradle; scanned in UPSTREAM_CLONE)
- Top-level source layout: `MediaServiceCore/`, `SharedModules/`, `chatkit/`, `common/`, `doubletapplayerview/`, `exoplayer-amzn-2.10.6/`, `fastlane/`, `filepicker-lib/`, `fragment-1.1.0/`, `gradle/`, `images/`, `leanback-1.0.0/`
- Snapshot size: **3265 files**, **408583 lines of code** (measured; see Benchmarks)
- Primary languages: `.java` (1679), `.xml` (811), `.png` (361), `.dump` (90), `(none)` (80), `.gradle` (46)
- Upstream commit pinned for this packaging: `224db48f8af897a930b810a6b6fc55af8cef0d57`

---

## Installation

Public keys may have been compromised, which is why I am sharing this issue. You can download the new version and the new public key below, and instructions for restoring backups are provided.

No extra actions are required since the app uses **one-time connection codes**. These codes have very limited permissions (for example, they cannot change your password). Still, you can revoke them if you want full peace of mind.

*Section quoted from the upstream readme.*
Overlay install (this project):

```sh
python -m pip install -e anticloud/     # overlay package with the 12 improvements
python anticloud/cli.py --help          # 13 subcommands, JSON stdout
```

---

## Usage

No usage section was found in the upstream readme. Entry points detected in this project directory:

Browse the snapshot layout listed under What This Project Does and follow the upstream run instructions for the detected ecosystem (Java / Gradle).

Anticloud overlay CLI (available in every project):

```sh
python anticloud/cli.py --help     # 13 subcommands, JSON stdout
python anticloud/cli.py checks     # run the 16-check suite
```

---

## API

The upstream API surface is defined by the `SMART` source tree vendored in `UPSTREAM_CLONE/` (Java / Gradle ecosystem). Public entry points:

- Source modules: `MediaServiceCore/`, `SharedModules/`, `chatkit/`, `common/`, `doubletapplayerview/`, `exoplayer-amzn-2.10.6/`, `fastlane/`, `filepicker-lib/`
- Overlay API: `anticloud/cli.py` exposes 13 subcommands with JSON stdout; `anticloud/bench/runner.py` runs the 16-check suite; `anticloud/provenance/chain.py` exposes the SHA3-256 + Ed25519 provenance chain.

---

## Dependencies

| Metric | Value |
|--------|-------|
| Ecosystem | Java / Gradle |
| Manifests detected | build.gradle |
| Files in snapshot | 3265 |
| Lines of code | 408583 |
| Dependency references | 0 |
| Upstream license | MIT |
| Overlay license | Anticommons 0.1.0 |

Pinned lockfile: `anticloud/requirements.lock` (hash-pinned, PEP 508). SBOM: `sbom.cdx.json` (CycloneDX 1.5, pinned to the upstream SHA).

---

## Configuration

Public keys may have been compromised, which is why I am sharing this issue. You can download the new version and the new public key below, and instructions for restoring backups are provided.

No extra actions are required since the app uses **one-time connection codes**. These codes have very limited permissions (for example, they cannot change your password). Still, you can revoke them if you want full peace of mind.

*Section quoted from the upstream readme.*
Overlay configuration (Anticloud):

- `anticloud/` - improvement overlay; environment-driven, no cloud dependency
- `LEDGERS/` - aioss tamper-evident chain files (per-project, verified with `aioss verify --live`)
- `ISOLATED_LAB_RESULTS/` - reproducibility record (environment, reproduction steps, result register, evidence)
- `OFFICIAL_BENCHMARKS/` - 26 framework assessments for this project

---

## Contributing

Upstream contributions: fork the `SMART` project, create a feature branch, and open a pull request against upstream. Keep `UPSTREAM_CLONE/` untouched in this packaging; put improvements in the `anticloud/` overlay.

Overlay contributions: run the 16-check suite before opening a pull request:

```sh
python anticloud/bench/runner.py --cwd anticloud
```

---

## License

**Upstream license: MIT** (evidence: `LICENSE` in the upstream snapshot).

License file excerpt:

```text
MIT License

Copyright (c) 2020-present yuliskov

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
```

### Anticommons 0.1.0 overlay

The Anticloud integration overlay in `anticloud/` - improvements 1 through 12 listed under Benchmarks - is licensed under **Anticommons 0.1.0**. Upstream code remains under its original MIT terms. See `ANTICOMMONS_LICENSE.md` in this directory for the overlay terms and contact.

SPDX: `MIT` (upstream) + Anticommons 0.1.0 (overlay, dual).

---

## Upstream

- **Project:** `SMART` (category: WASTE MANAGEMENT)
- **Upstream URL:** https://github.com/scwang90/SmartRefreshLayout
- **Pinned commit (SHA):** `224db48f8af897a930b810a6b6fc55af8cef0d57`
- **Branch:** main
- **Pin provenance:** GitHub API commits/main. The parent-project stamp is explicitly rejected for this project.
- **Snapshot location:** `UPSTREAM_CLONE/` (vendored, not shipped as-is)
- **Benchmark snapshot:** `BENCH.json`

---

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`edd445e2cffec373d2c3099127a9a22f713dc5baa4b25ebb0bc00b8125f8094a`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe and Mail, Business Insider, National Post, Financial Post, StreetInsider, Digital Journal, Barchart, International Business Times, and fox47 · National Law Review.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

