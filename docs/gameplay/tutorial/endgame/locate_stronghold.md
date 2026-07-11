# Locate Stronghold / Blind Travel

> **Goal:** Determine the location of the stronghold as quickly as possible — either by triangulating with Eyes of Ender, using Blind Travel (BT), or a combination of both — and dig down to enter it.

---

## Table of Contents

1. [Introduction](#introduction)
2. [Crafting Eyes of Ender](#crafting-eyes-of-ender)
3. [Ninjabrain Bot Overview](#ninjabrain-bot-overview)
4. [The Standard Eye Triangulation Method](#the-standard-eye-triangulation-method)
5. [Blind Travel (BT)](#blind-travel-bt)
6. [Digging to the Stronghold](#digging-to-the-stronghold)
7. [Common Mistakes](#common-mistakes)
8. [Tips & Tricks](#tips--tricks)

---

## Introduction

Finding the stronghold is the **critical bridge** between the Nether segment and the End Portal. How efficiently you locate the stronghold — and reach its portal room — determines a huge chunk of your final time. Even a 30-second improvement here can push your ranking significantly in MCSR Ranked.

There are two primary strategies for locating the stronghold:

| Method | Description | Skill Level |
|---|---|---|
| **Eye Triangulation** | Throw Eyes of Ender, watch where they fly, use Ninjabrain Bot to calculate the stronghold position | Beginner–Intermediate |
| **Blind Travel (BT)** | Travel toward where strongholds statistically generate before throwing Eyes, saving throws and time | Intermediate–Advanced |

Both methods ultimately converge: you always confirm the stronghold position with at least 1–2 Eye throws before digging. The difference is *when and where* you throw them.

### Key Tool: Ninjabrain Bot

**Ninjabrain Bot** is an external overlay tool that virtually all MCSR Ranked players use. It uses Bayesian probability calculations based on your position and the angle your thrown Eye travels to triangulate the most likely stronghold chunk. It is **legal to use** in MCSR Ranked runs.

This guide assumes you are using Ninjabrain Bot. Playing without it is technically possible, but significantly slower and less accurate.

---

## Crafting Eyes of Ender

### Recipe

```
[ Blaze Powder ] + [ Ender Pearl ] = [ Eye of Ender ]
```

- **1 Blaze Powder** + **1 Ender Pearl** = **1 Eye of Ender**
- Crafted in a 2×2 or 3×3 crafting grid — no specific spatial layout required.

### How Many to Craft

| Scenario | Eyes Recommended |
|---|---|
| Standard run (BT not used) | 10–12 |
| Blind Travel run | 10–12 |
| Very experienced / known easy seed | 8–10 |

Always craft at least **10 Eyes of Ender**. Here is why:

- **2–4 Eyes** will be thrown during triangulation. Each throw has an approximately **80% chance of the Eye returning** to be picked up, and a **~20% chance of it shattering** permanently.
- **Up to 12 Eyes** may be needed to fill empty End Portal frames in the portal room.
- Crafting fewer than 10 risks running out at the portal room, costing you a reset.

### When to Craft Them

Craft Eyes of Ender **after exiting the Nether**, during the transition back to the overworld. This is the most natural time — you have already gathered Blaze Rods (converted to Blaze Powder) and Ender Pearls during your Nether run. Do not waste overworld time crafting; do it during loading screens or immediately upon exiting the Nether portal.

> [!TIP]
> If your inventory is full, quickly reorganize before crafting. It is common to bulk-craft: turn all your Blaze Rods into Blaze Powder at once, then combine with all your Ender Pearls in a single crafting session.

---

## Ninjabrain Bot Overview

### What Is Ninjabrain Bot?

**Ninjabrain Bot** is a free, open-source program created by the MCSR community. It reads your game's F3 debug output and, when you throw an Eye of Ender, it captures your exact position and the angle of the Eye's flight path. It then applies **Bayesian inference** across all possible stronghold chunk positions to calculate a probability distribution of where the stronghold is located.

- **Download:** [github.com/Ninjabrain1/Ninjabrain-Bot](https://github.com/Ninjabrain1/Ninjabrain-Bot)
- **Format:** A small overlay window that sits on top of your Minecraft window.
- **Legal status:** Fully permitted in MCSR Ranked.

### Installation and Setup

1. Download the latest `.jar` release from the GitHub releases page.
2. Run it with Java: `java -jar NinjabrainBot.jar` — or double-click if Java is configured correctly.
3. In the bot's settings, configure:
   - **Sigma value:** This represents your expected aiming error in degrees. Set it to match your mouse sensitivity using the in-app calibration tool.
   - **Allow manual input:** Enable this if you want to type coordinates manually instead of using clipboard capture.
4. Set Minecraft to **Windowed Mode** so Ninjabrain Bot can overlay on top of it.
5. Ensure the **F3 debug screen** is accessible in-game.

### Input Method: F3+C (Recommended)

The fastest and most accurate way to feed data into Ninjabrain Bot:

1. Throw an Eye of Ender.
2. **Immediately** aim your crosshair at the Eye's trajectory — along the line the Eye is flying toward the horizon.
3. Press **F3+C** — this copies your exact X, Y, Z coordinates and your exact horizontal viewing angle (the `f:` value from the debug screen) to your clipboard.
4. Ninjabrain Bot reads this clipboard data automatically and instantly updates its prediction.

> [!IMPORTANT]
> The accuracy of Ninjabrain Bot depends entirely on how precisely you align your crosshair with the Eye's direction of travel. Look **directly along the Eye's flight path** — not at the Eye itself, but along the projected line it travels toward the horizon.

### Manual Input Method

If F3+C is not working (some Java installs block clipboard access):

1. Open F3 manually.
2. Note the exact values for `XYZ` and `f:` (the facing direction in degrees).
3. Type these values into Ninjabrain Bot's manual input fields.

This method is slower but produces identical results if done accurately.

### What Ninjabrain Bot Outputs

After each throw, the bot displays:

| Output | Meaning |
|---|---|
| **Most Likely Chunk** | The chunk (X, Z) where the stronghold is most probably located |
| **Confidence %** | How certain the bot is about that specific chunk prediction |
| **Error Ring** | A visual radius showing where the stronghold could realistically be |
| **Distance** | How far you are (in blocks) from the predicted chunk |
| **Overworld Direction** | The compass bearing to walk toward the stronghold |

### When to Dig: Confidence Thresholds

| Confidence | Recommended Action |
|---|---|
| Below 50% | Do not dig yet — throw again from a new position |
| 50–80% | Move further and throw once more to refine |
| **85%+** | Safe to start digging |
| **95%+** | Very high confidence; dig immediately |

Most experienced runners wait for **85–90% confidence** before digging. With 2 well-placed throws from at least 200 blocks apart, this is consistently achievable.

---

## The Standard Eye Triangulation Method

This is the baseline method all runners learn first. It works in all conditions and requires no prior knowledge of stronghold ring positions.

### Step-by-Step

#### Throw #1 — Establish Direction

1. After exiting the Nether and crafting your Eyes, find a flat open area. Avoid trees or tall terrain that could obstruct your view of the Eye's flight.
2. **Throw one Eye of Ender** by right-clicking with it selected in your hotbar.
3. The Eye will float upward and then begin flying horizontally in the direction of the stronghold before falling.
4. Watch carefully — the Eye travels toward the stronghold.
5. **Aim your crosshair along the Eye's exact travel direction** (not at the Eye — along its projected horizontal line of flight toward the horizon).
6. Press **F3+C** to copy your coordinates and angle to the clipboard.
7. Ninjabrain Bot updates automatically. Note the predicted chunk and confidence level (typically 20–50% after one throw).
8. If the Eye returns (approximately 80% chance), run to it and pick it up for reuse.

#### Moving Between Throws

After Throw #1:

- **Run 200–300 blocks** in the direction the Eye pointed. This baseline separation is critical — if you throw again from nearly the same spot, the angular difference between throws will be too small for accurate triangulation.
- Move primarily along the stronghold's direction. Slight lateral adjustments are fine but not necessary.
- Sprint continuously. Eat food while running to maintain health and hunger.

#### Throw #2 — Triangulate

1. From your new position, throw another Eye of Ender.
2. Aim your crosshair precisely along the Eye's new flight direction.
3. Press **F3+C**.
4. Ninjabrain Bot cross-references the two angle measurements and dramatically narrows down the possible stronghold location.
5. Confidence typically jumps to **70–90%** after a well-placed second throw that is far enough from the first.

#### Throw #3 (If Needed)

If confidence remains below 85% after Throw #2, move another 100–200 blocks along the predicted direction and throw again. Three well-placed throws will reliably reach 90%+ confidence in virtually all situations.

### When the Eye Goes DOWN — You Are There

One of the most important signals in the triangulation process: **if a thrown Eye immediately moves downward rather than flying horizontally**, you are standing directly above — or very near — the stronghold.

- This happens because the stronghold position is below your feet, causing the Eye to point downward rather than outward.
- When this occurs: **look at your Ninjabrain Bot coordinates, confirm the chunk, and start digging immediately**.
- Do not throw another Eye to "double check." A downward Eye is a definitive confirmation.

> [!IMPORTANT]
> A downward Eye is a clear signal. Throwing additional Eyes at this point wastes time and risks shattering them. Trust Ninjabrain Bot's chunk prediction and dig.

### Stronghold Depth Reference

Strongholds generate at approximately **Y=40 to Y=55** in most seeds, measured at the portal room floor level. When planning your dig:

- From sea level (Y=63): expect to dig **~10–25 blocks** to reach the top of the stronghold.
- From elevated terrain (Y=80+): expect to dig **~30–45 blocks**.
- Mountainous biomes may push this deeper. Do not give up if you haven't hit stone bricks by Y=50 — keep going to Y=30–35 before reconsidering your position.

---

## Blind Travel (BT)

### What Is Blind Travel?

**Blind Travel** is the technique of traveling a significant distance toward the likely stronghold location *before* throwing any Eyes of Ender. The core insight is that strongholds do not generate at completely random X/Z coordinates — they generate in **specific concentric rings** around the world's origin point (0, 0).

By traveling into the correct ring before throwing Eyes, you:
- Reduce the number of throws needed (you are already close to the stronghold).
- Save time compared to throwing from your Nether exit point.
- Use fewer Eyes (fewer shattering opportunities).

For experienced players, BT saves **30–60 seconds** per run compared to throwing from wherever you exit the Nether.

### The Stronghold Ring System

Minecraft generates strongholds in concentric rings centered on 0, 0. The relevant ring for MCSR Ranked is almost always the **first ring**:

| Ring | Distance from Origin (Overworld blocks) | Number of Strongholds |
|---|---|---|
| **Ring 1** | 1,280 – 2,816 blocks | **3 strongholds** |
| Ring 2 | 4,352 – 5,888 blocks | 6 strongholds |
| Ring 3 | 7,424 – 8,960 blocks | 10 strongholds |
| Rings 4–8 | Progressively farther | Progressively more |

In virtually every MCSR Ranked run, the target stronghold is in **Ring 1**, between 1,280 and 2,816 overworld blocks from (0, 0). Rings 2 and beyond are not practically relevant in normal play.

### The Blind Travel Math

The core principle of BT is dead simple:

1. **Exit the Nether.** (Your Nether coordinates × 8 = your Overworld coordinates.)
2. Open F3 and check your overworld X and Z coordinates.
3. **Sprint toward (0, 0)** — or in the direction your initial Eye will point — until you are approximately **1,500–2,000 blocks from the origin**.
4. **Throw your Eyes** from there. You are now inside or very near Ring 1, so 1–2 throws typically achieve high confidence.

**Example:**

- You exit the Nether at Nether coordinates X=700, Z=200.
- Overworld equivalent: X=5,600, Z=1,600. Distance from origin ≈ 5,825 blocks — that is Ring 2 territory.
- Instead of throwing immediately, you sprint toward 0,0 for ~60–90 seconds.
- At overworld position X=1,800, Z=400 (distance ≈ 1,844 blocks), you are inside Ring 1.
- You throw. One or two throws later, Ninjabrain Bot shows 90%+ confidence.

### Practical BT Execution

1. **Exit the Nether** and open F3 immediately. Note your X and Z coordinates.
2. **Estimate your distance** from (0, 0). You don't need exact math — rough estimation by eye is sufficient with practice.
3. **Head toward (0, 0)** at full sprint. Use a boat on water, sprint on land.
4. When you are approximately **1,500–2,000 blocks from origin**, throw your first Eye of Ender.
5. Follow Ninjabrain Bot's direction. One to two additional throws will usually finalize your position.
6. Begin digging when confidence exceeds 85%.

> [!TIP]
> You don't need to run directly toward (0, 0) in a straight line. The three Ring 1 strongholds are spaced roughly 120° apart around the ring. Let your first Eye throw guide you toward the nearest one — just get into the ring first, then follow the Eye.

### Why Divine Travel Does Not Work in MCSR Ranked

**Divine Travel** is a technique used in **Set Seed** speedrunning where the runner already knows the exact world seed. They can pre-calculate the stronghold's precise chunk coordinates using external tools and travel directly to it — no Eye throws needed at all.

In **MCSR Ranked**, seeds are **randomly generated and unknown** to the player before each run begins. There is no pre-run seed knowledge, no pre-calculation, and therefore no Divine Travel. You must always throw at least one Eye of Ender to locate the stronghold in MCSR Ranked.

### The Boat Eye Technique (Advanced)

For runners seeking maximum angular precision, the **Boat Eye** technique stabilizes your camera for more accurate Ninjabrain Bot inputs.

**Why it works:** When sitting in a boat, your camera rotation moves in discrete, stabilized increments rather than free-floating. This makes it significantly easier to align your crosshair *exactly* along the Eye's travel vector, reducing the angular error fed into Ninjabrain Bot and improving confidence from fewer throws.

**How to execute:**

1. Place a boat on flat ground or water.
2. **Enter the boat** (right-click).
3. Throw the Eye of Ender.
4. While still seated in the boat, **slowly rotate** your view to align your crosshair precisely along the Eye's flight path toward the horizon.
5. Press **F3+C** when perfectly aligned.
6. **Exit the boat** (Shift key), pick it up if needed, and continue.

**When to use it:**

- When you want 90%+ confidence from a single throw.
- On flat terrain or near water where boat placement is quick and easy.
- Not worth the setup time on steep mountainous terrain or dense forest.

> [!NOTE]
> The boat eye technique adds approximately 3–5 seconds of setup overhead but can return 95%+ confidence from one throw. At high-level play where every second counts, this trade-off is frequently worth it — especially when combined with Blind Travel, where you are already in Ring 1 and one precise throw is all you need.

### BT vs Standard Throws: When to Use Which

| Situation | Recommended Method |
|---|---|
| Exit Nether very far from origin (>5,000 OW blocks) | **Blind Travel** |
| Exit Nether near origin (<2,000 OW blocks) | **Standard throws** — already in range |
| Beginner runner | **Standard throws** — simpler to execute correctly |
| Intermediate / Advanced runner | **BT** for the time save |
| Large ocean between you and origin | Boat across, then BT or standard |
| Mountainous terrain everywhere | Either; judge by terrain and distance |

---

## Digging to the Stronghold

### Optimal Digging Angle

Always dig at a **45-degree staircase angle** — one block forward and one block down alternating. Never dig straight down. The staircase approach:

- Exposes a wider cross-section of underground terrain as you descend.
- Prevents you from falling into lava, caves, or dangerous stronghold rooms.
- Allows lateral movement if you need to adjust your position.

Visually:

```
█         ← surface (Y≈63)
 █
  █
   █
    █     ← expected stronghold range (Y=40–55)
```

### What to Look For While Digging

Watch the walls and floor of your staircase for these block types:

| Block | Meaning |
|---|---|
| **Stone Bricks** (regular) | Stronghold confirmed |
| **Mossy Stone Bricks** | Stronghold (common near water) |
| **Cracked Stone Bricks** | Stronghold |
| **Chiseled Stone Bricks** | Stronghold |
| **Stone Brick Slabs** | Stronghold floor or staircase |
| **Iron Bars** | Prison cell room of the stronghold |
| **Bookshelves** | Library — you've entered from the side |

The moment you see **any stone brick variant**, you have hit the stronghold. Stop digging your staircase and begin navigating horizontally to explore the structure.

### The Entrance Room Generation

When you break into the stronghold, the room you enter depends entirely on where your staircase intersected the structure. Common scenarios:

- **Corridor entry:** You enter a long hallway. This is the most common entry. Begin navigating according to the Stronghold Navigation guide.
- **Library entry:** You have entered from the side of a library. These are dead ends — exit through the door you find (or dig through) and locate the main corridor network.
- **Starter staircase entry:** The ideal entry; a natural staircase descends in front of you. Follow it down.

> [!NOTE]
> There is no "correct" entry point. Wherever you break in is your starting point. Refer to the [Stronghold Navigation](./endgame_stronghold.md) guide for routing from any room type.

### What If You Miss?

If you dig to Y=30 without hitting stone bricks:

1. **Recheck Ninjabrain Bot.** Confirm you are in the correct chunk. If your position drifted, the bot will show you how far you are from the predicted chunk.
2. **Dig laterally** toward the center of the predicted chunk before going deeper.
3. **Throw one more Eye** from underground if needed — it will fly through the ceiling and give you a fresh direction reading.
4. Do not give up until you have checked thoroughly. Strongholds can be at unusual depths near mountains or ocean floors.

---

## Common Mistakes

### Not Using Ninjabrain Bot

- **Symptom:** Throwing many Eyes in inconsistent directions, guessing the stronghold location by eye, losing 1–2 minutes at this phase.
- **Fix:** Install and configure Ninjabrain Bot before your first MCSR Ranked run. It is an industry-standard community tool, universally used at all competitive levels. Running without it is a structural disadvantage.

### Throwing Too Many Eyes (Shattering Risk)

- **Symptom:** Running out of Eyes before filling all portal frames because too many were used on triangulation.
- **Fix:** Each throw is an ~20% shattering risk. Poor crosshair alignment wastes throws and Eyes. Practice aiming precisely, use the boat eye technique for guaranteed accuracy, and craft 10–12 Eyes at minimum so that even a few shatters don't leave you short.

### Moving Too Little Between Throws

- **Symptom:** Ninjabrain Bot shows only marginal improvement in confidence between Throw #1 and Throw #2.
- **Fix:** Move at least **200–300 blocks** between any two throws. Two throws from nearly the same position produce nearly the same angle reading — the triangulation improvement is minimal. Distance between throw points is the single most important factor in triangulation accuracy.

### Not Knowing Stronghold Depth

- **Symptom:** Digging to Y=20 without hitting the stronghold, losing 30+ seconds, becoming confused.
- **Fix:** Know that strongholds are typically at **Y=40–55**. If you've reached Y=35 without stone bricks, you've almost certainly drifted from the target chunk. Stop and recheck Ninjabrain Bot before digging further.

### Throwing Eyes Before Exiting the Nether

- **Symptom:** Wasting Eyes or losing time by throwing prematurely before the Nether exit.
- **Fix:** Craft and throw Eyes **after** exiting the Nether, not before. You can't triangulate an overworld structure from inside the Nether.

### Ignoring the Eye Going Downward

- **Symptom:** Eye goes down → player runs further and throws again unnecessarily, wasting time and an Eye.
- **Fix:** A downward Eye means you are above the stronghold. **Dig immediately**. No additional throws are needed or beneficial.

### Poor Camera Alignment at F3+C

- **Symptom:** Ninjabrain Bot shows an unusually large error margin or the prediction is wildly inconsistent between throws.
- **Fix:** Practice aiming along the Eye's trajectory vector before pressing F3+C. The Eye travels in a straight horizontal line from your position. You need to look along that exact line to the horizon — not roughly in the right direction, but precisely.

---

## Tips & Tricks

- **Configure Ninjabrain Bot's sigma value carefully.** The sigma represents your expected aiming error in degrees. Too low and the bot will be overconfident in imprecise data. Too high and it requires many more throws to converge. Use the built-in calibration tool with your actual mouse sensitivity settings.

- **Practice throwing Eyes in a Creative world.** Set up a flat creative world with a command-spawned stronghold and practice the throw → aim → F3+C → check bot workflow until it is automatic muscle memory. Do it dozens of times.

- **Know your overworld distance at all times.** From the Nether, your position ÷ 8 = overworld position. Knowing your overworld distance from origin *before exiting the Nether* lets you pre-plan your BT route.

- **Sprint immediately after throwing.** You can throw an Eye, turn to aim, press F3+C, then immediately start sprinting toward the indicated direction — all as a seamless motion. Practice this flow until you lose no movement time per throw.

- **Pick up returned Eyes whenever safe.** After throwing, the Eye has an ~80% chance to return and float above the ground briefly. Run to it and pick it up. Over multiple throws, this recycles your Eyes and preserves your supply.

- **Use a boat on oceans.** If your BT route crosses a large ocean biome, a boat is dramatically faster than swimming. Always be ready to craft one (5 matching wood planks in a U shape in the crafting grid).

- **Ninjabrain Bot has a precision travel mode.** At high confidence (usually 90%+), the bot displays exact block-level coordinates of the stronghold's predicted chunk center. Navigate directly to those coordinates before digging for maximum precision.

- **The 3 Ring 1 strongholds are ~120° apart.** If one Eye throw shows the stronghold far to the left of 0,0, you are being directed toward one of the three. Subsequent throws will confirm exactly which one. This knowledge helps you mentally confirm BT direction.

- **In MCSR Ranked, stronghold time loss compounds.** Extra time spent here means fighting the dragon later, under more time pressure, with less favorable resource timing. Treat stronghold location as a high-priority optimization target — even 20–30 seconds of improvement here is highly valuable.

- **Learn to read Ninjabrain Bot's error radius visually.** A large error ring means your throws are not giving enough information. A small, tight ring means you are converging rapidly. The ring size helps you decide whether one more throw is worthwhile.

- **After digging in, mark your entry point.** Place a distinctive block (like a torch or colored wool) where you broke through. If you need to backtrack during stronghold navigation, having a marked entry point prevents disorientation.

---

## Quick Reference Cheat Sheet

```
═══════════════════════════════════════════
         STRONGHOLD LOCATION FLOW
═══════════════════════════════════════════

AFTER NETHER EXIT:
  1. Craft all Eyes of Ender (10-12)
  2. Check F3 → note X,Z → estimate distance from (0,0)
  3. If far (>3,000 blocks): SPRINT toward 0,0 first [BT]
  4. When ~1,500-2,000 blocks from origin: THROW Eye #1
  5. Aim precisely along Eye's travel vector → F3+C
  6. Check Ninjabrain Bot confidence
  7. Sprint 200-300 blocks in indicated direction
  8. THROW Eye #2 → aim → F3+C
  9. If confidence >85%: STOP AND DIG
 10. If Eye goes DOWN at any point: DIG IMMEDIATELY

DIGGING:
  - 45-degree staircase (never straight down)
  - Target depth: Y=40-55
  - Look for stone brick variants
  - Once inside: see Stronghold Navigation guide
═══════════════════════════════════════════
```

---

*This article is part of the [MCSR Ranked Wiki](https://wiki.mcsrranked.com). For related content, see [Stronghold Navigation](./endgame_stronghold.md) and [Dragon Fight](./endgame_dragon_fight.md).*
