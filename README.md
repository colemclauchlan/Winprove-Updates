# Winprove

Winprove is a Windows app for installing software, customizing Windows, monitoring your PC and running desktop and taskbar widgets.

This repository contains the installer, portable packages and update feed. The development repository is private.

## Downloads

Download the installer or portable ZIP from [Releases](https://github.com/colemclauchlan/Winprove-Updates/releases).

These are **unsigned development previews** for **Windows 10 2004 or later and Windows 11, x64**. The installer doesn't yet have a production Windows signing certificate.

Setup can install for your Windows account or extract a portable copy to a folder. A separate portable ZIP is also available. Portable preferences stay in the adjacent `Data` folder; move it with the app.

## Winprove Bar

Open the Bar from the status pill, tray icon or keyboard shortcut. Pin apps, files, folders and links to the hotbar. Added widgets appear in the sidebar; hotbar pins are configured separately.

![Winprove Bar Home](docs/images/bar-home.png)

*These previews use sample data rendered by Winprove's native UI.*

| Tab | Controls |
| --- | --- |
| **Home** | Media, weather, time, quick controls, audio sliders and resource cards. Cards can be rearranged. |
| **Media** | Audio-source selection, artwork, timeline, playback, shuffle/repeat, mixer and output selection. |
| **System** | CPU, GPU and memory readings, a choice of graph styles and top processes. |
| **Network** | Adapter and IP details, upload/download rates, latency and per-process traffic. |
| **Tools** | Power actions, custom timers, stopwatch, focus sessions and editable utility tiles. |
| **Shelf** | Files, text, pinned shortcuts and clipboard history, with search, copy, open and clear actions. |
| **Devices battery** | Readings for supported wireless devices, display styles, names, icons, scanning and visibility settings. |

<table>
  <tr>
    <td width="50%"><strong>Media</strong><br /><a href="docs/images/bar-media.png"><img src="docs/images/bar-media.png" alt="Winprove Bar Media tab" /></a></td>
    <td width="50%"><strong>System</strong><br /><a href="docs/images/bar-system.png"><img src="docs/images/bar-system.png" alt="Winprove Bar System tab" /></a></td>
  </tr>
  <tr>
    <td><strong>Network</strong><br /><a href="docs/images/bar-network.png"><img src="docs/images/bar-network.png" alt="Winprove Bar Network tab" /></a></td>
    <td><strong>Tools</strong><br /><a href="docs/images/bar-tools.png"><img src="docs/images/bar-tools.png" alt="Winprove Bar Tools tab" /></a></td>
  </tr>
  <tr>
    <td><strong>Shelf</strong><br /><a href="docs/images/bar-shelf.png"><img src="docs/images/bar-shelf.png" alt="Winprove Bar Shelf tab" /></a></td>
    <td><strong>Devices battery</strong><br /><a href="docs/images/bar-devices.png"><img src="docs/images/bar-devices.png" alt="Winprove Bar Devices battery tab" /></a></td>
  </tr>
</table>

### Bar settings

Settings is always the last icon in the sidebar. Its collapsible groups cover appearance, layout, the status pill, notifications, tools, media and advanced options. Right-click a Home card and choose **Customize** to rearrange cards.

![Winprove Bar Settings](docs/images/bar-settings.png)

The status pill can show readings, time and media, with options for persistent visibility, left/right information, hover playback and timer bubbles. More widgets, including calendars, clocks, notes, reminders and Smart Stacks, can be added to the sidebar.

With the Bar along the top edge, double-click its empty top or bottom center to close it. The first click shows a semicircular pulse.

## FPS display

Add FPS display from Widgets, or enable its corner overlay in Windows Mods. It also works in the Bar, Windows taskbar and on the desktop.

Settings include a program whitelist, persistent display, four screen corners and visibility switches for full-screen apps, the desktop, minimized windows and missing frames. Detailed mode adds frame time, 1% low, CPU, GPU, memory and available temperatures. Capture pauses in Gaming / Lite mode by default.

<img src="docs/images/fps-display.png" alt="FPS display with detailed sample readings" width="400" />

FPS counts the app's frame submissions, which can differ from frames shown on screen. Missing readings appear as a dash. Protected games and exclusive full-screen overlay compatibility are still being tested.

## Compatibility

- Media actions depend on the selected app. Seeking, shuffle and repeat require that app's Windows playback support.
- Battery readings require supported connected devices.
- Per-process traffic requires a one-time administrator-approved collector setup.
- FPS capture may need a one-time Windows approval to set up its bundled collector.

## Updates

Configured preview installations check this repository without a GitHub account or token. Packages must pass signature and version checks before installation. Signatures are verified against the Ed25519 key bundled with Winprove; this is separate from Windows code signing.

Updates keep your preferences, profiles, layouts and logs.

## Required source and notices

Each release includes source archives and required license notices. Keep those files when redistributing packages. Publishing release sources doesn't make the development repository public.
