# aMAG 1.0

Open **aMAG-1.0.exe** to run. Close any older copy first. The app starts with magnification off.

Your current settings have been copied into `preferences.txt`, including zoom, dock placement, shortcuts, and panel opacity. Keep that file beside the executable to retain them. The previous development folder has been left in place.

- **Dock, Lens, Screen:** select the view in the controls.
- **Ctrl+Alt+A:** toggle magnification.
- **Ctrl + wheel-button press:** toggle; ordinary wheel-button panning stays available.
- **Ctrl+Alt+F9 / F10:** decrease / increase zoom.
- **Ctrl+Alt+F7:** switch views.
- **Ctrl+Alt+F6:** emergency off.

Keyboard and mouse bindings can be changed in the controls. Zoom supports **100%–1600%**. The dock remembers its size and position; unlock its layout to move, resize, or use Windows Snap Layouts. The picture areas let you interact with the apps underneath. Follow typing and Smooth motion remain available. Panel opacity affects only the controls.

## Folder contents

| Item | Purpose |
| --- | --- |
| `aMAG-1.0.exe` | Ready-to-run 64-bit Windows application |
| `preferences.txt` | Your copied settings; updated by the app |
| `Build` | Complete 1.0 C# source, icon, manifest, and build/verification scripts |
| `Validation` | Release review and fresh verification results |
| `SHA256SUMS.txt` | Checksums for the executable and fixed release/build files |

To rebuild, see `Build/README.md`. No additional packages or Windows updates are required by this release. Use a writable folder so the app can save its preferences and diagnostics.

## Supported scope

This release targets the normal desktop on 64-bit Windows 11, with non-rotated displays. Windows sign-in/UAC secure desktops and protected content are subject to Windows capture restrictions. Display/session/power changes stop magnification; toggle on again when ready. Caret tracking depends on the app's accessibility support. The dock is an always-on-top window and does not reserve desktop workspace.

1.0 preserves the accepted 0.11 magnifier behavior. Release changes are version metadata, packaging, documentation, and replacing the old inconclusive capture diagnostic with the validated separate-process underlay check. Automated checks establish geometry, rendering, interaction routing, and persistence; they do not guarantee a frame rate or identical behavior in every application's custom graphics/editor controls.
