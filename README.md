# Winprove

Windows, within reach.

This repository distributes Winprove preview installers, portable packages, and the signed update feed used by Winprove. The main development repository remains private.

## Downloads

Open [Releases](https://github.com/colemclauchlan/Winprove-Updates/releases) for the latest available preview. Setup installs Winprove for the current Windows user; the portable package keeps the app together without a conventional installation.

These are development previews. Update packages and appcasts carry an Ed25519 signature checked against the key bundled in Winprove. Preview installers do not yet carry a production Windows code-signing certificate.

## Winprove Bar

Open the Bar from its status pill, tray icon or configurable shortcut. Its sidebar brings media, system readings and everyday tools together; pinned apps, files, folders and links live separately in the hotbar.

![Winprove Bar Home with media, weather, audio and resource cards](docs/images/bar-home.png)

*Interface previews use sample data rendered by Winprove's native UI. Available readings and controls depend on your PC and connected apps.*

| Tab | What's inside |
| --- | --- |
| **Home** | Rearrangeable media, weather/time, quick controls, audio sliders and resource cards. |
| **Media** | Source selection, artwork, timeline, playback, shuffle/repeat, mixer and output selection. |
| **System** | CPU, GPU and memory readings, alternate visualizations and top processes. |
| **Network** | Adapter and IP details, upload/download rates, latency and per-process traffic. |
| **Tools** | Power actions, custom timers, stopwatch, focus sessions and configurable utility tiles. |
| **Shelf** | Files, text and pinned shortcuts, plus clipboard history with search, copy, open and clear actions. |
| **Devices battery** | Supported wireless device readings, display styles, custom names/icons, scanning and visibility controls. |

<table>
  <tr>
    <td width="50%"><strong>Media</strong><br /><a href="docs/images/bar-media.png"><img src="docs/images/bar-media.png" alt="Winprove Bar Media tab with artwork and playback controls" /></a></td>
    <td width="50%"><strong>System</strong><br /><a href="docs/images/bar-system.png"><img src="docs/images/bar-system.png" alt="Winprove Bar System tab with CPU, GPU, memory and top processes" /></a></td>
  </tr>
  <tr>
    <td><strong>Network</strong><br /><a href="docs/images/bar-network.png"><img src="docs/images/bar-network.png" alt="Winprove Bar Network tab with connection details and throughput" /></a></td>
    <td><strong>Tools</strong><br /><a href="docs/images/bar-tools.png"><img src="docs/images/bar-tools.png" alt="Winprove Bar Tools tab with timers and utility tiles" /></a></td>
  </tr>
  <tr>
    <td><strong>Shelf</strong><br /><a href="docs/images/bar-shelf.png"><img src="docs/images/bar-shelf.png" alt="Winprove Bar Shelf tab with sample files, text and pinned items" /></a></td>
    <td><strong>Devices battery</strong><br /><a href="docs/images/bar-devices.png"><img src="docs/images/bar-devices.png" alt="Winprove Bar battery tab with sample wireless device readings" /></a></td>
  </tr>
</table>

### Your layout and appearance

The **Settings** cog stays last in the sidebar. Collapsible settings cards hold the Bar's materials, primary and optional secondary accents, position, screens, media and behavior options. Choose Dark, Light, Glass, Custom, Hybrid or ASCII, and rearrange Home cards through **Customize** in their right-click menu.

![Winprove Bar Settings with shared materials, colors and layout controls](docs/images/bar-settings.png)

Add widgets such as Spotify, Calendar, World Clock, notes, reminders or named Smart Stacks to the sidebar. Choose hotbar shortcuts separately. The **status pill** can show selected readings, time and media, with settings for persistent visibility, hover playback and timer bubbles.

Media controls follow each source's Windows playback capabilities. Battery readings require supported connected devices. Per-process network traffic requires the one-time approved collector setup.

## Updates

A configured preview installation checks this repository anonymously. No GitHub account or token is required. A package must pass Winprove's signature and version checks before Setup can apply it. Winprove preserves preferences, profiles, layouts, and logs when updating.

## Required source and notices

Each release includes its corresponding source archive and required license notices. Those files are part of the distribution; retain them when redistributing packages. Publishing these release sources does not change the visibility of the main development repository.
