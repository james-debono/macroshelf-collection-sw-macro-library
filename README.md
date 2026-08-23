# MacroDeck Collection

Every macro from my SOLIDWORKS projects, packaged together for one-step
installation and arranged the way they should appear on a toolbar.

The macros are ordinary `.swp` files and work on their own. The collection is laid
out as a [MacroDeck](https://github.com/james-debono/macrodeck-sw-addin) library,
which is where the name comes from — point MacroDeck at it and every macro appears
as a toolbar button, already set up.

If you only want one of them, each has its own repository with its source,
changelog and development notes — links below.

Works with SOLIDWORKS 2022, 2024 and 2025.

## What's in it

| Button | Macros | What it does |
|---|---|---|
| **Apply Colours** | 3 | Colours every geometrically unique body so anything different stands out, and clears those colours again |
| **Draw Rounded Rectangle** | 1 | Draws a rounded rectangle into the sketch you have open |
| **Screenshot High Res** | 1 | Exports the current view to an image at any pixel size, with a live preview |
| **Themes** | 5 | Switches the interface and viewport background between light and dark |

## Install

Download the [latest release](../../releases/latest) and unzip it somewhere
permanent — the macros run from where you put them, so a temporary folder is a bad
choice. You get a single `MacroDeck Collection` folder.

**With [MacroDeck](https://github.com/james-debono/macrodeck-sw-addin)** — point it
at the unzipped folder and every macro appears as a toolbar button, with icons and
hover text already set up. Folders holding several macros become drop-downs.

**Without MacroDeck** — the `.swp` files are ordinary SOLIDWORKS macros. Use
**Tools > Customize > Commands > Macro** to put one on a toolbar, or
**Tools > Macro > Run** to run it directly. Each macro folder holds its icon as
`icon.png` and a one-line description.

## Individual repositories

Each holds the readable source, the full changelog, and development notes covering
the SOLIDWORKS API findings behind it.

**Apply Colours**

- [apply-unique-colours-sw-macro](https://github.com/james-debono/apply-unique-colours-sw-macro)
- [remove-body-and-component-appearances-sw-macro](https://github.com/james-debono/remove-body-and-component-appearances-sw-macro)
- [remove-all-appearances-sw-macro](https://github.com/james-debono/remove-all-appearances-sw-macro)

**Sketch**

- [draw-rounded-rectangle-sw-macro](https://github.com/james-debono/draw-rounded-rectangle-sw-macro)

**Export**

- [screenshot-high-res-sw-macro](https://github.com/james-debono/screenshot-high-res-sw-macro)

**Themes**

- [set-ui-theme-dark-sw-macro](https://github.com/james-debono/set-ui-theme-dark-sw-macro)
- [set-ui-theme-light-sw-macro](https://github.com/james-debono/set-ui-theme-light-sw-macro)
- [set-background-colour-dark-sw-macro](https://github.com/james-debono/set-background-colour-dark-sw-macro)
- [set-background-colour-light-sw-macro](https://github.com/james-debono/set-background-colour-light-sw-macro)
- [set-background-scene-sw-macro](https://github.com/james-debono/set-background-scene-sw-macro)

## About this repository

**This repository owns the arrangement; the macros come from elsewhere.**

- The **folder structure, icons and `description.md` files are maintained here.**
  They are what turns a pile of macros into a toolbar: which macros group into a
  drop-down, what that drop-down is called, and what each button shows on hover.
  None of that belongs to any single macro, so it lives here.
- The **`.swp` files are copies**, refreshed from the individual repositories by
  `build-library.ps1`. Don't edit a macro here — fix it in its own repository and
  re-run the script, or the change is lost on the next refresh.

Grouping is deliberately kept separate from the macros themselves. Moving a macro
into a different drop-down, or renaming a drop-down, is a folder change here and
touches nothing else.

Each macro carries its version, author and the full licence text in its own header,
so a `.swp` passed on by itself still says what it is and how it may be used.

## Licence

MIT — see [LICENSE](LICENSE). Free to use, modify and share.

Created by James Debono, with AI assistance. Everything here was tested by
hand in SOLIDWORKS — nothing that touches the API can be verified any other way.

## Trademarks

SOLIDWORKS is a registered trademark of Dassault Systèmes SolidWorks Corporation.
This project is independent: it is not affiliated with, endorsed by, or sponsored
by Dassault Systèmes, and uses only the published SOLIDWORKS API.
