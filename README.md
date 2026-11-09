# Winprove

Winprove is a Windows app for installing software, customizing Windows, monitoring your PC and running desktop and taskbar widgets.

This repository contains the installer, portable packages and update feed. The development repository is private.

## Downloads

Download the installer or portable ZIP from [Releases](https://github.com/colemclauchlan/Winprove-Updates/releases).

These are **unsigned development previews** for **Windows 10 2004 or later and Windows 11, x64**. The installer doesn't yet have a production Windows signing certificate.

Setup can install for your Windows account or extract a portable copy to a folder. A separate portable ZIP is also available. Portable preferences stay in the adjacent `Data` folder; move it with the app.

The installed app includes a branded uninstaller in Windows Installed Apps. It closes Winprove normally and removes its tracked app files and shortcuts, keeping preferences, profiles, layouts, screenshots and downloads. Setup and removal share the same styling and a wider progress indicator.

## Winprove Bar

Open the Bar from the status pill, tray icon or keyboard shortcut. Pin apps, files, folders and links to the hotbar. Added widgets appear in the sidebar; hotbar pins are configured separately.

**Winprove Bar → Hotbar pins** has compact rows with search, drag reordering, per-pin visibility and shared icon choices. Save up to 16 named pin lists and quick-select one from the card. Lists keep their own order, names, targets, icons and switches; editing the current pins leaves the saved list unchanged until you update it. Undo restores the previous pin/list change. Deleting a saved list leaves the current pins in place.

![Winprove Bar Home](docs/images/bar-home.png)

*These previews use sample data rendered by Winprove's native UI.*

| Tab | Controls |
| --- | --- |
| **Home** | Media, weather, time, quick controls, audio sliders and resource cards. Cards can be rearranged. |
| **Media** | Audio-source selection, artwork, timeline, playback, shuffle/repeat, mixer and output selection. Hover the source selector and scroll to change sources. |
| **System** | CPU, GPU and memory readings, a choice of graph styles and top processes. |
| **Network** | Adapter and IP details, upload/download rates, latency and per-process traffic. |
| **Tools** | A featured Timer or utility, two labeled or four icon shortcuts, power actions and editable utility tiles. |
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

Use **Tools layout** in Bar settings to choose the large card. Keep Timer with custom durations, stopwatch and focus sessions, or choose from 29 tools. Unit Converter, Quick Launch, Reminders, Countdowns and Screenshot Editor join Screenshot, Audio mixer, Calculator, clipboard history and the other utilities. Pins beneath the large card can show two labeled cards or four compact icons. The remaining selected tools stay in the utility grid, without repeating the featured tool or visible pins.

Right-click a tool for its settings or actions. Right-click empty space in the grid to arrange the tools.

<table>
  <tr>
    <td width="50%"><strong>Featured screenshot controls</strong><br /><img src="docs/images/bar-tools-screenshot.png" alt="Featured Screenshot tool with capture choices and editor and settings shortcuts" /></td>
    <td width="50%"><strong>Featured audio mixer</strong><br /><img src="docs/images/bar-tools-mixer.png" alt="Featured Audio mixer with volume and microphone sliders and Apps, Output and Input controls" /></td>
  </tr>
  <tr>
    <td><strong>Two labeled shortcuts</strong><br /><img src="docs/images/bar-tools-pins-labels.png" alt="Two labeled shortcuts beneath the featured tool" /></td>
    <td><strong>Four icon shortcuts</strong><br /><img src="docs/images/bar-tools-pins-icons.png" alt="Four compact icon shortcuts beneath the featured tool" /></td>
  </tr>
</table>

### Bar settings

Settings is always the last icon in the sidebar. Its collapsible groups cover appearance, layout, the status pill, notifications, tools, media and advanced options. Right-click a Home card and choose **Customize** to rearrange cards.

Buttons, icons and menus use matching hover highlights. Long hover explanations wrap to show the full text. Appearance and configuration refreshes keep the current view steady.

**Settings → Appearance** offers Dark, Light, Glass, Custom, Hybrid, ASCII, Matte and Tonal. Matte uses opaque, low-sheen dark surfaces; Tonal uses pale accent-tinted layers. **Saturation** adjusts both the primary and optional secondary accent from 0–200%; 100% preserves the original appearance. Saved colors stay unchanged, and accent-button text adjusts for contrast. Appearance stays synchronized across the hub, Bar and popups.

**Settings → About** uses your accent for the rotating ASCII skull and blinking author cursor. The two icon buttons open the project repository and Cole's portfolio.

![Winprove Bar Settings](docs/images/bar-settings.png)

The status pill can show readings, time and media, with options for persistent visibility, left/right information, hover playback and timer bubbles. More widgets, including calendars, clocks, notes, reminders and Smart Stacks, can be added to the sidebar.

With the Bar along the top edge, double-click its empty top or bottom center to close it. The first click shows a semicircular pulse.

**Gaming mode** on Home uses the same setting as **Settings → Background → Lite mode**. The controller icon expands on hover and stays open with **Enabled** while the mode is on, in both the hub and Bar. It pauses tracking, sensors, traffic capture, automatic scans and update checks, media observation and animated wallpapers, and reduces animations. Turning it off restores your saved choices. Manual tools and enabled Windows mods remain available. Downloads and Windows changes already in progress aren't interrupted.

## Notifications

The hub's bell opens saved notification history, with unread and source filters, mark-read and clear actions. **Off**, **On** and **Do not disturb** control Bar notifications; they don't change Windows notification settings.

The hub’s bell opens notification history. **Notification settings → Set up Windows access** registers the bundled signed identity package, restarts Winprove, then asks Windows for permission. Preview builds need one-time administrator approval for their dedicated certificate in Trusted People; notification registration belongs to your account. Production packages use a trusted publisher certificate. Portable copies leave Windows registration unchanged. No root certificate or Developer Mode change is used.

**Dismiss copied originals** keeps new notifications in Winprove and removes their Windows copy only after it is saved. Existing Windows history stays in place. A Windows banner may appear before the copy is dismissed; notification access does not intercept banners before delivery.

## Screenshots

Screenshot settings include a magnified-reticle switch and an optional step to adjust the selected area before capturing. Drag to move or resize it, then press Enter or double-click to capture.

Turn off **Show options after screenshot** to choose one automatic action: copy to the clipboard, open the default viewer, save to your folder, or upload to Imgur and copy the link. Clipboard-only creates no image file, gallery copy or upload. **Capture region to clipboard only** applies that action once without changing your preferred mode.

![Screenshot output settings](docs/images/screenshot-output.png)

The gallery supports multiple selections and select-all for the visible results. Delete asks for confirmation, then moves the selected files to the Recycle Bin. Favorite changes keep the selection, scroll position and thumbnails in place.

## Widgets

**Unit Converter** covers 13 quantity groups, including length, temperature, speed and data. Choose the units, enter an amount, swap the direction or copy the result. It works in the Bar, taskbar, desktop and Smart Stacks.

<img src="docs/images/unit-converter.png" alt="Unit Converter widget" width="344" />

## Windows Mods and Power tools

**Windows Mods → Taskbar → Taskbar Restart Explorer** adds **Restart Explorer** to the empty taskbar’s right-click menu. It asks the current shell to exit normally and starts it again if Windows has not already done so. If the shell does not close, it leaves it running.

**Windows Mods → Windows → Window pinning** keeps chosen app windows on top. Enable it, then use the recorded shortcut or window picker. App exclusions and a Gaming / Lite pause are in its options. Only windows pinned by Winprove are restored when you disable it or close the app.

<img src="docs/images/window-pinning.png" alt="Window pinning settings" width="500" />

**Windows Mods → Appearance → Automatic Windows theme** switches Windows apps and surfaces between light and dark at your chosen times. The two targets can be selected separately. It starts off and can pause during Gaming / Lite mode. Manual appearance changes stay in place until the next scheduled period.

![Automatic Windows theme settings](docs/images/automatic-windows-theme.png)

**Windows Mods → Power tools → File checksums** calculates SHA-256, SHA-384 or SHA-512 for selected files. Paste an expected checksum or compare two files. Large reads show progress and can be cancelled; leaving the tab cancels the work too. Files are never changed.

![File checksum comparison](docs/images/file-checksums.png)

## FPS display

Add FPS display from Widgets, or enable its corner overlay in Windows Mods. It also works in the Bar, Windows taskbar and on the desktop.

Settings include a program whitelist, persistent display, four screen corners and visibility switches for full-screen apps, the desktop, minimized windows and missing frames. Detailed mode adds frame time, 1% low, CPU, GPU, memory and available temperatures. Capture pauses in Gaming / Lite mode by default.

In **Display → Text only**, the counter draws just the number and **fps** in your accent color on a transparent background. The card, border and hover frame are hidden. Switching it off restores your previous compact or detailed view.

<img src="docs/images/fps-display.png" alt="FPS display with detailed sample readings" width="400" />

FPS counts the app's frame submissions, which can differ from frames shown on screen. Missing readings appear as a dash. Protected games and exclusive full-screen overlay compatibility are still being tested.

## Clean URLs

Find it in **Windows Mods → Privacy → Clean URLs**. Automatic cleaning is off until you enable it. Winprove then cleans plain-text clipboard links before you paste or share them; formatted copies and links typed directly in other apps stay unchanged.

Choose whether to remove campaign tags, advertising IDs and social tracking, unwrap supported redirects, or clean links inside messages. Add excluded domains to leave those sites alone. **Try a link** shows the result before you copy it.

![Clean URLs settings and link preview](docs/images/clean-urls.png)

## Ad blocking

Open **Windows Mods → Privacy → Ad blocking**. The bundled filters cover 6,570 unique domains. Choose ads and common trackers, extra analytics, allowed domains and custom blocked domains. The preview shows the proposed count before you apply changes.

Winprove backs up the hosts file and edits only its own marked rules. Switching the mod off removes those rules. Apps using a separate resolver or proxy can bypass them, and ads on the content's own domain cannot be blocked separately. Restart your browser if cached connections keep using the old rules.

![Ad blocking settings with sample domains](docs/images/ad-blocking.png)

## Telemetry

**Windows Mods → Telemetry** has 25 reviewable controls for diagnostics, advertising, activity history, suggestions and browser reporting. These include Windows Error Reporting and Chrome/Firefox reporting switches. Changes use the same detection, review, apply and undo flow as System Customization.

These controls do not guarantee zero telemetry. Windows Home and Pro can still send required diagnostic data, and required service data is separate.

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
