# BetterEXP

[Thunderstore Page](https://thunderstore.io/c/lethal-company/p/Swaggies/BetterEXP/)

**BetterEXP** is a Lethal Company mod looking to spice up the current experience system in the game. Right now the XP system feels a bit clunky and not a good (enough) measure of a player's true experience working for The Company, so I've created BetterEXP to hopefully make the XP system feel much more satisfying and rewarding/punishing, depending on your actions.

If you would like to help, give ideas, report bugs, or just play Lethal Company with me, you can contact me on Discord `@swaggies`. Shoot me a message anytime and I'll get back as soon as I can!

![Showcase](https://github.com/Swaggies/BetterEXP/blob/main/bxpgif.gif?raw=true)
![Round Summary](https://github.com/Swaggies/BetterEXP/blob/main/bxpimg.png?raw=true)

## End-game Notes
This mod also includes custom player notes! I've changed the way notes are distributed to make sure up to 3 notes can be shown consistently, and also display the corresponding stat for each note (eg. how much scrap the most profitable employee collected). This (hopefully) also fixes some bugs where the Most profitable and Most paranoid stats weren't getting reset after the day ended (somewhat important for this mod).

*Note that this may conflict with mods that also tamper with player notes, I haven't tested compatibilities, report to me on Discord with findings!!*

Here's the list of notes including old and new:
- "The laziest employee" -> **The Laziest**: took the fewest amount of steps.
- "The most paranoid employee" -> **Most Paranoid**: had the most camera turns.
- "Sustained the most injuries" -> **Most Injured**: took the most damage.
- "Most profitable" -> **Most Profitable**: collected the most scrap value.
- **Most Active**: took the most amount of steps.
- **Least Working**: collected the least amount of scrap value.

If any two (or more) players tie on any of these stats, they will all get the note!

## BetterXP System
- You will now gain "BetterXP" (BXP) based on a fixed amount of scrap you get, rather than the percentage of total you can get. This makes going to harder moons net more BXP.
    - Collecting between 0 to 100 scrap awards **0 to 5 BXP**
    - Collecting 100 to 400 awards **5 to 35 BXP**
    - Collecting 400 to 700 awards **35 to 55 BXP**
    - Collecting 700 to 1000 awards **55 to 70 BXP**
    - Collecting 1000 to 1500 awards **70 to 80 BXP**
    - Collecting any more than 1500 will cap at **80 BXP**
    - The BXP scales with each credit earned; for example, getting 850 creds (halfway between 700 and 1000) gives 62 BXP (halfway between 55 and 70 BXP).
- Being the most profitable employee or playing solo grants a 25% bonus to your scrap collected, *unless* everyone died.
- Dying will lose you 15 BXP by default, but you'll lose more and more the higher rank you are.
- If everyone dies, the BXP Penalty for dying is amplified by **50%**.
- The BXP Penalty for dying is capped at -99 BXP. Likewise, the BXP from collecting scrap is capped at +99 BXP.
- Killing enemies will earn you BXP, **regardless of how it dies or who kills it**. Using landmines, lightning, or even another enemy to kill an enemy **will** grant BXP. You will also be notified at the bottom of your screen when an enemy dies (configurable).
- Depending on the weather of the moon, you may receive a bonus to your BXP earned from collecting scrap. Be warned though, as dying will also bear a larger penalty.

### New Rank Table
| Rank | BXP |
| ---- | :-: |
| Intern | **0 BXP** |
| Trainee | **25 BXP** |
| Apprentice | **50 BXP** |
| Part-Timer | **100 BXP** |
| Full-Timer | **200 BXP** |
| Leader | **300 BXP** |
| Manager | **500 BXP** |
| Sr. Manager | **700 BXP** |
| 3rd Boss | **1000 BXP** |
| 2nd Boss | **1300 BXP** |
| 1st Boss | **1600 BXP** |
| 3rd Vice President | **2000 BXP** |
| 2nd Vice President | **2400 BXP** |
| 1st Vice President | **2800 BXP** |
| 3rd Executive V.P. | **3200 BXP** |
| 2nd Executive V.P. | **3600 BXP** |
| 1st Executive V.P. | **4000 BXP** |
| Deputy President | **4500 BXP** |
| President | **5000 BXP** |
| Vice Chairman | **6000 BXP** |
| Chairman | **7000 BXP** |
| Co-Founder | **8000 BXP** |
| Founder | **9000 BXP** |
| Greatest Asset | **10000+ BXP** |
| The Company | **20000+ BXP** |

### Enemy Bonuses
| Enemy | BXP Awarded |
| ----- | :---------: |
| Snare Flea | **3 BXP** |
| Hoarding Bug | **4 BXP** |
| Thumper | **6 BXP** |
| Bunker Spider | **9 BXP** |
| Nutcracker | **9 BXP** |
| Masked | **10 BXP** |
| Baboon Hawk | **10 BXP** |
| Bracken | **12 BXP** |
| Eyeless Dog | **15 BXP** |

### Weather Bonuses
| Weather | Scrap/Death Multiplier |
| :-----: | :--------------------: |
| None | 0% |
| Rainy | **+5%** |
| Foggy | **+15%** |
| Flooded | **+15%** |
| Stormy | **+25%** |
| Eclipsed | **+25%** |


## Things to note
### Does BetterEXP replace the old system?
Nope, the BetterEXP system will run **alongside** the vanilla exp system. After a game, the XP bar will show your BetterXP Rank and XP amount, but your vanilla xp will still secretly be accounted for in the background. At any time, you may type `bxp/vanilla` in the in-game chat to view your current vanilla xp. You may also type `bxp/level` or open the pause menu to view your current BetterXP level.

### Can I turn off enemy notifications?
Yeah! You can tweak a few options in the config file. Access it through your mod manager, or `BepInEx/config`.

### Headstart
When you first load in with the BetterEXP mod, you'll start with 0 BXP at Intern rank. However, if you've played Lethal Company quite a bit, you'll start at a higher BetterXP level than just Intern. You'll receive a notification in-game about what your starting rank is. This will only display once, even if you reinstall the mod. You will be able to safely uninstall and reinstall the mod without affecting your vanilla XP, however, **you can not progress your BetterXP level without having the mod active** (duh).
| Vanilla Rank | BetterEXP Starting Rank |
| :----------: | :---------------------: |
| Part-Timer | **Trainee** |
| Employee | **Apprentice** |
| Leader | **Part-Timer** |
| Boss | **Full-Timer** |
| Boss (1000 EXP) | **Leader** |
| Boss (1500 EXP) | **Manager** |
| Boss (2000 EXP) | **Sr. Manager** |
| Boss (2500 EXP) | **3rd Boss** |
| Boss (3000 EXP) | **2nd Boss** |

### Incompatibilities
None that I'm aware of. Please check GitHub for updates on this, or to report an incompatibility.

---

betterexp version 1.2.1

lethal company version 49
