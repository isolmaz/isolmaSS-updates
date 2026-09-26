# isolmaSS updates

Public Windows release repository for [isolmaSS](https://ss.isolmaz.com). It holds release metadata and signed binaries only; the application source lives in [`isolmaz/isolmaSS_V2`](https://github.com/isolmaz/isolmaSS_V2) and the publisher's private key is never stored here.

Current release: **v0.5.7**. Download [`isolmass-setup.exe`](https://github.com/isolmaz/isolmaSS-updates/releases/latest/download/isolmass-setup.exe) for a per-user installation, or [`isolmass-portable-windows-x64.zip`](https://github.com/isolmaz/isolmaSS-updates/releases/latest/download/isolmass-portable-windows-x64.zip) for manual portable use. Asset hashes and the source commit are recorded in [`releases/v0.5.7.json`](releases/v0.5.7.json); each release has its own manifest in [`releases/`](releases/).

isolmaSS captures a region or window, lets you mark it up, and copies, saves or uploads it. Upload sends the image to a Worker the app installs in your own Cloudflare account and shows the link in a small card with Copy and Open; the link is already on the clipboard. The publisher hosts no screenshots, and local capture needs no Cloudflare account.

The installed app verifies `isolmass-setup.exe` with `isolmass-setup.exe.sig` against its pinned publisher key before installing, and again right before running it. The installer is not Authenticode-signed, so Windows SmartScreen may warn; the app never bypasses that warning. A portable ZIP does not replace an installed copy. Published releases and manifests are immutable; every change ships as a new version.

Cloudflare installation, sharing and upload behave according to the account you authorize; usage in that account may incur Cloudflare charges.
