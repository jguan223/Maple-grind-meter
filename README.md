# Maple Grind Meter

A browser overlay for MapleStory Classic that measures EXP and mesos per hour while you train, so you can compare maps. Nothing to install: open the page in Chrome or Edge, share the game window, and press Start.

**Live:** https://jguan223.github.io/Maple-grind-meter/

## What it does
- Reads the EXP / meso / item pickup messages in the bottom-right of the game with in-browser OCR (Tesseract.js). Your screen never leaves your computer.
- Cross-checks EXP against the numbers on the EXP bar and shows a match %.
- Start / Pause / End, an optional training timer with an alarm that ends the session, or no limit.
- Pop-out overlay: a small always-on-top window with totals and Pause/End.
- Kills by monster (solo: matched by each mob's EXP; party: estimates your share, how many people are splitting, and the party bonus).
- Session summary with per-hour and per-30-minute averages, a 30-minute breakdown, kills and drops picked up. Copy, download or share it.
- Ranks the maps you've trained on by EXP/hr, mesos/hr, or both.
- Boxes adjust between fullscreen and windowed; each game size remembers its own layout.
- Low CPU: only the boxed areas are read, and only when they change.

## Tips
- Open **Calibration** to see what the reader sees. Raise or lower *Text brightness cut* until the messages read cleanly.
- The map name is read from the two lines at the top of the minimap (area + map). The map's picture and its monsters (with pictures, best drops and a kill counter) come from the built-in Classic database.
- The EXP bar (e.g. `EXP 88,666 [4.78%]`) is read every 3 seconds; when it can be read, EXP totals come from the bar, which is exact.
- Drag the middle of a box to move it, any corner or edge to resize. Press **Save settings for this PC** to keep your layout on that PC; **Copy settings code** moves it to another PC.
- Paste a map's monster table (Monster · Lv · HP · EXP) from its NiaMeowDB page once to get kills per monster by name.

## Credits
Classic map, monster, drop and picture data: [MapleClassic Wiki](https://mapleclassic.wiki), licensed [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/). The overlay downloads it once into your browser as its own database (Update database refreshes it). Map links: [NiaMeowDB](https://meowdb.com/msclassic). Party EXP formula as published on NiaMeowDB (credit ohmi + azzybish). OCR: [Tesseract.js](https://github.com/naptha/tesseract.js).
