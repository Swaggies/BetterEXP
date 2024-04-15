# BetterEXP

[GitHub](https://github.com/Swaggies/BetterEXP)
[Thunderstore Page](https://thunderstore.io/c/lethal-company/p/Swaggies/BetterEXP/)

**BetterEXP** is a Lethal Company mod looking to spice up the current experience system in the game. Right now the XP system feels a bit clunky and not a good (enough) measure of a player's true experience working for The Company, so I've created BetterEXP to hopefully make the XP system feel much more satisfying and rewarding/punishing, depending on your actions.

If you would like to help, give ideas, report bugs, or just play Lethal Company with me, you can contact me on Discord `@swaggies`. Shoot me a message anytime and I'll get back as soon as I can!

![Showcase](https://github.com/Swaggies/LCModAssets/blob/main/v2/v2%20performance.gif?raw=true)
![Round Summary](https://github.com/Swaggies/LCModAssets/blob/main/v2/v2%20round%20summary_main.png?raw=true)

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
- **Most Lethal**: killed the most entities in a day.
- **The Pacifist**: was the *only* employee to not kill an entity.

If any two (or more) players tie on any of these stats, they will all get the note!

## BetterXP System
- You will now gain "BetterXP" (BXP) primarily based on scrap collected, and your ability to fully clear the facility of scrap. See the below table for values (where Total Scrap Value is the amount of scrap value needed for a full clear, and Max BXP Possible is the amount of BXP awarded for a full clear):

| Total Scrap Value | Max BXP Possible |
| :---------------: | :--------------: |
| 0 - 300 | 0 - 7 |
| 300 - 500 | 7 - 15 |
| 500 - 700 | 15 - 25 |
| 700 - 1000 | 25 - 36 |
| 1000 - 1600 | 36 - 60 |
| 1600 - 2000 | 60 - 70 |
| 2000 - 2500 | 70 - 80 |
| 2500 - 3000 | 80 - 88 |
| 3000 - 4000 | 88 - 100 |
| 4000 - 8000 | 100 - 115 |
| 8000 - 9999 | 115 - 120 |
| 9999+ | 120 |

- Depending on how much you contributed for your team, you may receive bonus BXP as a reward.
    - When playing solo, you are always granted a 25% bonus to your scrap collected.
- Dying will lose you a bit of BXP, but you'll lose more and more the higher rank you are.
- If everyone dies, the BXP Penalty for dying is amplified by **25%**.
- The BXP Penalty for dying is capped at -100 BXP.
- Killing enemies will earn you BXP, as long as you're the person to finish them off. Using landmines, lightning, or even another enemy to kill an enemy will not grant BXP **unless you damaged it beforehand**. You will also be notified at the bottom of your screen when an enemy dies (configurable).
    - The more enemies you kill, the less BXP you will get for each kill.
- Depending on the weather of the moon, you may receive a bonus to your BXP earned from collecting scrap. Be warned though, as dying will also bear a larger penalty.

### Enemy Bonuses
| Enemy | Base BXP |
| ----- | :---------: |
| Tulip Snake | **1 BXP** |
| Manticoil | **2 BXP** |
| Snare Flea | **4 BXP** |
| Hoarding Bug | **4 BXP** |
| Thumper | **6 BXP** |
| Bunker Spider | **6 BXP** |
| Masked | **6 BXP** |
| Butler | **8 BXP** |
| Nutcracker | **8 BXP** |
| Bracken | **8 BXP** |
| Baboon Hawk | **8 BXP** |
| Eyeless Dog | **12 BXP** |
| Forest Giant | **16 BXP** |

### Weather Bonuses
| Weather | Scrap/Death Multiplier |
| :-----: | :--------------------: |
| None | 0% |
| Rainy | **+10%** |
| Foggy | **+15%** |
| Flooded | **+15%** |
| Stormy | **+25%** |
| Eclipsed | **+25%** |

### New Rank Table
| Rank | BXP |
| ---- | :-: |
| Intern | **0 BXP** |
| Trainee | **25 BXP** |
| Apprentice | **50 BXP** |
| Part-Timer | **100 BXP** |
| Full-Timer | **200 BXP** |
| Employee | **300 BXP** |
| Leader | **400 BXP** |
| Manager | **600 BXP** |
| Sr. Manager | **800 BXP** |
| 3rd Boss | **1000 BXP** |
| 2nd Boss | **1300 BXP** |
| 1st Boss | **1600 BXP** |
| 3rd Vice President | **2000 BXP** |
| 2nd Vice President | **2300 BXP** |
| 1st Vice President | **2600 BXP** |
| 3rd Executive V.P. | **3000 BXP** |
| 2nd Executive V.P. | **3300 BXP** |
| 1st Executive V.P. | **3600 BXP** |
| 3rd Deputy President | **4000 BXP** |
| 2nd Deputy President | **4300 BXP** |
| 1st Deputy President | **4600 BXP** |
| President | **5000 BXP** |
| Sr. President | **5500 BXP** |
| Vice Chairman | **6000 BXP** |
| Chairman | **6500 BXP** |
| First-Class Asset| **7500 BXP** |
| Co-Founder | **8500 BXP** |
| Founder | **10000+ BXP** |


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
| Boss (1000 EXP) | **Employee** |
| Boss (1500 EXP) | **Leader** |
| Boss (2000 EXP) | **Manager** |
| Boss (2500 EXP) | **3rd Boss** |
| Boss (3000 EXP) | **3rd Boss** |

### Incompatibilities
- *(minor)* **LCUltrawide**: Pause menu BXP display goes off-screen.
- *(minor)* **AdvancedCompany**: Pause menu BXP display overlaps with the "Save" button, making it unclickable.
---

betterexp version 2.0.0

lethal company version 50
