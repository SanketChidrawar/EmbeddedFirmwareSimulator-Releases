# Embedded Firmware Simulator releases

Windows installers and signed update feeds for Embedded Firmware Simulator.

[Download setup.exe for a first installation](https://mxciidrxfhanxknxcrgx.supabase.co/functions/v1/distribution-download)

[Download Update.exe for an existing installation](https://github.com/SanketChidrawar/EmbeddedFirmwareSimulator-Releases/releases/latest/download/Update.exe)

Requires Windows 10 or 11 on an Intel/AMD 64-bit PC. Python and simulation runtimes
are included; recipients do not need to install development tools.

## Upgrade an existing copy

1. Save your projects and close Embedded Firmware Simulator.
2. Run Update.exe. It finds the existing installation, updates it and reopens the app.
3. Use Tools → Updates and privacy to check for subsequent releases.

Saved projects and reports are kept. The first upgrade enables the update checker
in older copies that did not have one. Later releases are offered inside the app;
installation requires the user's confirmation.

## Optional activity reports

Anonymous reporting can be enabled or disabled in Tools → Updates and privacy.
It sends a random installation ID, app version, platform and activity times.
It does not send circuits, firmware, project files, names or email addresses.

## Release verification

Each release includes setup.exe, Update.exe, SHA256 checksums, release metadata and
a signed stable.json feed. The app verifies the Ed25519 feed signature and the
installer's hash and size before installation. Feed signing is separate from a
Windows Authenticode publisher certificate; these executables have no such certificate.

The latest release page contains version-specific assets and release notes.
This repository contains release artifacts and documentation. Signing keys and
account credentials stay on the publisher's PC.
