---
title: "Off to Middle-earth"
description: "You are ready to play for real - time to log into the web client and begin your adventure."
teach:
  - command: "look"
    desc: "inspect your surroundings and client layout"
  - command: "map"
    desc: "view live map orientation"
  - command: "who ranger"
    desc: "find online Rangers dedicated to assisting new players"
steps:
  - story: "As dawn rises over the Black Hills, Fuor prepares to step into Middle-earth!"
  - ask: "look"
    note: "Type `look` to orient yourself in the Web Client interface."
    accept:
      - "look"
      - "l"
    hint: "Type: look"
  - ask: "map"
    note: "Type `map` to examine the live MMapper radar view."
    accept:
      - "map"
      - "m"
    hint: "Type: map"
  - ask: "who ranger"
    note: "MUME Rangers exist specifically to assist new players! Check active Rangers with `who ranger`."
    accept:
      - "who ranger"
      - "who rangers"
      - "who"
    hint: "Type: who ranger"
responses:
  look: "The Foaming Mug's Beer Garden\nA quiet courtyard paved with cobblestones lies behind the tavern.\nExits: south, west.\nRanger Irelm smiles warmly at you.\n\n*+->"
  map: "    #   .   .\n    |   |   |\n  .-*---*---*-.\n    |   |   |\n    #   .   .\n\n*+->"
  who ranger: "Rangers\n-------\n\n0 such allies or visible Ainur on.\n\n*+->"
  who rangers: "Rangers\n-------\n\n0 such allies or visible Ainur on.\n\n*+->"
  who: "Players Online: Fuor, Martyrson, Elrond, Glorfindel.\n\n*+->"
---

# Off to Middle-Earth

That's the basics - you've learned to look, move, examine, gear up, talk, trade, fight, flee, rest, train and rent. When you play for real you'll do it all in the **web client**, with a live map (MMapper) beside the text. You'll start your adventures with **Gandalf** before you find yourself back in Tower Hills, where your life in MUME will begin. Remember - Rangers (who are actual characters) are online to help new players; use `who ranger` to see who is online.
