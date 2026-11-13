# Dungeon Crawler — Enhanced Edition

A browser game inspired by Matt Dinniman's *Dungeon Crawler Carl*. It started as a short Twine (Harlowe) story; this version rebuilds it as a full dungeon crawler in a single `index.html` file. No build step, frameworks or downloads are needed.

> Unofficial, non-commercial fan project for a Digital Humanities course. *Dungeon Crawler Carl* and its characters belong to Matt Dinniman.

## Play

Open `index.html` in any modern browser, or publish the repository with GitHub Pages (see below).

## What's in it

The original Twine story had about 15 passages, one item choice and a fixed HP value. The enhanced version keeps that story's opening, choices, jokes and endings, and builds a game around them.

| | Original Twine | Enhanced |
|---|---|---|
| Floors | Floor 1 only, as text | 5 generated floors with fog-of-war maps |
| Stats | HP | STR, CON, DEX, INT, CHA, plus HP, MP, XP and levels |
| Items | Snacks or a machete | 69 items: gear for six slots, consumables, explosives, crafting materials, skill scrolls |
| Skills | None | 20 skills, including class skills and passives |
| Enemies | Goblins | 39 monster types, 8 Neighborhood Bosses, the Rage Elemental, 4 Floor Guardians and 4 castle lords |
| Achievements | None | 45, most with a loot box reward, all with System AI commentary |
| Endings | A handful | 16 endings, tracked across playthroughs |

### Floors (following the books)

1. **The First Floor** has corridors, goblins, rats and cockroach swarms. You must find the **Tutorial Guild** before you can descend. The Neighborhood Bosses are **The Hoarder**, who retches cockroaches, and a goblin steam machine.
2. **The Second Floor** has bigger neighborhoods, kobolds and gnolls. Other things you'll run into here:
   - The **Krakaren Clone** and the **Rage Elemental** (you can lure it into a stairwell for *Experience Denied*).
   - **Prince Maestro's** game show and the player killers **Frank Q & Maggie My**.
   - **Team Meadow Lark**, who help you against **The Ball of Swine** if you helped them earlier.
   - A boss chamber with a pet to hatch.
3. **The Over City** is where you choose your **race and class** (Primal, Compensated Anarchist, Former Child Actor and more). Circus monsters fill the streets, and the boss is **Grimaldi**, the vine-possessed ringmaster.
4. **The Iron Tangle** is a subway maze with no map. You ride trains between platforms, dodge Jikininki, and face bounty hunters if you make the Top Ten.
5. **The Bubbles** has four castles (Land, Sea, Air and Subterranean). Capture all four to open the final stairwell, with 15 days on the clock.

### Systems

- **Collapse timer:** every floor collapses. Moving, resting and searching all cost time.
- **Combat:** turn-based fights against groups. You can target enemies, use skills with cooldowns, throw explosives, play to the crowd, or run for your life.
- **Loot boxes:** Bronze, Silver, Gold, Platinum, Legendary and Celestial, in Adventurer, Fan, Boss, Explosives and Pet varieties. You can only open them in safe rooms.
- **Viewers and sponsors:** being entertaining earns Fan Boxes, sponsor gifts and a spot on the **Top Ten leaderboard**.
- **Safe rooms and Mordecai's guild:** rest, shop, craft (including a *Jug O' Boom*), train skills and save checkpoints.
- **Achievements:** each one comes with commentary from the dungeon's System AI.
- **Odette's talk show:** an interview between floors.
- **Pets:** pets fight beside you. Feed one an *Enhanced Pet Biscuit* and it learns to talk.

### Controls

- **Move:** arrow keys or WASD, the on-screen d-pad, or click a neighboring room on the map.
- **Choices:** number keys 1–9.
- **Windows:** **I** inventory, **C** character, **B** loot boxes, **M** menu, **Esc** close.

Progress autosaves in your browser (localStorage). Checkpoints are made at safe rooms, guilds and the start of each floor.

## Publishing with GitHub Pages

1. Create a new repository on GitHub, then push this one to it:
   ```bash
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
   ```
2. On GitHub, open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**, then select `main` and `/ (root)`.
4. The game will be live at `https://<your-username>.github.io/<repo-name>/` within a minute or two.

## Repository layout

```
index.html          The whole game: HTML, CSS and JavaScript in one file
Reference/          The original Twine project (.twee source and exported .html)
README.md
```

## Sources

The book details came from plot summaries and reader notes, including:

- [Books That Slay: *Dungeon Crawler Carl* summary](https://booksthatslay.com/dungeon-crawler-carl-summary-characters-and-themes/)
- [Books of Brilliance: Book 1 recap](https://booksofbrilliance.com/2026/11/09/dungeon-crawler-carl-book-1-recap/)
- Goodreads reader notes, for the loot box tiers and the Krakaren Clone
- Publisher and review summaries of the later books, for the Over City, the Iron Tangle and the Bubbles

All in-game writing is original, apart from lines carried over from the original Twine story.
