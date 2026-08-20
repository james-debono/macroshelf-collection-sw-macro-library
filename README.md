# MacroDeck Collection

Every macro from my SOLIDWORKS projects, packaged together for one-step
installation. If you only want one of them, each has its own repository with its
source, changelog and development notes — links below.

The macros are ordinary `.swp` files and work on their own. The collection is
arranged as a [MacroDeck](https://github.com/james-debono/macrodeck-sw-addin)
library, which is where the name comes from — point MacroDeck at it and every
macro appears as a toolbar button, already set up.

Works with SOLIDWORKS 2022, 2024 and 2025.

## What's in it

| Button | Macros | What it does |
|---|---|---|
| **Apply Colours** | 3 | Colours every geometrically unique body so anything different stands out, and clears those colours again |
| **Draw Squound** | 1 | Draws a rounded rectangle into the sketch you have open |
| **Screenshot HD** | 1 | Exports the current view to a PNG at any pixel size, with a live preview |
| **Themes** | 5 | Switches the interface and viewport background between light and dark |

## Install

Download the [latest release](../../releases/latest) and unzip it somewhere
permanent — the macros run from where you put them, so a temporary folder is a bad
choice.

**With [MacroDeck](https://github.com/james-debono/macrodeck-sw-addin)** — point it at the
unzipped folder and every macro appears as a toolbar button, with icons and hover
text already set up. Folders holding several macros become drop-downs.

**Without MacroDeck** — the `.swp` files are ordinary SOLIDWORKS macros. Use
**Tools > Customize > Commands > Macro** to put one on a toolbar, or
**Tools > Macro > Run** to run it directly. Each macro folder holds its icon as
`icon.png` and a one-line description.

## Individual repositories

Each of these holds the readable source, the full changelog, and development notes
covering the SOLIDWORKS API findings behind it:

- [apply-colours-sw-macro](https://github.com/james-debono/apply-colours-sw-macro)
- [draw-squound-sw-macro](https://github.com/james-debono/draw-squound-sw-macro)
- [screenshot-hd-sw-macro](https://github.com/james-debono/screenshot-hd-sw-macro)
- [themes-sw-macro](https://github.com/james-debono/themes-sw-macro)

## About this repository

**The contents are generated.** Every file here is copied from one of the project
repositories above by a build script, so that this collection can never drift from
the individual projects. Fixes and changes belong in the project repository, not
here.

Each macro carries its version, author and the full licence text in its own header,
so a `.swp` passed on by itself still says what it is and how it may be used.

## Licence

MIT — see [LICENSE](LICENSE). Free to use, modify and share.

Written by James Debono.

## Trademarks

SOLIDWORKS is a registered trademark of Dassault Systèmes SolidWorks Corporation.
This project is independent: it is not affiliated with, endorsed by, or sponsored
by Dassault Systèmes, and uses only the published SOLIDWORKS API.
