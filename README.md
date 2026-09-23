# isolmaSS updates

Public Windows release repository for [isolmaSS](https://github.com/isolmaz/isolmaSS-updates/releases/latest). This repository contains release metadata and binaries, not the private source code or publisher private key.

Current release: **v0.4.2**. Download `isolmass-setup.exe` for a per-user installation or `isolmass-portable-windows-x64.zip` for manual portable use. The app uses `isolmass-setup.exe.sig` to verify the installer with its pinned public key; a portable ZIP does not automatically replace an installed copy. Asset hashes and the private source commit are recorded in [`releases/v0.4.2.json`](releases/v0.4.2.json).

An installed build without the pinned-key verifier requires one manual installation of 0.4.0 or later. Windows SmartScreen may warn because the installer is not Authenticode-signed; no warning is bypassed automatically. Never execute an update unless its identity and origin match what you intended to install.

The 0.4.2 Settings window uses a compact two-column layout and content-sized tabs. Manual checks show progress and results in Settings or through a visible tray result dialog; installation consent warns that isolmaSS will close and restart. Earlier signed releases and manifests remain immutable.
