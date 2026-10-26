# Resona v0.8.0-alpha.5

An early Linux x86_64 alpha of Resona, a desktop remote for an existing Roon Server.

## Included in this build

- Browse albums, artists and playlists, with album cards following their Roon Browse references.
- Control playback and volume in the selected zone, with seeking, shuffle and repeat where supported.
- View a queue that updates automatically and retries after temporary read errors.
- See artwork, audio-format details and the reported signal path.
- Restore the previous window size and use a Now Playing layout that adapts to the available height.
- Read longer artist and album introductions in a separate window using **Show more**.
- Use English or Norwegian, with light and dark themes.

## Downloads

- **Graphical installer:** `Install-Resona-0.8.0-alpha.5-x86_64.run`
- **Portable app:** `Resona-0.8.0-alpha.5-x86_64.AppImage`
- **Checksums:** `SHA256SUMS`

Close any running copy of Resona before installing this build. On first connection, enable Resona under **Settings → Extensions** in an official Roon app.

## Alpha limitations

This build has been tested locally on Fedora. Other Linux distributions have not yet been verified. Some browsing and playback capabilities remain incomplete and depend on what the connected Roon Server exposes. Please report reproducible problems through this repository's Issues page.

Local checks for the underlying development snapshot included 155 GUI tests, 17 packaging tests, formatting and compilation checks. Fourteen network/socket tests could not run in the restricted development environment. These checks do not replace testing against real Roon systems.
