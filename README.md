# Resona

**A Roon remote for Linux.**

Resona controls an existing Roon Server on your network from a native Linux desktop app. This repository hosts public alpha releases and user documentation.

## Download

[View Linux x86_64 releases](https://github.com/Tante-Diazepam/Resona/releases)

If no release is listed, the installer has not been published yet. The files below describe the planned v0.8.0-alpha.5 release.

Choose one of these files from the release's **Assets** section:

| File | Use |
| --- | --- |
| `Install-Resona-0.8.0-alpha.5-x86_64.run` | Graphical installer with an application-menu shortcut. |
| `Resona-0.8.0-alpha.5-x86_64.AppImage` | Run Resona directly without installing it. |
| `SHA256SUMS` | Verify your download. |

This is an early alpha for Linux x86_64. It has been tested locally on Fedora; compatibility with other distributions has not yet been verified.

## Install

1. Download the `.run` installer.
2. Open its file properties and allow execution if your desktop requires it.
3. Run the file, choose English if needed, then select **Install Resona** and **Start Resona**.

Installation is for your user account and does not require administrator privileges.

From a terminal, in your download directory:

```bash
chmod +x Install-Resona-0.8.0-alpha.5-x86_64.run
./Install-Resona-0.8.0-alpha.5-x86_64.run
```

For the portable AppImage:

```bash
chmod +x Resona-0.8.0-alpha.5-x86_64.AppImage
./Resona-0.8.0-alpha.5-x86_64.AppImage --appimage-extract-and-run
```

## Connect to Roon

1. Start Resona and select your Roon Server. You can enter its address manually if discovery does not find it.
2. In an official Roon app, open **Settings → Extensions** and enable **Resona**.
3. Select a playback zone in Resona.

The interface supports English and Norwegian. Change the language and theme in **Settings**.

## What the alpha includes

- Album, artist and playlist browsing through Roon.
- Playback controls, seeking, volume, shuffle and repeat where supported by the selected zone.
- An automatically updating queue with playback from a selected queue item.
- Album artwork, audio-format information and a signal-path view.
- A window that remembers its size, light and dark themes, and expandable artist and album introductions.

Album availability, metadata and supported controls depend on your Roon Server and connected services. Some views and controls remain incomplete. Resona is an independent community project, not an official Roon application.

## Updates and removal

Close Resona, run the newer installer and choose its reinstall/update option. Installation management is also available from **Settings** and the application-menu shortcut. Settings, Roon authorization and the artwork cache are retained when uninstalling.

## Verify downloads

Download `SHA256SUMS` alongside both release files, then run:

```bash
sha256sum --check SHA256SUMS
```

If you downloaded only one of the two release files, its matching entry can be checked with:

```bash
sha256sum --check --ignore-missing SHA256SUMS
```

## Feedback

[Report an issue](https://github.com/Tante-Diazepam/Resona/issues) with your Resona version, Linux distribution, desktop environment, and the steps needed to reproduce the problem. Please remove access tokens, server addresses and personal music information from logs and screenshots before sharing them publicly.

Resona is distributed under the [MIT license](LICENSE). Third-party notices are included in the application package.
