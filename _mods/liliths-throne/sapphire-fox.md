---
title: Sapphire Fox Hotel & Spa
summary: Adds a hotel in Demon Home called the Sapphire Fox Hotel & Spa.
downloads:
  - name: Sapphire.Fox.Hotel.Spa.v1.0.zip
    url: https://github.com/NoHornyOnMain/lt-mods/releases/download/hotel-v1.0/Sapphire.Fox.Hotel.Spa.v1.0.zip
images:
  - source: /images/mods/liliths-throne/sapphire-fox/001.png
  - source: /images/mods/liliths-throne/sapphire-fox/002.png
  - source: /images/mods/liliths-throne/sapphire-fox/003.png
---
# Things to Note
- Located on the same tile as 'Sawlty Towers' (Arthur's apartment building).
- Requires completion of the 'Demon Home' section of 'The search for Arthur'.
- Slaves assigned to the 'Bedroom' work type will always go to your bedroom in Lilaya's house, not your suite.
    - This is because the job hard-codes the location as being in Lilaya's house, so versions of the room in different places are not considered.
- Slaves assigned to the 'Spa' work types will always go to the spa in Lilaya's house, not the hotel.
    - Similar to the 'Bedroom' work type, the location is hard-coded as being in Lilaya's house.
- If you want to change the price, you'll need to change both instances of '3750000' in `nhom/dialogue/hotel.xml` to your desired value.
    - To make the text match, you'll also need to update `nhom/txt/hotel.xml`.
    - Alternatively, you can give yourself the suite by running `[##player.setAffection("nhom_hotel_has_purchased", 1)]` in the parser.
    - It's also possible to give yourself money via the parser by running something like `[#player.incrementMoney(3750000)]`.

# Known Issues
- If you want to visit Sawlty Towers, it now requires two interactions.
    - `Approach Sawlty Towers` -> `Sawlty Towers`
    - This is a workaround for the fact that the internal dialogue cannot currently be referenced from a mod.
- The hotel is not accessible when leaving Sawlty Towers.
    - As a workaround, simply walk away one tile and walk back.
- Flavour text for the spa and the bedrooms in the player's suite don't make a lot of sense in context.
    - This is because they are re-using the rooms from Lilaya's house, as custom slave rooms cannot yet be added via mods.
- You can fast travel from the bedrooms in the player's suite as if you were in Lilaya's house.
    - This is similarly due to re-using the rooms from Lilaya's house.
- You can't interact with the receptionist after buying the suite.
    - I'm not much of a writer (especially for dialogue) and couldn't think of any useful interactions beyond purchasing the suite.
    - I'll likely come back to this later in some capacity if I feel like having a go at making NPCs.
