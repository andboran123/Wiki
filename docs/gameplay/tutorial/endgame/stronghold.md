# Stronghold Navigation

> **Goal:** Find the Portal Room inside the stronghold, fill all empty End Portal frames with Eyes of Ender, and jump into the portal to reach The End.

---

## Table of Contents

1. [Introduction](#introduction)
2. [How to Enter the Stronghold](#how-to-enter-the-stronghold)
3. [Stronghold Layout Basics](#stronghold-layout-basics)
4. [Finding the Portal Room](#finding-the-portal-room)
5. [The Portal Room](#the-portal-room)
6. [Filling the End Portal](#filling-the-end-portal)
7. [Common Mistakes](#common-mistakes)
8. [Tips & Tricks](#tips--tricks)

---

## Introduction

The **stronghold** is an underground structure that contains the **End Portal** — the only way to reach The End and fight the Ender Dragon. Every MCSR Ranked run ultimately leads here. Your objective inside the stronghold is simple:

1. Navigate the maze-like halls to find the **Portal Room**.
2. Fill any empty **End Portal frames** with Eyes of Ender.
3. **Jump into the activated portal** to complete the overworld segment.

Despite sounding straightforward, the stronghold is one of the most time-consuming parts of a run. Players who can navigate it efficiently — ideally in under 60–90 seconds — gain a massive time advantage. This article covers everything you need to know to do exactly that.

---

## How to Enter the Stronghold

### Digging Down After Eye Triangulation

After using Eyes of Ender (and Ninjabrain Bot) to pinpoint the stronghold's location, you will need to **dig down** to find it. Strongholds generate primarily between **Y=40 and Y=55**, though they can appear slightly higher or lower depending on terrain.

- Dig at a **45-degree staircase angle** — never straight down. Digging straight down risks falling into a cave, lava lake, or directly into a dangerous part of the stronghold.
- You are looking for **stone bricks** (regular, mossy, or cracked). Spotting any of these block types while digging means you have hit the stronghold structure.
- Once you break into the stronghold, stop digging outward and start navigating.

### The Staircase Entrance (Starter Room)

Every stronghold has a **starter staircase room** — a stone brick staircase descending into the structure. This room is typically the first room you encounter when you first break into the stronghold at its edge. It usually features:

- A **descending staircase** made of stone brick slabs.
- Possible **torches** on the walls.
- A **wooden door** at the base of the stairs leading into the main corridor network.

> [!NOTE]
> The starter staircase room is **not** always your entry point when digging in. You may break into a corridor, library, or even a prison cell depending on where you dig. Don't panic — just start navigating.

### Alternative Entries

- **Surface holes:** Some strongholds partially expose themselves through ravines or cave entrances. If you see stone brick blocks on the surface or in a ravine wall, you may be able to enter the stronghold through there without digging.
- **Cave systems:** Caves occasionally intersect with strongholds. You might enter through a cave opening if the geometry lines up with the stronghold location.

---

## Stronghold Layout Basics

Strongholds are **procedurally generated** — no two are exactly the same. However, they follow a set of **structural rules** defined by the game code, meaning there are recognizable patterns and room types you will encounter every time.

### Key Room Types

| Room Type | Description | Dead End? |
|---|---|---|
| **Starter Staircase** | Entry point; descending stairs with a door | No |
| **Corridor** | Long hallway with doors on the sides | No |
| **Crossroads** | Junction connecting multiple corridors | No |
| **5-Way Crossing** | The largest junction; very important landmark | No |
| **Prison Cell Room** | Small room with iron bars and possibly a chest | Often |
| **Library** | Large room with bookshelves, cobwebs, chests | **Yes — Dead End** |
| **Portal Room** | Contains the End Portal and silverfish spawner | **Terminal** |

### General Layout Rules

- Strongholds are **not infinite**. They have a finite number of rooms and always contain exactly **one Portal Room**.
- The layout branches like a tree from the starter staircase. Each branch can lead deeper or terminate at a dead end.
- **Libraries are always dead ends.** Do not follow a library corridor expecting to find the portal room beyond it.
- **Crossroads and corridors** are part of the main network. Prioritize following these.
- The portal room is typically **deeper and further** from the entrance — it is rarely found at the first junction you encounter.

---

## Finding the Portal Room

This is the most skill-intensive part of stronghold navigation. There are two complementary methods experienced runners use.

---

### Method 1: The Subtitles / Silverfish Method

This is the most reliable in-game tool for locating the portal room.

**Setup:** Go to **Options → Accessibility → Show Subtitles: ON**. This makes all nearby game sounds appear as text on the right side of your screen.

**How it works:**
- The Portal Room contains a **Silverfish Spawner** block.
- Silverfish spawners emit a faint hissing sound that appears in subtitles as **"Silverfish hisses"** or similar text.
- When you see silverfish hissing in your subtitles, the portal room is **nearby** — usually within 10–20 blocks through walls.

**Steps:**
1. Navigate the stronghold normally.
2. Watch the right side of your screen for the silverfish subtitle.
3. Once it appears, begin **mining through walls** in the direction you believe the sound is coming from.
4. You can confirm you are getting closer when the subtitle text frequency increases.

> [!TIP]
> Subtitles do not show directional arrows in all Minecraft versions used in MCSR Ranked. Learn to roughly estimate direction by moving toward or away from the subtitle trigger and noting whether it appears more or less frequently.

---

### Method 2: Pie Chart Navigation (F3 Menu)

The **Debug Pie Chart** (accessed via **F3 + Shift**) is an advanced technique used at the surface *before* entering the stronghold, to orient yourself toward the portal room's general direction.

**How it works:**
- When you are standing near (or above) the stronghold, the pie chart renders game processes.
- Experienced runners read the **"% minecraft:end_portal"** slice of the pie chart to determine the relative direction to the End Portal block.
- By rotating your character and watching the pie chart slice, you can determine the portal room's bearing.

**Steps:**
1. Before digging in, open F3 + Shift.
2. Rotate slowly until the End Portal slice of the pie chart is maximized.
3. This gives you a general heading — the portal room is roughly in that direction underground.
4. Mentally note this heading as you navigate the stronghold interior.

> [!NOTE]
> The pie chart method takes practice. It is most useful combined with the subtitles method — use pie chart on the surface for broad orientation, then subtitles inside for precise location.

---

### Navigation Priority: Follow the Main Path

The most important rule of stronghold navigation is **avoiding dead ends**.

- **Avoid libraries** unless the starter staircase room connects directly to one (that library will be a dead end regardless; note its location and backtrack immediately).
- **Follow corridors and crossroads** — these are part of the main structural branch.
- At any junction, prefer to go **forward or downward**. The portal room tends to generate deeper in the stronghold.
- **Don't explore every room.** In a speedrun, you are not looking for loot — you are looking for the portal.

---

### The 5-Way Crossing

The **5-way crossing** is the most significant room in any stronghold. It is a large stone brick junction with passages leading in multiple directions — typically 5 exits (hence the name).

- The portal room is **statistically likely to be accessible from one of the branches of the 5-way crossing**.
- When you reach a 5-way crossing, use your subtitles to check for silverfish hissing from each direction before committing to a path.
- Look for **descending staircases** leaving the 5-way crossing — the portal room is usually down, not up.

---

### The Silverfish Spawner as an Indicator

Even without subtitles enabled, you may see a **silverfish spawner** before the portal room itself. The spawner looks like a cage-like block with an animated silverfish inside. If you spot this block while navigating, the portal room entrance is directly behind or to the side of it.

- Do not break the spawner during navigation — this wastes time.
- More critically: **do not mine silverfish-infested stone** (infested stone bricks) near the portal room entrance. Doing so will trigger a silverfish swarm (see [Common Mistakes](#common-mistakes)).

---

## The Portal Room

The Portal Room is the terminal room of the stronghold and your final destination. It is unmistakable once you find it.

### Appearance

- The room is a **large, multi-level chamber** built almost entirely of stone brick.
- A **lava pit** fills the lower section of the room.
- In the center, hovering over the lava, is the **End Portal frame** — a ring of 12 End Portal Frame blocks arranged in a 3×3 square (with empty corners).
- Underneath the portal frame (accessible by a small staircase), is the **Silverfish Spawner**.
- The entrance to the room is through a **wooden door** at the top of a staircase.

### Key Visual Cues

- **Lava glow:** The lava pool beneath the portal is visible from the doorway.
- **End Portal Frame blocks:** Greenish-grey blocks with a starry texture. Any that already contain an Eye of Ender will glow with a green light on their top face.
- **Silverfish Spawner:** Located at the base of the platform, below the frame level.

---

## Filling the End Portal

### How Many Eyes Do You Need?

The End Portal has **12 frame blocks**, each of which may or may not already contain an Eye of Ender. In MCSR Ranked seeds:

- Seeds are **verified** to be completable — all 12 frames are guaranteed to be fillable.
- On average, **4 to 8 frames are already filled** in typical seeds, meaning you only need to place a few Eyes.
- In rare cases, you may need to fill all 12. Always carry at least **10–12 Eyes of Ender** when heading to the stronghold.

### Placing Eyes of Ender

1. Equip your Eyes of Ender (hotbar).
2. **Right-click each empty frame block** while looking at it. Empty frames look like solid stone with a greenish tint but no inner glow. Filled frames emit a green light from their top face.
3. You do not need to place them in any particular order.
4. Once all 12 frames are filled, the portal activates: a swirling **black portal texture** appears in the center.

> [!IMPORTANT]
> Make sure you are **not sneaking** when filling frames — it is easy to accidentally look at the lava or the floor. Stand at the edge of the platform and look slightly upward toward each frame block.

### Jumping Into the Portal

- Once activated, simply **walk or jump** into the swirling portal texture.
- You will be transported to The End instantly. The run timer **does not stop here** — the dragon fight begins immediately.
- Do not fall into the lava while filling the portal. Position yourself carefully on the stone brick platform.

---

## Common Mistakes

### Getting Lost in the Stronghold

- **Symptom:** Wandering in circles, revisiting the same corridors.
- **Fix:** Use subtitles. Follow the main corridor system — corridors and crossroads, not dead-end wings. When in doubt, move downward.

### Going Into Library Dead Ends

- **Symptom:** Walking into a large room with bookshelves and cobwebs, then having to backtrack.
- **Fix:** Learn to recognize a library entrance (bookshelves visible through the door). Unless you entered the stronghold through a library, turn around immediately. Libraries do not connect to the portal room.

### Breaking Silverfish-Infested Stone

- **Symptom:** Mining stone bricks near the portal room, accidentally releasing a silverfish, triggering a swarm.
- **Fix:** Near the portal room (especially if you are cutting through walls using the subtitles method), mine **carefully**. If a silverfish appears, do not mine any more blocks nearby — attack the silverfish and let it die before continuing. Never hit infested stone repeatedly.
- Silverfish swarms slow you down and deal consistent damage. They are one of the most time-costly surprises in any run.

### Not Using Subtitles

- **Symptom:** Taking 2+ minutes to find the portal room.
- **Fix:** Enable subtitles before every run. It takes 3 seconds in the options menu and saves tens of seconds in the stronghold.

### Running Out of Eyes of Ender

- **Symptom:** Reaching the portal room only to find many empty frames and not enough Eyes to fill them.
- **Fix:** Always craft and carry **10–12 Eyes of Ender** before entering the stronghold. In most runs you won't need all of them, but some seeds have many empty frames.

### Falling Into the Lava Pit

- **Symptom:** Falling off the platform while filling frames, dying in lava.
- **Fix:** Move slowly and deliberately on the portal platform. Sneak (Shift) when near the edge. Fill frames from a safe, stable position.

---

## Tips & Tricks

- **Memorize the library door frame.** Libraries have a distinctive taller entrance frame with a door. Recognizing it from a distance saves you the time of walking up to it.

- **Use your F3 coordinates.** If you noted the X/Z chunk coordinates of the stronghold from Ninjabrain Bot, compare them to your F3 display as you navigate — you can roughly tell if you are moving toward the center of the stronghold structure.

- **Don't mine unless you have to.** The fastest stronghold navigation involves running through open corridors, not mining through walls. Only mine when the subtitles method indicates you are very close and the route through corridors is unclear.

- **Practice stronghold-only seeds.** Many practice seeds exist where the runner spawns near or inside a stronghold. Use these to practice navigation without needing to complete a full run.

- **Speedrun.com and MCSR Ranked Discord have portal room seed databases.** Knowing common portal room placements for popular seeds can eliminate stronghold navigation entirely in favorable cases.

- **The portal room is always at a lower elevation.** Don't search for it on the upper levels of the stronghold — focus your effort on the lower corridors.

- **Right-clicking frames is faster than sneaking and placing.** Stand at a comfortable distance and right-click all empty frames in a single sweep of your mouse. Don't reposition for every single frame unless necessary.

- **Sound on is mandatory.** Even without subtitles, the hissing silverfish sound is audible. Train your ear to recognize it even in the middle of combat sounds.

- **The pie chart + subtitles combo is elite-level.** Using the pie chart on the surface to orient yourself, then subtitles underground for confirmation, is the fastest consistent method used by top MCSR Ranked players.

- **Don't open every door.** Prison cell rooms and short corridors that clearly dead-end don't need to be explored. Peek through the door and if you see iron bars or a dead-end wall, move on.

---

*This article is part of the [MCSR Ranked Wiki](https://wiki.mcsrranked.com). For related content, see [Locate Stronghold / Blind Travel](./endgame_locate_stronghold.md) and [Dragon Fight](./endgame_dragon_fight.md).*
