# Season 4

## GR 5.0.0 | Alpha 1
- Fixed bug with defense pickup gamepass where multiple players owned the same defense block location
- Fixed bug with anticheat mod detection not scanning the second list of mods
- Anticheat modified to remove limbo world compatibility | Virtual sign GUI instead of a physical sign, reducing load, and making it faster
- Anticheat checks now check if sign lines *contain* the fallback string, instead of are equal to the fallback string | Eliminates all false flags due to milisecond keyboard inputs
- Season 3 Seasonal Tag Added (lime green)
- Genspeed nerfed | `10s Default -> 15s Default` - `5s Maxed -> 10s Maxed`
- Defense range added | 75 block range
- Fixed defense pickup bug | 2 players can no longer own the same defense block if one is broken by a player with the gamepass

## GR 5.0.0 | Alpha 2
- Fixed disconnection bug during an anticheat packet race with the player's chunks loading | If the client doesnt render the sign GUI before it closes, the client throws an error and disconnects. Fixed
- Removed all debug worlds and timers from the anticheat | You will no longer see the sign appear, and no longer be teleported. Entirely seamless
- Removed the lifesteal enchantment | Too unbalanced. Too OP.
- Added Plunder enchantment
  - Each level of this enchantment, increases the amount of money you steal by killing a player, by 5%
  - When you kill a player, by default, you steal 10% of their money. With each level of plunder on your sword, you steal an extra 5%
  - Maxes out at level 3
- Fixed bug where if a player stands inside of a door/trapdoor block hitbox during a modcheck, for the door to be removed and they walk through it, they are now teleported back to their original location after the door/trapdoor is restored.

## GR 5.0.0 | Alpha 3
- Patched sign dupe | Mine the sign as it spawns to check your mods. Every rejoin would dupe 3 signs. This is no longer the case.
- Bow + Arrows added to shop
  - Possible enchantments: Power 1, Power 2, Flame 1 + Power 2 (Maxed)
- Level milestone enchantment rewards update
  - When selecting an enchantment upgrade, you now select a specific tool/item to upgrade the protection/sharpness/efficiency/power level of.
- Added back button to all milestone reward GUI's
- Claiming a milestone reward no longer closes the GUI | Makes it easier to claim multiple
- Made all system chat prefixes uniform (The same)
- Increased level milestones to level 350, instead of 210

## GR 5.0.0
- Added Meteor Shower Event
  - The server falls to night, as meteors rain down from the sky. Once a meteor lands, it spawns a chest, with a range of loot for players to collect.
  - Event occurs every 2 hours
  - Loot table for chests:
    - Item | Chance | Qty
    - Money Note | 85% | $1,250-$3,750
    - Shard Note | 80% | ♦10-30
    - T1 Defense | 90% | 20-40
    - T2 Defense | 85% | 15-30
    - T3 Defense | 75% | 10-20
    - T1 Door | 80% | 5-15
    - T1 Trapdoor | 75% | 5-15
    - T4 Generator | 80% | 1-4
    - T5 Generator | 65% | 1-4
    - T6 Generator | 45% | 1-4
    - T7 Generator | 25% | 1-4
    - T8 Generator | 12% | 1-4
    - T9 Generator | 5% | 1-4
    - Cobblestone | 85% | 16–48
    - Quartz Block | 70% | 8–16
    - Arrows | 80% | 16–48
    - Defense Wax | 85% | 10–30
    - Respawn Beacon | 55% | 1
    - Tesla Coil    20% | 1
    - Supply Crate | 8% | 1
    - Scout Rank | 2% | 1
  - Meteor shower lasts 30 seconds
  - 20 meteors spawn per event
- Added proxy | All players who connect via the main IP (**Play.CarrotNetwork.Net**) will directly connect to the backend servers, bypassing minekeep entirely. Please use this IP, unless you have a reason to connect via the minekeep IP. We support both fully, but do reccomend the main IP.
