# Nether Fortress

The Nether Fortress is one of the most critical structures in any MCSR Ranked run. It is the only place in the game where **Blazes** spawn naturally, and Blazes are the sole source of **Blaze Rods** — the ingredient required to craft **Blaze Powder**, which in turn is used to craft **Eyes of Ender**. Without Eyes of Ender, you cannot locate and open the End Portal. The Nether Fortress is, therefore, a mandatory stop in every single-segment speedrun.

---

## Table of Contents

1. [Introduction & The Math](#1-introduction--the-math)
2. [Locating the Fortress](#2-locating-the-fortress)
3. [Fortress Structure Anatomy](#3-fortress-structure-anatomy)
4. [Finding the Blaze Spawner](#4-finding-the-blaze-spawner)
5. [Fighting Blazes — Detailed Combat Guide](#5-fighting-blazes--detailed-combat-guide)
6. [Spawner Farming Efficiency](#6-spawner-farming-efficiency)
7. [Blaze Rod Collection](#7-blaze-rod-collection)
8. [Wither Skeletons — A Serious Threat](#8-wither-skeletons--a-serious-threat)
9. [When to Leave the Fortress](#9-when-to-leave-the-fortress)
10. [Common Mistakes](#10-common-mistakes)
11. [Tips & Tricks](#11-tips--tricks)

---

## 1. Introduction & The Math

### Why You Need the Fortress

The End Portal in a Stronghold requires **Eyes of Ender** to activate. Each Eye of Ender is crafted from:
- **1 Blaze Powder** (crafted from 1 Blaze Rod → yields 2 Blaze Powder)
- **1 Ender Pearl** (obtained from Endermen or Piglin bartering)

Because 1 Blaze Rod = 2 Blaze Powder = 2 Eyes of Ender (assuming you have pearls), the number of rods you need depends on how many pearls you have and how many End Portal frames are already filled.

### The Critical Numbers

| Goal | Blaze Rods Needed |
|---|---|
| Bare minimum (very lucky portal, many pre-filled eyes) | 4–5 rods |
| Safe minimum for most runs | 7–8 rods |
| **Recommended target** | **10 rods** |
| If going for extra safety margin | 12 rods |

> [!IMPORTANT]
> A standard End Portal has **12 frames**, but some frames are pre-filled with Eyes of Ender at world generation. On average, about 0–3 frames will already be filled. Never leave the fortress with fewer than **7 rods** unless you have confirmed a heavily pre-filled portal via seed knowledge.

### Full Math Breakdown

- Each **Blaze Rod** → 2 Blaze Powder
- Each **Eye of Ender** = 1 Blaze Powder + 1 Ender Pearl
- 10 Blaze Rods → 20 Blaze Powder → 20 Eyes of Ender (if you have 20 pearls)
- In practice, 10 rods covers a 12-frame portal plus extras for traveling to the stronghold

> [!TIP]
> You only need **12 Eyes** at maximum for the portal. Getting 10 rods = 20 powder, which is more than enough powder. Your actual bottleneck is usually **Ender Pearls**, not rods. Plan your barter/Endermen kills accordingly.

---

## 2. Locating the Fortress

Finding a Nether Fortress quickly is one of the highest-skill-expression parts of any run. A minute lost searching for the fortress can make or break a competitive time.

### 2.1 Visual Identification

Nether Fortresses are composed of **dark Nether Brick** blocks, which contrast sharply with the surrounding Netherrack. Key visual cues:

- **Dark reddish-brown brick texture** — visually distinct from Netherrack's dull red
- **Large pillars and archways** rising above the Nether floor
- **Long, flat bridge-like corridors** extending outward
- **Open staircase platforms** jutting out from the main body
- The structure often appears **above lava lakes or cliffs**, making it visible from a distance

Look for straight edges and geometric shapes — the Nether is otherwise completely organic and chaotic. Any sharp corners or flat surfaces almost certainly indicate a Fortress.

### 2.2 Biome Clues

Nether Fortresses spawn in **all Nether biomes** with one critical exception:

| Biome | Fortress Can Spawn? |
|---|---|
| Nether Wastes | ✅ Yes |
| Crimson Forest | ✅ Yes |
| Warped Forest | ✅ Yes |
| Soul Sand Valley | ✅ Yes |
| **Basalt Deltas** | ❌ **No** |

> [!WARNING]
> If you find yourself in a **Basalt Delta** biome (recognizable by dark grey basalt columns and white blackstone), do **not** waste time searching there. Move in any direction until you exit the biome.

Soul Sand Valleys are particularly useful as visual searching is easier due to the flat terrain and low fog density. Crimson Forests, while dense, often border Nether Wastes where fortresses commonly appear.

### 2.3 The Z-Band Generation Rule

This is one of the most important navigation concepts in Nether speedrunning:

> Nether Fortresses generate in **bands along the North-South axis (Z-axis)**. Specifically, they appear in alternating **positive and negative Z bands**, each roughly **768 blocks wide** in the Nether's coordinate system.

**What this means in practice:**

- If you find a fortress at coordinates (X=200, Z=400), other fortresses exist **near the same Z value** — both east and west of your current position.
- Moving **East (positive X) or West (negative X)** while staying at roughly the same Z value has a high chance of finding another fortress.
- Moving **North or South (Z-axis)** takes you out of the current band and into a potentially empty zone.

**Action:** Once you confirm your Z coordinate from F3, move along the **X-axis** to search for the fortress efficiently within your current Z band.

### 2.4 The Pie Chart Method (F3 / Shift+F3)

The **Debug Menu** in Minecraft provides a powerful tool for fortress detection: the **entity/chunk rendering pie chart**.

#### How to Enable the Pie Chart:
1. Press **F3** to open the debug screen
2. Press **Shift+F3** to toggle the pie chart overlay (appears in the bottom-right or top-right corner)
3. The chart shows what the game is spending rendering time on

#### Reading the Pie Chart for Fortress Detection:

- Look for the **"spawners"** or **"entities"** sections in the breakdown
- Blazes and Wither Skeletons inside a fortress will show up as entity rendering load
- If you see **"blaze"** listed in the entity rendering breakdown, you are near a Blaze spawner
- A large number of mob-type entries suggests you are close to a fortress interior

> [!NOTE]
> The pie chart entity method works best when you are **within ~100–150 blocks** of the fortress. It is a confirmation tool more than a discovery tool, but experienced runners use it to confirm they are closing in on a spawner.

#### Using F3+F (Render Distance):
- Press **F3+F** to **increase render distance** by 1 each press
- A higher render distance lets you see fortress structures from further away
- Useful when you are in a flat Nether Wastes area with good visibility
- Be aware: increasing render distance drops FPS and may cause lag spikes — use sparingly

### 2.5 Movement Strategy

When actively searching for a fortress:

1. **Stay on the surface.** Do not tunnel through Netherrack. You need visual contact with the fortress.
2. **Sprint and jump.** Move as fast as possible while scanning the horizon.
3. **Gain elevation.** If you can safely get on top of a Netherrack pillar or mound, you dramatically increase your visible range.
4. **Follow the X-axis.** As discussed above, move East or West once you know your Z band.
5. **Avoid lava ocean areas.** They waste time. Stick to areas where you can move freely.
6. **Listen for sounds.** Blaze sounds (a sharp crackling/whirring) can be heard through walls at moderate distances — a key audio cue that a fortress is nearby.

---

## 3. Fortress Structure Anatomy

Understanding the layout of a Nether Fortress will save you enormous amounts of time. Fortresses are procedurally generated from a set of modular "rooms," connected in various configurations.

### 3.1 The Two Main Types of Sections

**Bridge/Corridor Sections:**
- Long, open walkways of Nether Brick
- Exposed on the sides, often with fencing or railings
- Wither Skeletons and regular Nether Skeletons patrol these heavily
- Not where you want to spend time — traverse quickly

**Enclosed Room Sections:**
- Fully enclosed or partially enclosed brick rooms
- Include the Nether Wart room, the Blaze Spawner room, and miscellaneous storage rooms
- These are your targets

### 3.2 Blaze Spawner Rooms

There are typically **1–2 Blaze Spawners** per fortress (sometimes 0 or 3, but 2 is most common).

**What the Blaze Spawner room looks like:**
- An **open-air staircase platform** jutting from the side of the fortress
- A **cage block (Mob Spawner)** sitting on or near the center of the platform
- Surrounded by **Nether Brick half-slabs** on multiple levels
- Blazes spawn from the cage and wander the platforms around it

This room is intentionally exposed to open air, making it more dangerous (no walls for cover) but also easier to spot visually once you know what to look for.

### 3.3 The Nether Wart Room

- Contains **Soul Sand** patches with **Nether Wart** growing on them
- **Not important for standard speedrunning** — Nether Wart is used for Potions, not End Portal activation
- Useful only if you are pursuing a potion-heavy strategy (e.g., Fire Resistance)
- You may run through this room while navigating; don't linger

### 3.4 The Fortress "Hub" System

Rooms in a Nether Fortress are not random — they connect in a branching tree structure:

- A central **spine** of corridors runs through the fortress
- Rooms **branch off** from this spine
- Each branch can dead-end or connect to another corridor
- **Blaze Spawner rooms are always accessible from a corridor** — follow the corridors and check each branch

> [!TIP]
> When exploring, mentally mark which corridors you have already checked. The fortress has a finite number of rooms — systematic exploration beats random wandering.

---

## 4. Finding the Blaze Spawner

### 4.1 Visual Recognition of the Spawner

The **Mob Spawner cage** is a distinctive 1×1×1 block with a visible spinning mob inside (in this case, a tiny spinning Blaze model). It emits **flame particles** continuously, even when no Blazes are actively spawning. Look for:

- The orange/yellow flicker of flame particles
- The dark iron cage texture
- The staircase platform it sits on

You will often see the spawner **before** you see the room clearly — the flame particles are visible through small gaps and around corners.

### 4.2 Using Subtitles to Detect Blazes

Enable **Subtitles** in your audio settings (Options → Music & Sounds → Show Subtitles: ON). This is **highly recommended** for speedrunning.

- Blazes make a unique **whirring/crackling sound** when they exist nearby
- The subtitle "Blaze whirs" or "Blaze shoots" will appear on screen when a Blaze is within audio range
- This gives you directional audio feedback that a spawner is active nearby
- Hearing Blaze sounds through walls narrows your search significantly

### 4.3 Pie Chart Entity Detection for the Spawner

When you are inside the fortress and using the Shift+F3 pie chart:

1. Walk slowly through corridors
2. Watch the entity rendering slice of the pie chart
3. When the "blaze" entry appears or grows, you are moving **toward** the spawner
4. When it disappears or shrinks, you are moving away

This method is especially powerful in confusing multi-level fortresses where visual searching is difficult.

### 4.4 Navigating to the Spawner Efficiently

- Once you detect Blaze sounds or pie chart evidence, **sprint toward the signal**
- The spawner room is always accessible — there is no maze with a dead end between you and it
- Clear Wither Skeletons in your path only if necessary; otherwise sprint past them
- Upon reaching the staircase platform, **immediately begin combat** — do not pause to explore further

---

## 5. Fighting Blazes — Detailed Combat Guide

Blaze combat is one of the highest-risk moments in a speedrun. Getting it right dramatically affects both your time and your health pool for the rest of the run.

### 5.1 Blaze Statistics

| Stat | Value |
|---|---|
| Health | 20 HP (10 hearts) |
| Attack — Fireball | 5 damage (2.5 hearts) per fireball, 3-fireball burst |
| Attack — Melee (contact) | 6 damage (3 hearts) |
| XP on death | 10 XP orbs |
| Blaze Rod drop rate | 50% (0 or 1 rod, never more) |
| Spawn range from spawner | Within 4 blocks horizontally, 2 blocks vertically |

**The 3-Fireball Burst:** Blazes attack in a pattern — they ignite (rise into the air, flash orange) then fire **3 fireballs in rapid succession**. After the burst, they pause briefly before repeating. This pause is your best window to deal damage safely.

### 5.2 Snowball Method

> [!TIP]
> The fastest Blaze-killing method if you have snowballs.

- **Damage per snowball:** 3 HP (1.5 hearts)
- **Snowballs to kill a Blaze:** 7 snowballs (7 × 3 = 21 damage, overkills by 1)
- **Throw speed:** Very fast — you can throw multiple per second
- Blazes are knocked back by snowballs, resetting their attack pattern

**When is this viable?**
- Only if your overworld route took you through a **cold biome** (Snowy Plains, Snowy Taiga, Ice Spikes, Frozen Ocean)
- You need to collect **snowballs** before entering the Nether — each snow layer breaks into 1–3 snowballs, and snowmen can be crafted
- Viable for Village/Buried Treasure routes that pass cold biomes, or if you specifically detoured

**Technique:**
1. Strafe to dodge the fireball burst
2. Spam snowballs during the Blaze's pause window
3. A coordinated player can kill Blazes in under 2 seconds each

### 5.3 Sword Method

The most common combat method. Works regardless of your overworld route.

| Sword Type | Damage per hit | Hits to Kill |
|---|---|---|
| Wooden Sword | 4 HP | 5 hits |
| Stone Sword | 5 HP | 4 hits |
| Iron Sword | 6 HP | 4 hits |
| Diamond Sword | 7 HP | 3 hits |
| Iron Sword + Critical | 9 HP | 3 hits |

**Critical Hits:**
- Jump and attack at the peak of your jump to deal a **critical hit** (approximately 1.5× damage)
- The critical hit animation shows stars/sparks on the enemy
- Critical hits with an Iron Sword effectively kills Blazes in 3 hits — same as a Diamond Sword
- **Spam critical hits** by jump-attacking repeatedly for maximum damage output

**Recommended combat loop:**
1. Close the distance as soon as the Blaze finishes its fireball burst
2. Jump-attack (critical hit) as many times as possible during its pause
3. Back away when it begins to ignite again
4. Repeat

### 5.4 Close-Range Combat Technique

One of the most important techniques for Blaze combat:

> **Stand directly underneath the Blaze** when it fires.

Blaze fireballs are fired from the Blaze's eye level and travel in a straight line. If you are standing **directly beneath** the Blaze (within 1–2 blocks), the fireballs fly over your head. This dramatically reduces incoming damage.

- Requires you to be directly below the Blaze — position matters
- Works especially well on the raised staircase platforms where Blazes hover above you
- Combine with sword strikes upward for damage

### 5.5 Shield Method

If you crafted or found an **Iron Shield** during your run:

- **Shields completely block Blaze fireballs** when raised (right-click)
- The fireball deals 0 damage and is reflected (reflected fireballs can damage other Blazes — free damage!)
- Shields have a 5-tick activation delay — raise the shield **before** the Blaze begins its burst
- Highly recommended for newer runners or for conserving health

**Iron cost:** Shields require 6 planks + 1 iron ingot — very cheap. If you have iron to spare in your run, craft one.

### 5.6 Bed Explosion Method

An advanced, high-risk high-reward technique:

- **Beds explode** when placed and activated in the Nether (same as the End)
- The explosion radius can damage multiple Blazes simultaneously for **massive AoE damage**
- A single bed explosion can kill or severely weaken a cluster of Blazes

**Execution:**
1. Wait until multiple Blazes are grouped near the spawner
2. Place the bed on the ground or against a wall near the cluster
3. Right-click the bed to activate the explosion
4. The explosion deals approximately **40–70 HP of damage** in a radius — more than enough to kill any Blaze

> [!WARNING]
> Bed explosions also deal damage to the **player**. Position yourself behind a wall or pillar, or have sufficient health. This technique can be self-fatal if misused. Blaze platforms are often open-air — be careful not to be launched into lava.

### 5.7 Fire Damage & Health Management

Blazes set you on fire when they deal contact damage, and fireballs also cause the **on-fire status effect** (2 seconds of burn):

- Eat food continuously to offset fire damage — golden carrots, bread, cooked meat
- **Fire Resistance Potion** makes you completely immune to fire and fireballs — extremely powerful if you have one
- Lava proximity and Blaze fireballs stack fire damage fast
- Keep your health above **6 hearts** (12 HP) to survive a full 3-fireball burst

---

## 6. Spawner Farming Efficiency

### 6.1 Stay Within 16 Blocks of the Spawner

Mob spawners have a **spawn radius** and only produce mobs when a player is **within 16 blocks**. If you move too far away:
- The spawner deactivates
- No new Blazes appear
- You lose precious farming time

Always position yourself **within 16 blocks** of the spawner while farming — ideally within 4–8 blocks for maximum efficiency.

### 6.2 Clear the Room First

Before settling in to farm:

1. **Kill all currently active Blazes** in the room
2. Locate and destroy (or avoid) any Wither Skeletons that wandered onto the platform
3. Identify escape routes in case your health gets low

A cluttered room with multiple threats will kill you. Take 10–15 seconds to clear it before dedicated farming begins.

### 6.3 Kill Blazes the Instant They Spawn

The faster you kill each Blaze, the faster the spawner can produce the next one. Mob spawners have a **cooldown between spawns**, but the cooldown is shorter when Blazes are not already alive near the spawner.

- The spawner can have **up to 6 Blazes alive** in its vicinity at once before it stops spawning
- Killing Blazes immediately keeps the alive count low → spawner stays active → faster spawns
- Do not let them pile up — constant pressure on the spawner is more efficient

### 6.4 Do NOT Break the Spawner

> [!CAUTION]
> Never mine/destroy the Blaze Spawner. Once destroyed, it is gone permanently for that run. You need it to keep producing Blazes for the duration of your farm.

Spawners can only be broken with a pickaxe, so as long as you are not accidentally clicking on it with one, you are fine. Just be aware during hectic combat.

### 6.5 Second Spawner Strategy

If the fortress has a **second Blaze Spawner** (which many do):
- Finding it doubles your spawn rate
- Consider spending 15–20 seconds to locate it if your rod count is low
- Farm both spawners by alternating between them, staying within 16 blocks of each

---

## 7. Blaze Rod Collection

### 7.1 Drop Rate and Expected Yield

| Metric | Value |
|---|---|
| Drop chance per Blaze | 50% (0 or 1 rod) |
| Average rods per kill | 0.5 |
| Expected rods from 10 kills | ~5 rods |
| Expected rods from 20 kills | ~10 rods |
| Kills needed for 10 rods (average) | ~20 kills |

> [!NOTE]
> The 50% drop rate means significant variance. You may get 10 rods in 15 kills on a lucky run, or only 6 rods from 20 kills on an unlucky one. Plan your farm time with this variance in mind — always kill a few extra Blazes beyond your minimum.

### 7.2 Pick Up Rods Immediately

Dropped items in Minecraft despawn after **5 minutes (6000 game ticks)**. During an intense Blaze fight, rods can fall into awkward positions:

- **Into lava** — destroyed instantly, no recovery
- **Off platform edges** — lost if there is no floor below
- **Behind the spawner** — easy to miss while fighting

After each kill, glance at where the rod landed and move to pick it up if it is safe. Do not let rods sit for more than 30–60 seconds during active combat.

### 7.3 Rod Counting

Keep a mental (or literal) count of how many rods you have collected:
- Check your inventory periodically via quick-open (E key)
- Know your target number (8–10 rods)
- Once you hit your target, do **not** overfarm — every extra second in the fortress is time lost

### 7.4 Looting Enchantment

If you somehow have a **Looting III** sword (unlikely in a normal run but possible on some seeds):
- Looting increases max rod drops to **1–4 rods per kill**
- This dramatically reduces kills needed — you can hit 10 rods in 5–6 kills
- Worth noting if you find an enchanted sword in a chest

---

## 8. Wither Skeletons — A Serious Threat

### 8.1 Stats & Abilities

| Stat | Value |
|---|---|
| Health | 20 HP (10 hearts) |
| Attack damage | 8 HP (4 hearts) per hit |
| **Wither Effect** | 10 seconds of Wither II — deals 2 HP/second, can kill through healing |
| Height | 2.4 blocks tall — won't fit through 2-block gaps |

The **Wither Effect** is extremely dangerous:
- Turns your health bar black, making it impossible to see your actual HP
- Deals continuous damage over 10 seconds (20 HP total at Wither II — enough to kill you)
- **Does not stop at 0.5 hearts** like normal damage — Wither can kill you completely
- Stacks if you are hit multiple times

### 8.2 Where They Spawn

- Wither Skeletons spawn throughout the **enclosed corridors and rooms** of the Nether Fortress
- They do NOT spawn on Blaze Spawner platforms (which are open-air)
- Most common in the long bridge corridors connecting rooms
- They can be numerous — groups of 2–5 are common

### 8.3 How to Handle Them

**Option 1: Avoid/Sprint Past**
- Wither Skeletons are slow and have a relatively short aggro range
- Sprinting past them is usually viable when navigating to the spawner
- They will chase you but rarely keep up with a sprinting player

**Option 2: Kill with Height Advantage**
- Wither Skeletons are 2.4 blocks tall — they cannot walk through 2-block-tall gaps
- Create a small 2-block gap and hit them from safety — they cannot reach you
- Very efficient for clearing corridors

**Option 3: Shield Block**
- Shields do NOT block the Wither effect from Wither Skeleton melee attacks
- A shield blocks the damage but the Wither effect still applies on some versions
- Do not rely on shields for Wither Skeletons the same way you do for Blazes

> [!WARNING]
> Never let a Wither Skeleton hit you when your health is already low from Blaze combat. The Wither effect can finish you off even if the actual hit deals manageable damage.

### 8.4 Wither Skeleton Skulls (Not Your Goal)

Wither Skeletons have a rare chance to drop their skull, used to summon the Wither boss. This is **irrelevant to a standard speedrun** — do not farm for skulls.

---

## 9. When to Leave the Fortress

Knowing **when to stop** is as important as the combat itself. Staying too long wastes time; leaving too early forces you back or dooms the run.

### 9.1 The Rod Count Threshold

| Rod Count | Decision |
|---|---|
| 0–5 rods | Keep farming — do not leave |
| 6–7 rods | Consider leaving only if health is critically low or run is falling apart |
| **8–10 rods** | **This is your target — leave when you reach this range** |
| 11+ rods | You are overfarming — stop and leave immediately |

### 9.2 Health-Based Decision Making

Your health upon leaving the fortress matters because you will need to:
- Navigate back through the Nether
- Find and navigate the Stronghold
- Fight the Ender Dragon

**Leave immediately if:**
- You are below **4 hearts** and actively taking damage
- You have no food and are hungry
- A Wither effect is active and you have no milk

**Accept the risk and keep farming if:**
- You are at 8+ hearts and only need 1–2 more rods
- You have plenty of food to sustain through more combat

### 9.3 Time-Based Instinct

In competitive runs, every second matters. Develop an instinct for when you have spent "too long" in the fortress relative to your run's pace:

- A clean fortress visit should take **60–120 seconds** from spawner found to leaving
- Elite runners can complete the fortress in under 60 seconds with a good spawner position and good drops
- If you have been farming for over **3 minutes** and still do not have 8 rods, something went wrong (bad drops, second spawner needed, etc.)

---

## 10. Common Mistakes

### 10.1 Searching in Basalt Deltas
**Mistake:** Spending 30–60 seconds wandering through Basalt Deltas looking for a fortress.  
**Fix:** Immediately exit any Basalt Delta biome upon recognizing it. Move perpendicular to the biome border.

### 10.2 Breaking the Blaze Spawner
**Mistake:** Accidentally mining the spawner cage during combat.  
**Fix:** Equip your sword before entering the spawner room. Only switch to pickaxe when intentionally mining.

### 10.3 Moving Too Far From the Spawner
**Mistake:** Chasing a Blaze that wandered 20+ blocks away, deactivating the spawner.  
**Fix:** Let wandering Blazes come back to you, or finish them quickly and return to within 16 blocks.

### 10.4 Ignoring Wither Skeletons
**Mistake:** Getting hit by a Wither Skeleton at low health during Blaze farming, dying from the Wither effect.  
**Fix:** Clear the spawner platform perimeter before settling in to farm. Be aware of your surroundings at all times.

### 10.5 Not Picking Up Rods
**Mistake:** Dropping rods into lava or off platform edges, failing to reach your rod target despite enough kills.  
**Fix:** Position combat over solid ground when possible. Pick up rods within 30 seconds of each kill.

### 10.6 Overfarming
**Mistake:** Continuing to farm blazes after reaching 12+ rods "just to be safe," wasting 30–60 extra seconds.  
**Fix:** Set a clear mental target (10 rods). Leave the second you hit it.

### 10.7 No Food for the Fortress
**Mistake:** Entering the fortress with no food, unable to heal fire/fireball damage.  
**Fix:** Always carry food from your overworld segment. Bread, carrots, or cooked meat from village chests are ideal.

### 10.8 Tunneling Through Netherrack
**Mistake:** Mining through Netherrack instead of searching on the surface, taking far longer to find the fortress.  
**Fix:** Stay on the surface, gain elevation, and scan visually. Only mine if you are completely stuck.

### 10.9 Going the Wrong Direction
**Mistake:** Moving North or South (Z-axis) to search for a fortress when you should be moving East or West (X-axis).  
**Fix:** Note your Z coordinate from F3. Move along the X-axis to stay in your current Z generation band.

---

## 11. Tips & Tricks

### 11.1 Nether Brick as a Landmark
Once you spot any Nether Brick — even a single pillar — you are near a fortress. Follow the brickwork; it always leads to more structure.

### 11.2 F3 Coordinates at All Times
Keep F3 open throughout your Nether search. Knowing your exact X and Z coordinates is essential for applying the Z-band rule and using the pie chart effectively.

### 11.3 Pre-Angle Your Camera
While sprinting through the Nether looking for the fortress, tilt your camera **upward slightly**. Fortresses often appear elevated above the Nether floor. Looking at ground level causes you to miss structures that are up on ridges or cliffs.

### 11.4 Audio Priority
Turn your **mob sounds up** in settings. Blaze sounds carry further than you think. Many experienced runners find the fortress by hearing Blazes before they see the structure.

### 11.5 Lava as a Fortress Indicator
Nether Fortresses frequently spawn near or over **lava oceans and lava falls**. If you see a large lava feature, scan the surrounding area carefully — a fortress may be partially submerged in or adjacent to it.

### 11.6 Use the Fortress for Pathing
Once you have your rods, the fortress itself provides high ground for better Nether navigation. Use it as a landmark to reorient before heading to your Nether exit/portal.

### 11.7 Potions of Fire Resistance
If your run includes a **Bastion Remnant**, you may loot **Potions of Fire Resistance** from Piglin bartering or chest loot. Using one during Blaze combat:
- Makes you completely immune to fireballs
- Lets you stand still and sword-spam without dodging
- Dramatically speeds up your kill rate
- Eliminates the risk of fire-related death

### 11.8 Auto-Jump for Platform Traversal
The Blaze Spawner's staircase platform has multiple levels. Enable **Auto-Jump** (Options → Controls) if you do not normally use it — it can help quickly navigate the half-slab steps without having to manually jump.

### 11.9 Eat Between Bursts
The Blaze fireball 3-burst pattern gives you a predictable window. Use the **pause between bursts** not only to deal damage but also to **eat food** if your health is low. Eating is momentary — you can interrupt it if the Blaze begins to fire again.

### 11.10 Knowing When to Run
If a cluster of 4+ Blazes is actively firing and your health is below 5 hearts — **run**. Duck into an enclosed corridor (Blazes cannot follow easily into tight spaces), eat food, and recover before re-engaging. A death reset loses far more time than a brief retreat.

### 11.11 Strafe, Don't Stand Still
Even without a shield, strafing side-to-side while a Blaze charges its burst makes you significantly harder to hit. Blazes must aim their fireballs — lateral movement disrupts their targeting. Combine strafing with the close-range technique (staying underneath the Blaze) for the safest combat experience.

### 11.12 Practice Makes Perfect
Blaze combat is a **mechanical skill** — the timing, positioning, and decision-making only improve through repetition. Dedicate practice sessions specifically to Nether Fortress routing and Blaze fighting. Use creative mode or practice worlds to drill the combat without the pressure of an active run.

---

## Quick Reference Card

| Task | Key Info |
|---|---|
| Rods needed | 8 minimum, **10 recommended** |
| Rod → Powder | 1 rod = 2 powder |
| Powder → Eye | 1 powder + 1 pearl = 1 Eye |
| Blaze HP | 20 HP (10 hearts) |
| Snowballs to kill | 7 snowballs |
| Iron sword hits | 4 hits (3 with crits) |
| Rod drop chance | 50% per kill |
| Spawner activation range | 16 blocks |
| Max Blazes near spawner | 6 before spawner pauses |
| Fortress biome exception | ❌ Basalt Deltas |
| Search direction | Move along **X-axis** (East/West) |
| Wither Skeleton danger | Wither II effect — 2 HP/sec for 10 sec |

---

*Page maintained by the MCSR Ranked Wiki contributors. For meta updates and strategy revisions, refer to the MCSR Ranked Discord.*
