---
title: Race Icon Tattoos
summary: Adds a total of 50 tattoos, one for each race (and subspecies) in the base-game that has an icon stored in the res folder. It uses these icons directly from the res folder, so it requires no extra .svg files and only takes up ~28KB of storage.
changelogs:
  - version: 1.1
    changes:
        - "Updated the imageName paths to utilise the new SVG functionality in 0.4.7."
        - "Corrected the name and path of the 'canine paw' tattoo."
downloads:
  - name: Race.Icon.Tattoos.v1.1.zip
    url: https://github.com/NoHornyOnMain/lt-mods/releases/download/race-icon-tattoos-v1.1/Race.Icon.Tattoos.v1.1.zip
  - name: Race.Icon.Tattoos.v1.0.zip
    url: https://github.com/NoHornyOnMain/lt-mods/releases/download/race-icon-tattoos-v1.0/Race.Icon.Tattoos.v1.0.zip
images:
  - source: /images/mods/liliths-throne/race-icon-tattoos/001.png
---
# Things to Note
Version 1.1+ of the mod requires version 0.4.7 of the game or newer. If you're on an older game version, download version 1.0 instead.

Whilst every single base-game race (at time of creation) that has an icon stored in the res folder is included, some are disabled by default to not unnecessarily crowd the tattoo screen. Specifically, the disabled tattoos (and why they are disabled) are as follows:
- Dog: The icon is already used by the base-game 'paw-print' tattoo.
- Horse: The icon is already used by the base-game 'horse-shoe' tattoo.
- Snow Leopard: The icon is identical to that used by leopards.
- Bald Eagle: I encountered issues colouring this tattoo and, other than having an extra colour for the beak, it's essentially the same as the regular eagle icon.

If you wish to enable any of these tattoos, open the corresponding .xml file (e.g. 'dog.xml') and replace this line:
`<availabilityRequirements unique="true"><![CDATA[false]]></availabilityRequirements>`
With this:
`<availabilityRequirements/>`

Similarly, if you wish to disable any of the tattoos without deleting the file, you can replace the latter line with the former in any given file.
