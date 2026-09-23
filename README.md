# Trials Ascension

**Current public/source version:** `2.3.4.27`  
**Developer / maintainer:** **Jam4_**

Trials Ascension is an **independent roguelike overhaul for Baldur's Gate 3**.

It is built on the GPL-licensed foundations of **Trials of Tav** and **Trials of Tav Reloaded**, but follows its own gameplay direction focused on long-term roguelike progression, scaling difficulty, Ascension systems, contracts, milestone encounters, custom rewards, equipment progression and replayability.

## Current development changes — V9H test branch

The current development build includes a major custom-weapon pass and loot cleanup. This is **development/test information** and does not replace the public `2.3.4.27` source snapshot linked below.

- Mythic weapons are restricted to the dedicated Mythic reward pool.
- Mythic weapon pool currently includes **Hallebarde du Zénith**, **Trident de la Marée Funèbre**, **Faux de Myrkul** and **Arc du Néant de Dakousai**.
- High-tier item prices are standardized at **900 gp (Very Rare/Epic)**, **1,800 gp (Legendary)** and **3,000 gp (Mythic)**.
- **Arc du Néant de Dakousai** now uses the native Bow of the Banshee weapon base/behaviour while keeping its Trials Ascension spell and bonus package; a permanent Necrotic weapon VFX was added.
- **Lame de Yurgir** uses its native Orthon weapon handling/animation path instead of forced humanoid greatsword animation metadata.
- **Fléau du Vortex** no longer uses the problematic Electrified Flail/Thunderous Smite action. It uses native weapon actions including Concussive Smash and Weakening Strike, alongside its validated defensive bonuses.
- **KatanaTheus** no longer displays the duplicate +2 Dexterity line.
- The non-functional Destructive Wave: Necrotic grant was removed from **Faux de Myrkul**; its other validated bonuses remain.
- **Creuset de l'Alchimiste** and **Espadon du Guetteur** were removed from the active custom-weapon set.
- French, English and Chinese localization files are maintained for the current development content; the full-mod Chinese localization is still being audited before being declared 100% complete.

## Project independence

Trials Ascension is independently developed, maintained, balanced and supported by **Jam4_**.

It is built upon the work of:

- **Trials of Tav** — Hippo0o
- **Trials of Tav Reloaded** — celerev

**Hippo0o and celerev are not involved in the development, maintenance, balancing, support or direction of Trials Ascension.**

Please do not contact them for Trials Ascension support, bug reports or compatibility questions.

## Source code

The corresponding source snapshot for version **2.3.4.27** is available directly in this repository:

**[Download the 2.3.4.27 source archive](./TrialsAscension_Source_2.3.4.27_GitHub.zip)**

Archive SHA-256:

`0cd0ebaeeeda4b66cbbccaaa6da37e1fb1f6ae57cb2d3d9372c53edd870a2b68`

The archive contains the unpacked mod workspace, including the `Mods`, `Public`, `Localization` and Script Extender source used to build the published `CombatMod.pak`.

The internal package/module name remains **CombatMod** for compatibility reasons.

## Building the PAK

Use a BG3-compatible version of **LSLib / Divine ExportTool**.

Example:

```text
Divine.exe -g bg3 -a create-package -s "<source>\src\CombatMod" -d "CombatMod.pak" -c lz4hc
```

## Required external dependencies

These projects must be installed separately:

- **ImprovedUI / ImpUI**
- **UnlockLevelCurve**
- **AdvancedTabletopSpells**
- **BG3 Script Extender**

Optional integration:

- **Spells of Exandria**

**AdvancedTabletopSpells and Spells of Exandria are separate external projects. Their content is not part of Trials Ascension and is not redistributed in this repository.**

## Recommended player load order

1. ImprovedUI
2. UnlockLevelCurve
3. AdvancedTabletopSpells
4. Trials Ascension

Do **not** install Trials of Tav or Trials of Tav Reloaded alongside Trials Ascension.

## Localization

Current in-game languages:

- English
- French

## License

Trials Ascension contains modified code derived from the GPL-licensed Trials codebase. GPL-covered code and modifications are distributed under the **GNU General Public License v3.0**.

See [LICENSE](./LICENSE) and [CREDITS_AND_LICENSE.txt](./CREDITS_AND_LICENSE.txt).

Third-party assets, Baldur's Gate 3 content and external dependencies remain subject to their respective rights and licenses.

Baldur's Gate 3 and related intellectual property belong to their respective rights holders. Trials Ascension is an unofficial community project.
