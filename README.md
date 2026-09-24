# isolmaSS updates

Public Windows release repository for [isolmaSS](https://github.com/isolmaz/isolmaSS-updates/releases/latest). This repository contains release metadata and binaries, not the [public application source](https://github.com/isolmaz/isolmaSS_V2) or publisher private key.

Current release: **v0.5.0**. Download `isolmass-setup.exe` for a per-user installation or `isolmass-portable-windows-x64.zip` for manual portable use. The app uses `isolmass-setup.exe.sig` to verify the installer with its pinned public key; a portable ZIP does not automatically replace an installed copy. Asset hashes and the public source commit are recorded in [`releases/v0.5.0.json`](releases/v0.5.0.json).

An installed build without the pinned-key verifier requires one manual installation of 0.4.0 or later. Windows SmartScreen may warn because the installer is not Authenticode-signed; no warning is bypassed automatically. Never execute an update unless its identity and origin match what you intended to install.

Version 0.5.0 adds an explicit **Upload** action and detailed Cloudflare settings. Users who want share links install a private Worker/R2/D1 from the [public source tag](https://github.com/isolmaz/isolmaSS_V2/tree/v0.5.0/cloudflare) into their own Cloudflare account; the publisher provides no central image host. Local Copy/Save needs no Cloudflare account. The [static site source](https://github.com/isolmaz/isolmaSS_V2/tree/v0.5.0/site) provides bilingual downloads, documentation and privacy information; its custom-domain deployment belongs to the account owner. Earlier signed releases and manifests remain immutable.
