# Evidence for the status bar focus / alignment pull requests

Captured on a Sony Bravia XBR-49X800E (Android TV 9, 1920x1080, 2 px/dp) over adb
`screencap`, cropped and scaled 2x. Top half of each frame is before, bottom half after.

- `focus-shift-before-after.gif` / `focus-shift-frames.png` — focus stepping
  Settings > Inputs > Wi-Fi. Dashed guides mark the icon positions after the fix.
- `gear-alignment-before-after.gif` / `gear-alignment-frames.png` — settings glyph
  vs the left edge of the first app tile (dashed guide), gear unfocused and focused.

This branch holds only these assets and is not meant to be merged.

- `hidden-apps-icons-before-after.gif` / `.mp4` / `hidden-apps-icons-frames.png` — Settings >
  Applications, hiding three apps in a row on the Android TV emulator (API 36, 4K). Left/before:
  icons stay behind while names shift. Right/after: rows keyed by package.
- `new-app-sort-before-after.gif` / `new-app-sort-frames.png` — installing an app while the
  TV Apps section is sorted alphabetically. Before: appended at the end. After: sorted into place.
- `issue128-back-screensaver.gif` / `.mp4` — Back set to Show screensaver, on the Android TV
  emulator (API 36). Left/before: nothing happens. Right/after: the screensaver starts.
- `sony-screensaver-settings-before-after.png` — Display & Screensaver > Screensaver Settings on
  the Bravia. Before: Sony's top-level Settings. After: Sony's Screen saver page. Account and
  Wi-Fi names are blanked out.
- `new-section-before-after.gif` / `.mp4` — Settings > Interface > Sections > Add section, a
  Games category, Save, on the Android TV emulator (API 36, release builds on #151's toolchain).
  Before: the form stays with Save greyed out, then turns into "Modify section", whose Delete does
  nothing. After: back on the Sections list with the new section.
