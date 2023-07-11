---
title: Feral Essence
summary: Adds two items ("Bestial Essence" and "Anthro Essence") which transform characters into ferals and anthros.
downloads:
  - name: Feral.Essence.v1.0.zip
    url: https://github.com/NoHornyOnMain/lt-mods/releases/download/feral-essence-v1.0/Feral.Essence.v1.0.zip
images:
  - source: /images/mods/liliths-throne/feral-essence/001.png
---
# Things to Note
- Ferals are ***not*** fully implemented into the game yet. They are broadly speaking functional, but you use them at your own risk.
- Both essences are sold at Roxy's shop in the Gambling Den down in Submission; they can also be found randomly in Submission and Dominion's alleyways.
- Ferals cannot be mixed race (this is a game limitation).
    - Any parts that are not of the character's primary race will be converted to that race when becoming feral.
    - Any parts the target feral race can't have (wings, horns, etc.) will be removed.
- Similar to normal TF items, I've stopped the essences from working on unique characters by default due to potential bugginess.
    - If you want to override this, change the `#IF(!npc.isUnique() || npc.isPlayer())` line in each item's XML file to read `#IF(true)`
- When turning a feral into an anthro, they will always become a greater morph of the applicable race.

# Known Issues
- Specific attributes (size, colour, etc.) of most body parts are re-generated when transforming from anthro to feral (and vice versa).
    - The presence of body parts seems to stay consistent (unless the target feral race doesn't have that part; see Things to Note).
    - Subspecies requirements are retained (e.g. an arctic wolf morph will still have white fur after either transformation).
- All virginities will be partially reset when transforming from anthro to feral (and vice versa).
    - It seems that the game remembers *how* the virginities were lost, but resets that they *have* been lost. As such, when the virginity is lost again the original message will re-appear.
