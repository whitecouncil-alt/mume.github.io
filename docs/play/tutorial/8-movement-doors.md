---
title: "Movement & Doors"
description: "Practise moving between rooms with compass directions, and opening closed doors."
map:
  img: /assets/images/tutorial-maps/market-square.jpg
  label: "Around the village"
teach:
  - command: "east"
    desc: "step east into the Beer Garden"
  - command: "south"
    desc: "step south into the Stables"
  - command: "west"
    desc: "step west into the Market Square"
  - command: "open west"
    desc: "open a closed door (exits shown as =west= are shut)"
  - command: "north"
    desc: "step north, back to the Common Room"
steps:
  - ask: "east"
    note: "Leave the inn: type `east` (or `e`) to step out into The Foaming Mug's Beer Garden."
    accept:
      - "east"
      - "e"
    hint: "Type: east (or e)"
  - story: "Fuor steps out among the wooden tables, the smell of ale giving way to fresh morning air."
  - ask: "south"
    note: "From the garden, go `south` (or `s`) to the Black Hill Stables."
    accept:
      - "south"
      - "s"
    hint: "Type: south (or s)"
  - ask: "west"
    note: "From the stables, head `west` (or `w`) into the Black Hill Market Square."
    accept:
      - "west"
      - "w"
    hint: "Type: west (or w)"
  - ask: "open west"
    note: "Some exits are closed doors, shown in the exit list like `=west=`. Open one before you can pass with `open <direction>` - try `open west`."
    accept:
      - "open west"
      - "open door"
    hint: "Type: open west"
  - ask: "north"
    note: "Head `north` (or `n`) to return to the Common Room where you started."
    accept:
      - "north"
      - "n"
    hint: "Type: north (or n)"
responses:
  east: |
    The Foaming Mug's Beer Garden
    Wooden tables have been set on the grass in this garden allowing those staying
    at the inn to eat and drink outdoors when the weather permits. Faint sounds of
    horses neighing and whinnying can be heard from the stables to the south.
    A circular stone well has been built here.
    Exits: south, west.

    !.*>
  e: |
    The Foaming Mug's Beer Garden
    Exits: south, west.

    !.*>
  south: |
    Black Hill Stables
    Narrow wooden stalls filled with fresh-cut hay provide basic but comfortable
    accommodation for horses and mules of all kinds. A ladder leads up to the loft.
    A long water trough made of wood stands here.
    A rather dirty young boy is here, ready to tend to the stable.
    Exits: north, east, west.

    ![>
  s: |
    Black Hill Stables
    Exits: north, east, west.

    ![>
  west: |
    Black Hill Market Square
    This is the heart and centre of the village. Many residents crowd the square,
    talking and laughing as they go about their business. A small market has been
    set up here specialising in vegetables and other local produce. A large
    building with a frothing-beer-mug sign dominates the northern side.
    Maelton, village elder of Black Hill, stands here watching the goings-on.
    Exits: north, east, south, =west=.

    !+*>
  w: |
    Black Hill Market Square
    Exits: north, east, south, =west=.

    !+*>
  open west: |
    You open the door to the west.

    !+*>
  open door: |
    You open the door to the west.

    !+*>
  north: |
    Common Room of The Foaming Mug
    A large stone fireplace with a roaring fire warms the room.
    A bartender watches you calmly, while wiping ale mugs with a grimy cloth.
    Exits: north, east, south, up.

    ![>
  n: |
    Common Room of The Foaming Mug
    Exits: north, east, south, up.

    ![>
---

# Stepping out into the Village

Fuor leaves the inn to explore Black Hill. You move between rooms with compass directions - `north`, `south`, `east`, `west` (and `up` / `down`). Some exits are closed doors, shown in the exit list like `=west=`; open them with `open <direction>` before you pass through.
