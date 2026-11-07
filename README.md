# Winprove

Windows, within reach.

This repository distributes Winprove preview installers, portable packages, and the signed update feed used by Winprove. The main development repository remains private.

## Downloads

Open [Releases](https://github.com/colemclauchlan/Winprove-Updates/releases) for the latest available preview. Setup installs Winprove for the current Windows user; the portable package keeps the app together without a conventional installation.

These are development previews. Update packages and appcasts carry an Ed25519 signature checked against the key bundled in Winprove. Preview installers do not yet carry a production Windows code-signing certificate.

## Updates

A configured preview installation checks this repository anonymously. No GitHub account or token is required. A package must pass Winprove's signature and version checks before Setup can apply it. Winprove preserves preferences, profiles, layouts, and logs when updating.

## Required source and notices

Each release includes its corresponding source archive and required license notices. Those files are part of the distribution; retain them when redistributing packages. Publishing these release sources does not change the visibility of the main development repository.