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

`latest.zip` is the packaged build Dalamud downloads. To publish a new version:

1. Rebuild the plugin in Release/x64 (produces a fresh `latest.zip`).
2. Bump `<Version>` in the project and `AssemblyVersion` in `pluginmaster.json`.
3. Replace `plugins/Tan_Auto_Retainer/latest.zip` with the new build.
4. Commit and push.

## Source & License

This plugin embeds AGPL-3.0 licensed code from Dagobert. It is therefore distributed
under the **GNU Affero General Public License v3.0** (see `LICENSE.md`).

Full source code: https://github.com/TanYukseloglu/Tan_Plugin
