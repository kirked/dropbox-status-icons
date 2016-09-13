An Inkscape document containing Dropbox status bar icons for Gnome on HiDPI displays (48px).

The Dropbox icon itself was downloaded from https://dropbox.com/branding, and the status badges were added as layers using colors I chose, and Unicode characters in the Clear Sans Bold font.

### Generate
To generate the icons, open the file in Inkscape, and selectively hide layers to generate the needed files:

| File                    | Layers               |
| ----------------------- | -------------------- |
| dropboxstatus-logo.png  | dropbox_glyph        |
| dropboxstatus-idle.png  | dropbox_glyph, idle  |
| dropboxstatus-x.png     | dropbox_glyph, x     |
| dropboxstatus-busy.png  | dropbox_glyph, busy  |
| dropboxstatus-busy2.png | dropbox_glyph, busy2 |

Export each combination with the given names above.

### Install

The icons are installed at `~/.dropbox-dist/dropbox-lnx.x86_64-{VERSION}/images/hicolor/16x16/status`. Rename that directory and create a new `status` directory to place your new icons in. Then, copy (or link) the `dropboxstatus-blank.png` image from the old status directory to the new one.

----------
License: MIT <small>(with the additional restrictions that Dropbox places on using their logo at https://dropbox.com/branding)</small>
