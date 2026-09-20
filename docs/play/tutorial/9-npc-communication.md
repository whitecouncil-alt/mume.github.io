---
title: "NPCs and Player Interaction"
description: "Converse with people in the room and interact directly with tell and follow."
teach:
  - command: "say yes"
    desc: "this is communicated to everyone in the room"
  - command: "tell irelm hello"
    desc: "send a private message to an actual player anywhere"
  - command: "follow irelm"
    desc: "follow a player and join their group"
steps:
  - ask: "say yes"
    note: "Maelton the village elder asks for help. NPCs respond to simple keyword triggers spoken aloud. Type `say yes` to accept."
    accept:
      - "say yes"
      - "say y"
    hint: "Type: say yes"
  - story: "Irelm the Ranger steps out from the shadow of the tavern, adjusting his weathered dark grey cloak."
  - ask: "tell irelm hello"
    note: "Unlike automated NPCs, living players and Rangers engage in rich, freeform communication! Reply to Irelm using `tell irelm hello`."
    accept:
      - "tell irelm hello"
      - "tell irelm"
      - "tell"
    hint: "Type: tell irelm hello"
  - story: "Irelm smiles warmly and unslings his longbow, beckoning Fuor to fall into line."
  - ask: "follow irelm"
    note: "Irelm invites you to join his party. Type `follow irelm` to travel alongside the ranger."
    accept:
      - "follow irelm"
      - "fol irelm"
    hint: "Type: follow irelm"
responses:
  say yes: |
    You say 'yes'
    Maelton the village elder says 'Thank you, Fuor! Please visit the local grocer in the southern shop.'

    Irelm the Ranger steps out from the shadow of the inn, smiling warmly.
    Irelm tells you 'Greetings, young Fuor! Are you ready for the wild?'

    !+*>
  say y: |
    You say 'yes'

    Maelton the village elder says 'Thank you, Fuor!'

    Irelm tells you 'Greetings, young Fuor! Are you ready for the wild?'

    !+*>
  tell irelm hello: |
    You tell Irelm 'hello'

    Irelm tells you 'Follow me, young Fuor! I shall guide you through the hills.'

    !+*>
  tell irelm: |
    You tell Irelm 'hello'

    Irelm tells you 'Follow me, young Fuor! I shall guide you through the hills.'

    !+*>
  tell: |
    You tell Irelm 'hello'

    Irelm tells you 'Follow me, young Fuor! I shall guide you through the hills.'

    !+*>
  follow irelm: |
    You now follow Irelm.
    You are now a member of Irelm's group.

    Irelm says 'Excellent! Together we shall explore the eastern countryside.'

    !+*>
  fol irelm: |
    You now follow Irelm.
    You are now a member of Irelm's group.

    !+*>
---

# Meeting Irelm the Dunadan

In the village Fuor meets two kinds of character. **Non-Player Characters** (game-generated characters, also called "mobs") react to keyword phrases spoken aloud with `say`. **Actual players**, like our example - **Irelm the Dúnadan** - talk freely (`tell irelm hello`) and let you follow him around (`follow irelm`). You can also `group` to ensure that you share experience points during your adventures.
