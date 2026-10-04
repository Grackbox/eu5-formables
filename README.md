# EU5 Formable Nations

An interactive index of every formable nation in Europa Universalis V (game version 1.4): tiers, required territory, who can see and form each nation, the effects of forming it, rank bonuses and its country advances.

**Open it:** https://grackbox.github.io/eu5-formables/

- Filter by tier, rule (historical, plausible, fantasy), continent and features; sort by tier, name, territory size or number of country advances.
- Select a nation to see its description, required lands, conditions, effects and country advances grouped by age.
- Three lists: formable nations, nations that can't be formed (no tier), and cultures. Each nation shows its country advances and state principles; each culture shows its culture advances, the formable nations it can form and the nations that start with it. Formable nations list the cultures they require.
- All game text comes from the game's own localization in its 11 languages. The page opens in your browser's language and remembers your choice.

## Rebuilding after a game patch

Requires Python 3 and a local copy of the game.

```
set EU5_GAME=E:\SteamLibrary\steamapps\common\Europa Universalis V\game
python tools/build.py
```

The script writes `tools/site/pages.html` and `tools/site/data/<language>.json`. Copy `pages.html` to `index.html` and the JSON files to `data/` in the repository root.

## Notes

- This is a fan-made tool and is not affiliated with Paradox Interactive. Game names, text and data belong to Paradox Interactive.
- Location counts leave out seas, lakes and impassable mountains, as the game does.
- The connecting phrases in conditions (for example "Owns location:") are in Russian for the Russian page and in English for the other languages.

Built with Claude (Anthropic).
