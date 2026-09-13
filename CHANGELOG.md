# Changelog

All notable changes to Cringe Dancer. Download the newest version from the
[README](README.md) — the links there always point at the latest release.

## 1.0.0 — 2026-09-13

First full release.

### Fixed
- **Windows: pop-out mode did nothing.** Clicking the pop-out button parked the
  plugin window as expected, but the dancer never appeared on the desktop. He
  was actually there — the window was created fully transparent, so there was
  nothing to see. He now shows up beside the plugin window like on macOS, with
  the desktop showing through around him, and the empty space around him
  still passes clicks through to your DAW.
- **Windows: pop-out controls are easier to hit.** The close X, the
  clubber-switch icon and the resize grip sit on small dark chips, so you can
  click them without aiming at a two-pixel line.

macOS is unchanged from 0.1.6.

## 0.1.6 — 2026-09-05

### Changed
- **Windows installer is now signed.** The installer, the uninstaller and the
  plugin itself carry an EDM GHOST PRODUCTION INC. code signature, so Windows
  names the publisher instead of warning about an unknown one, and SmartScreen
  stays quiet.

### Fixed (Windows installer)
- **Custom install folders now work in every DAW.** FL Studio ignores VST3
  bundles in user-added folders; the installer now links your chosen folder
  into the standard VST3 location, so the files stay where you put them and
  every host still finds the plugin. Nothing to configure.
- **Uninstall works with your DAW still open.** The plugin disappears from the
  host immediately; the one file Windows can't delete while it's loaded is
  cleaned up at the next restart — and the installer no longer demands a
  restart it doesn't need.
- **Reinstalling to a different folder no longer leaves the old copy behind.**
- The uninstaller's own files no longer land in your plugin folder.

## 0.1.5 — 2026-07-18

Pop-out mode polish (macOS and Windows):

- The clubber-switch moved to its own person icon next to the close X.
  Clicking the dancer himself only ever drags him — no more accidental
  switching while moving him around.
- The empty margin around the dancer is click-through, so the pop-out never
  steals a click from your DAW.

Earlier versions (0.1.1–0.1.4) were test builds and are no longer available.
