# Popout Resizer

Popout Resizer lets you resize Foundry VTT sidebar popout windows, including combat, scenes, actors, journals, items, roll tables, playlists, compendiums, and settings.

This fork is a Foundry V14 compatibility release of Cardagon's original Popout Resizer module.

## Install

Install this fork from Foundry's **Add-on Modules** screen with this manifest URL:

```text
https://github.com/SpencerZPoole/popout-resizer/releases/latest/download/module.json
```

The release zip for this build is:

```text
https://github.com/SpencerZPoole/popout-resizer/releases/download/v1.6.1/module.zip
```

After installation, enable **Popout Resizer** in your world's **Manage Modules** menu.

## Compatibility

- Module version: `1.6.1`
- Foundry minimum: `13`
- Verified with Foundry: `14.362`
- Tested environment: Foundry `14.362` with the D35E system `3.0.2`

This fork is intended to keep the original module behavior while making sidebar popout resizing work with Foundry's V13/V14 application rendering.

## Features

- Adds resize support to Foundry sidebar popouts.
- Supports default sidebar popout width and height settings.
- Can remember sidebar popout size and position between sessions.
- Keeps combat tracker scroll-to-turn behavior when reopening remembered combat popouts.

## Changes In This Fork

### `1.6.1`

- Verified against Foundry `14.362`.
- Updated compatibility metadata for Foundry V14 and removed the stale maximum-version cap.
- Ported the useful V13/ApplicationV2 sidebar popout work from upstream PR [#22](https://github.com/Cardagon/popout-resizer/pull/22), credited to iconmaster5326.
- Added V14-aware `renderApplicationV2` handling for sidebar popouts.
- Uses Foundry's current `foundry.applications.ux.Draggable` class when available.
- Hardened resize setup for missing handles and repeated renders.
- Fixed saved-size setting updates so stored dimensions remain an object.
- Published release assets for direct installation from this public fork.

Upstream pull requests will be proposed after this fork has been locally tested on Foundry V14.

## Credits

Popout Resizer was created by Cardagon. This fork credits iconmaster5326 for the prior V13 sidebar popout work in PR [#22](https://github.com/Cardagon/popout-resizer/pull/22), which informed the V14 compatibility update here.

This compatibility fork preserves the original module id, repository history, and attribution.
