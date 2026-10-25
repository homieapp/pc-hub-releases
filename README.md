# Homie PC Hub downloads

Use a compatible computer at home as a local Matter controller for [Homie](https://smarthomie.ai).

## Linux beta

[Download Linux beta 0.1.0-beta.1](https://github.com/homieapp/pc-hub-releases/releases/tag/desktop-hub-linux-v0.1.0-beta.1).

The supported beta target is Ubuntu 24.04 x64 with a graphical desktop and Bluetooth. The `.deb` is recommended because it installs the Bluetooth permission and launch-at-login hooks. AppImage is an alternative portable build with manual setup requirements.

Download the `.deb` and `SHA256SUMS-linux` from the same release, then run:

```bash
sha256sum --ignore-missing --check SHA256SUMS-linux
sudo apt install ./homie-desktop-hub-0.1.0-beta.1-amd64.deb
```

Open **Homie PC Hub**, sign in with your Homie account, and choose the home this computer will serve. Keep the computer awake and signed in. Closing the window keeps the hub running in the tray; choosing Quit stops it.

This beta has passed automated installation, sandboxed startup, setup renderer, local bridge authentication, reinstall/restart, and retained-data tests. Physical Bluetooth/Matter pairing and production use are being tested during the beta. Packages are unsigned; SHA-256 checksums are provided.

For an upgrade, quit PC Hub from the tray, install the new `.deb`, and reopen it. Reinstalling or uninstalling preserves user data. Back up commissioned hub data before a downgrade.

Windows and macOS installers are not publicly released yet.

This repository contains public installers and release documentation. Application source and credentials are maintained separately.
