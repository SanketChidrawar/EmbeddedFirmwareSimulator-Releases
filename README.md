# Embedded Firmware Simulator releases

[Official product page, screenshots and getting started](https://embedded-firmware-simulator.witty-genet-3312.chatgpt.site)

Windows installers and signed update feeds for Embedded Firmware Simulator.

[Download setup.exe for installation or upgrade](https://mxciidrxfhanxknxcrgx.supabase.co/functions/v1/distribution-download)

Requires Windows 10 or 11 on an Intel/AMD 64-bit PC. Python and simulation runtimes
are included; recipients do not need to install development tools.

## Upgrade an existing copy

1. Save your projects and close Embedded Firmware Simulator.
2. Run setup.exe and keep the existing installation folder.
3. Check for subsequent releases inside the app under Tools → Updates and privacy.
   Releases after v0.2.0.5 show a green Update available button at the top-right
   only when a newer version has been detected. There is no top-right control
   when up to date. Version v0.2.0.5 uses its existing Tools menu.

Saved projects and reports are kept. The first upgrade enables the update checker
in older copies that did not have one. Later releases are offered inside the app;
installation requires the user's confirmation.

## Optional activity reports

Anonymous reporting can be enabled or disabled in Tools → Updates and privacy.
It sends a random installation ID, app version, platform and activity times.
It does not send circuits, firmware, project files, names or email addresses.

## Release verification

New releases contain one installer, setup.exe, its SHA256 checksum, release metadata
and a signed stable.json feed. The historical v0.2.0.5 also contains Update.exe;
setup.exe can be used for both installation and upgrades. The app verifies the Ed25519 feed signature and the
installer's hash and size before installation. Feed signing is separate from a
Windows Authenticode publisher certificate; these executables have no such certificate.

The latest release page contains version-specific assets and release notes.
This repository contains release artifacts and documentation. Signing keys and
account credentials stay on the publisher's PC.
