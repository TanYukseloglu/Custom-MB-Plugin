# Tan_Auto_Retainer — Dalamud Plugin Repository

A Dalamud plugin that runs an AutoRetainer venture cycle and, after each retainer
collects and assigns a quick venture, pinches (undercuts) that retainer's market
board listings using an embedded Dagobert engine — before moving to the next retainer.

**Per-retainer flow:** collect → quick venture → pinch → next retainer.

## Install

1. In-game, open Dalamud settings: `/xlsettings`
2. Go to the **Experimental** tab
3. Under **Custom Plugin Repositories**, paste this URL and click **+**, then **Save**:

   ```
   https://raw.githubusercontent.com/TanYukseloglu/Custom-MB-Plugin/main/pluginmaster.json
   ```

4. Open the plugin installer: `/xlplugins`
5. Search for **Tan_Auto_Retainer** and click **Install**

## Requirements

- **AutoRetainer** installed and enabled, with **Multi-Mode ON**
- Disable the standalone **Dagobert** plugin (pinch is built in here)

## Usage

- `/tanar` — open the main window
- `/tanar config` — open settings

## Updating the plugin

The packaged build (`latest.zip`) is hosted as a **GitHub Release asset**, not committed
in the source tree. To publish a new version:

1. Rebuild the plugin in Release/x64 (produces a fresh `latest.zip`).
2. Bump `<Version>` in the project and `AssemblyVersion` in `pluginmaster.json`.
3. Create a new GitHub Release (e.g. `v0.2.0.0`) and upload the new `latest.zip` as an asset.
4. Update the three `DownloadLink*` URLs in `pluginmaster.json` to the new release tag.
5. Commit and push `pluginmaster.json`.

## Source & License

This plugin embeds AGPL-3.0 licensed code from Dagobert. It is therefore distributed
under the **GNU Affero General Public License v3.0** (see `LICENSE.md`).

Full source code: https://github.com/TanYukseloglu/Tan_Plugin
