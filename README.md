# isolmaSS updates

Public Windows release repository for [isolmaSS](https://github.com/isolmaz/isolmaSS-updates/releases/latest). This repository contains release metadata and binaries, not the [public application source](https://github.com/isolmaz/isolmaSS_V2) or publisher private key.

Current release: **v0.5.1**. Download `isolmass-setup.exe` for a per-user installation or `isolmass-portable-windows-x64.zip` for manual portable use. The app uses `isolmass-setup.exe.sig` to verify the installer with its pinned public key; a portable ZIP does not automatically replace an installed copy. Asset hashes and the public source commit are recorded in [`releases/v0.5.1.json`](releases/v0.5.1.json).

An installed build without the pinned-key verifier requires one manual installation of 0.4.0 or later. Windows SmartScreen may warn because the installer is not Authenticode-signed; no warning is bypassed automatically. Never execute an update unless its identity and origin match what you intended to install.

Version 0.5.1 makes the first **Upload** open a short Cloudflare setup. The screenshot stays local while the user approves deployment of their own private Worker/R2/D1, copies two keys and pairs the provided `workers.dev` address. Pairing from Upload then sends the pending screenshot automatically; subsequent Upload actions need no setup. No custom domain is needed or attached automatically. Unfinished setup keys are DPAPI-protected for the current Windows user. See the [public source tag](https://github.com/isolmaz/isolmaSS_V2/tree/v0.5.1/cloudflare) and [bilingual site source](https://github.com/isolmaz/isolmaSS_V2/tree/v0.5.1/site). The publisher hosts no screenshots; local Copy/Save requires no Cloudflare account. Earlier signed releases and manifests remain immutable.
