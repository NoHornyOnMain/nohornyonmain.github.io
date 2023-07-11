---
title: Player-Owned Stable
summary: Adds a stable with functional slave rooms that can be purchased and used by the player.
changelogs:
  - version: 1.1
    changes:
        - "Changed the requirements for the override, allowing base game encounters at Lilaya's house to trigger normally."
downloads:
  - name: Player-Owned.Stable.v1.1.zip
    url: https://github.com/NoHornyOnMain/lt-mods/releases/download/player-owned-stable-v1.1/Player-Owned.Stable.v1.1.zip
  - name: Player-Owned.Stable.v1.0.zip
    url: https://github.com/NoHornyOnMain/lt-mods/releases/download/player-owned-stable-v1.0/Player-Owned.Stable.v1.0.zip
images:
  - source: /images/mods/liliths-throne/player-owned-stable/001.png
---
# Things to Note
- Uses the existing Dungeon Cell and Ground Floor Window slave room types.
    - These can be changed in `nhom/maps/stable/worldType.xml`.
    - It doesn't seem possible to add new slave room types externally at this time.
- Costs 250,000 flames to purchase.
    - If you want to change the price, you'll need to change both instances of `250000` in `nhom/dialogue/stable.xml` to your desired value. To make the text match, you'll also need to update `nhom/txt/stable.xml`.
    - You can also just give yourself the stable by running `[##player.setAffection("nhom_stable_has_purchased", 1)]` in the parser.

# Known Issues
- Currently not accessible when exiting Lilaya's house (move away and then back).
- The override encounter 'follows' the player off the Lilaya's house tile.
    - This is ultimately harmless, but very much unintentional and can cause a lot of errors to appear in the log.
