# Buried Treasure — Overworld Strategy

> [!NOTE]
> This page covers the **Buried Treasure** overworld seed type used in MCSR Ranked. If you are looking for other overworld strategies, see [Village](./overworld_village.md), [Shipwreck](./overworld_shipwreck.md), or [Ruined Portal](./overworld_ruined_portal.md).

---

## Table of Contents

1. [Introduction](#introduction)
2. [MCSR Ranked Seed Guarantees](#mcsr-ranked-seed-guarantees)
3. [How Buried Treasure Seeds Work](#how-buried-treasure-seeds-work)
4. [Buried Treasure Loot](#buried-treasure-loot)
5. [Step-by-Step Strategy](#step-by-step-strategy)
6. [After the Treasure](#after-the-treasure)
7. [Ocean Biome Challenges](#ocean-biome-challenges)
8. [Building the Portal](#building-the-portal)
9. [Inventory Checklist](#inventory-checklist)
10. [Tips & Tricks](#tips--tricks)

---

## Introduction

**Buried Treasure** is one of the more advanced overworld seed types in MCSR Ranked. These seeds generate the player near a buried treasure chest hidden beneath the ocean floor (or occasionally a beach), providing a reliable early-game iron and food source without needing to explore a shipwreck or village.

### Elo Distribution

Buried treasure seeds are gated behind a relatively high Elo threshold. They only appear in the seed pool for experienced players:

| Elo Range   | Buried Treasure Chance |
|-------------|------------------------|
| 0 – 599     | 0%                     |
| 600 – 1199  | 0%                     |
| 1200+       | ~20%                   |

This means you will **not** encounter buried treasure seeds until you have climbed past 1200 Elo. At that point, roughly one in five of your runs may start with a buried treasure spawn. Because of this, buried treasure is considered a **high-Elo seed type** and requires a more practiced routing mindset than the beginner-friendly village or shipwreck starts.

### Why Are They High-Elo Seeds?

Buried treasure seeds are classified as high-Elo for several reasons:

- **Ocean biome start:** You often spawn with no wood nearby, requiring quick adaptation.
- **Underwater navigation:** Finding and digging up the chest requires comfort with underwater movement and breath management.
- **Routing flexibility required:** Unlike village seeds with clear structures, buried treasure demands confident F3 coordinate usage and efficient decision-making after looting.
- **Higher execution ceiling:** A good player extracts significant time saves from a buried treasure seed; a struggling player may drown, run out of food, or waste time aimlessly swimming.

### Buried Treasure vs. Shipwreck

Both seed types involve ocean exploration, but they differ substantially:

| Feature                   | Buried Treasure         | Shipwreck                    |
|---------------------------|-------------------------|------------------------------|
| Structure type            | Underground chest       | Partially submerged ship     |
| Navigation method         | F3 coordinates          | Visual spotting              |
| Wood access               | Usually none nearby     | Shipwreck provides planks    |
| Iron source               | Chest loot (ingots)     | Chest loot (ingots/armor)    |
| Food source               | Chest loot (fish)       | Chest loot (suspicious stew) |
| Breath management         | Critical — long dives   | Easier — air pockets inside  |
| Execution difficulty      | Higher                  | Moderate                     |

---

## MCSR Ranked Seed Guarantees

MCSR Ranked uses a **filtered seed pool** — every seed in the rotation has been pre-screened to guarantee specific conditions at spawn. For buried treasure seeds, the following are guaranteed:

- **Buried treasure chest spawns within a short distance of spawn** — you will never have to travel hundreds of blocks to reach it.
- **The chest is accessible underwater** — it will not be buried in a location that is unreachably deep or obstructed by unusual terrain.
- **Sufficient iron and food** in the chest to enable a nether portal (see loot section below).
- **A lava pool exists within a reasonable distance** of the treasure location (or can be found via cave/ravine nearby), enabling portal construction without requiring a nether fortress lava detour.
- The seed is verified to be **completable** — every MCSR Ranked seed has a viable route from spawn to credits.

> [!IMPORTANT]
> MCSR Ranked seeds are **not vanilla random seeds**. They are curated. This means some vanilla buried treasure frustrations (e.g., no lava pool for miles, chest spawning at Y=20 under solid stone) do not apply here.

---

## How Buried Treasure Seeds Work

### Vanilla vs. MCSR Ranked

In **vanilla Minecraft**, buried treasure chests are found by:
1. Locating a shipwreck or ocean ruins.
2. Finding a treasure map inside.
3. Following the map to an **X mark** on the map image.
4. Digging at that X mark to find the chest.

In **MCSR Ranked**, this whole map-reading step is bypassed. The seed pool is designed so that:

- You **spawn very close** to the buried treasure location — often directly on top of it or within visual range.
- You are expected to use **F3 coordinates** to navigate to the chest without needing a treasure map.
- The chest is almost always buried under **sand or gravel** at approximately **Y = 9** (just above bedrock level), directly beneath the ocean floor.

### Finding the Chest Without a Map

Because no map is required, your workflow is entirely coordinate-driven:

1. Open **F3** immediately upon spawning to orient yourself.
2. Identify the ocean or beach biome and swim/walk toward the known treasure location.
3. Use F3 X/Z coordinates to pinpoint the **chunk center** where treasure chests always spawn — buried treasure always generates at **X = chunkOrigin+9, Z = chunkOrigin+9** within its chunk (i.e., 9 blocks from the chunk's northwest corner).
4. Dive down, dig through sand/gravel, and retrieve the chest contents.

> [!TIP]
> Buried treasure always spawns at the **chunk's 9,9 position** (chunk-relative coordinates). If you know which chunk the treasure is in, press F3 and look for coordinates ending in **+9 within the chunk** to zero in on the exact dig spot. In practice on MCSR Ranked, the spawn location often puts you directly above or adjacent to the chest.

### Y-Level of the Chest

The chest spawns at the **first solid block** below the ocean floor surface, typically:
- **Y = 9** when under deep sand/gravel.
- Occasionally slightly higher if the ocean floor is shallower.
- Always **above Y = 5** (above typical bedrock).

You will rarely need to dig more than **4–6 blocks** straight down through sand or gravel before hitting the chest.

---

## Buried Treasure Loot

The buried treasure chest has a **fixed loot table** with weighted random rolls. Across MCSR Ranked seeds, you can expect the following items consistently:

### Always Present

| Item              | Quantity | Speedrun Use                          |
|-------------------|----------|---------------------------------------|
| Heart of the Sea  | 1        | ❌ Not useful for speedrunning         |
| Iron Ingot        | 1–5      | ✅ Critical — used for iron pickaxe/bucket |
| Cooked Cod        | 2–4      | ✅ Food for early game                 |
| Cooked Salmon     | 2–4      | ✅ Food for early game                 |

### Common Rolls

| Item             | Quantity | Speedrun Use                              |
|------------------|----------|-------------------------------------------|
| Gold Ingot       | 1–5      | ✅ Very useful — saves gold mining in nether |
| TNT              | 1–2      | ⚠️ Situationally useful (blasting lava)   |
| Emerald          | 4–8      | ❌ Not useful for speedrunning             |
| Prismarine       | 1–5      | ❌ Not useful for speedrunning             |
| Leather Tunic    | 1        | ❌ Not useful for speedrunning             |
| Chainmail Helmet | 1        | ❌ Not useful for speedrunning             |

### What Actually Matters

For a speedrun, you primarily care about:

1. **Iron Ingots** — You need at least **3 iron** minimum (for a bucket to carry lava). More iron lets you make a pickaxe and full-iron tools.
2. **Gold Ingots** — Any gold from the chest reduces your nether gold-mining workload significantly.
3. **Food** — The cooked fish provides enough saturation to sprint and stay alive through the early ocean sections.

> [!NOTE]
> The **Heart of the Sea** is guaranteed in every buried treasure chest but has **zero value** in a speedrun context. It is used to craft a Conduit, which requires materials you won't collect. Ignore it entirely.

> [!WARNING]
> **Do not take the Heart of the Sea**. It wastes an inventory slot. If your inventory is crowded, leave it in the chest.

---

## Step-by-Step Strategy

### Step 1 — Spawn and Immediate Identification

1. **Open F3 immediately** when you spawn. Note your X and Z coordinates.
2. Identify your biome — if you spawn on a **beach or in/near ocean**, a buried treasure seed is likely confirmed.
3. Look around for visible ocean. You do not need to identify the exact direction yet — just confirm the biome type.
4. If you spawned on land with a beach nearby, walk briskly toward the water.

> [!TIP]
> On some buried treasure seeds, you will spawn **directly on a beach** with the sand very close to the treasure. On others, you spawn in shallow water. Either way, begin moving toward the water immediately.

### Step 2 — Getting to the Treasure Location

1. **Sprint-swim** toward the known treasure location. On MCSR Ranked seeds, this is typically within **30–60 blocks** of spawn.
2. If you have not yet eaten, eat food from your hotbar if available (most seeds do not give you starter food, so prioritize retrieving the chest).
3. Navigate using **F3 coordinates**. Look at your X and Z values and move toward the chunk-9,9 position.
4. Do not waste time looking for structures — go straight to the coordinates.

### Step 3 — Diving and Breath Management

1. Once above the treasure location, **look down through the water** to identify the ocean floor.
2. **Dive straight down**. If the water is shallow (< 10 blocks), you can safely reach the bottom and return without drowning.
3. If the water is deep (> 15 blocks), you need to manage your **breath bar** carefully:
   - Dive, dig a few blocks, return to surface for air, then dive again.
   - Each dive, try to dig 2–3 blocks deeper into the sand/gravel column.
4. **Sprint-swimming** underwater (hold W + Space while swimming) is faster and helps you descend quickly.

> [!CAUTION]
> Watch your **breath bar** (the bubble icons above your health bar). If it hits zero, you begin taking drowning damage — 2 HP per second. Always resurface before the last 2–3 bubbles disappear.

### Step 4 — Digging to the Chest

1. Position yourself **directly above the treasure coordinates** (chunk X+9, Z+9).
2. Dig straight **downward** through sand or gravel. These blocks break fast with your fist — no tools required.
3. The chest will appear within **4–6 blocks** of digging. You will see its distinct wood-and-latch texture.
4. If you hit stone before finding the chest, you are likely **1–2 blocks off** horizontally. Shift your position slightly and try again.
5. Once exposed, **right-click the chest** to open it.

> [!NOTE]
> Sand and gravel are **gravity-affected blocks**. When you dig the block directly above the chest, sand/gravel may fall into the chest space. This is fine — the chest is protected and will not be crushed. Simply dig around the fallen blocks to expose the chest lid.

### Step 5 — Efficiently Looting the Chest

1. Open the chest and **immediately take iron ingots, gold ingots, and food** first.
2. If you have inventory room, take TNT (useful for lava pool creation if no natural pool is found).
3. **Leave behind:** Heart of the Sea, Prismarine, Leather armor (unless you have none), Emeralds.
4. Close the chest and immediately begin swimming back to the surface.
5. Eat cooked fish/salmon as soon as you surface to restore hunger and begin natural regeneration.

---

## After the Treasure

Once you have the chest loot, your next priorities are:

### 1. Get Wood (If You Haven't Already)

If you spawned in a pure ocean biome with no trees visible:
- Swim or walk toward the **nearest land mass** — usually visible on the horizon or within 50–100 blocks.
- You need **at least 3 wooden planks** for a crafting table and sticks.
- If there is a shipwreck nearby, you can break its planks for wood — check for one while navigating.

> [!TIP]
> Always scan the horizon as soon as you surface from the dive. Trees on a nearby island or coast are immediately identifiable by their green canopy. Sprint toward the nearest one as soon as the chest is looted.

### 2. Craft Basic Tools

With iron ingots from the chest:

```
Priority crafting order:
1. Crafting Table         (4 planks)
2. Wooden Pickaxe         (if no stone available yet) → Stone Pickaxe ASAP
3. Iron Pickaxe           (3 iron ingots + 2 sticks) — needed to mine gold/obsidian
4. Iron Bucket            (3 iron ingots) — needed for lava portal
5. Flint and Steel        (1 iron + 1 flint) — needed to light the portal
```

> [!IMPORTANT]
> You need **a minimum of 7 iron ingots** to craft both an iron pickaxe AND a bucket in one go. Buried treasure chests can provide this, but if you only got 3–4 iron, prioritize the **bucket** and use a wooden/stone pickaxe to mine more iron from a nearby cave.

### 3. Find a Lava Pool

The buried treasure chest does **not** provide lava — you still need to find lava to build your nether portal. On MCSR Ranked buried treasure seeds, lava is typically found via:

- **Surface lava pool** — visible on nearby land. Check beaches and plains biomes.
- **Cave or ravine** — dig into the nearest land mass and descend to Y = 10–12 for lava lakes.
- **Using TNT** from the chest to expose underground lava quickly.

### 4. Get More Food If Needed

The cooked fish from the chest (4–8 pieces total) may not be enough for the entire overworld section. If your hunger drops below half:
- Kill **nearby fish** with your hand or a sword.
- Cook them in a **furnace** (requires 8 cobblestone).
- Alternatively, look for **kelp** — smelted kelp provides a renewable food source when cooked.

---

## Ocean Biome Challenges

Buried treasure seeds disproportionately spawn players in ocean or beach biomes. This introduces several obstacles not present in land-based seed types.

### No Wood Nearby

This is the **most common challenge**. Solutions:

| Situation                       | Solution                                               |
|---------------------------------|--------------------------------------------------------|
| Island visible on horizon       | Sprint-swim there immediately after looting            |
| Shipwreck visible nearby        | Loot its lower chest AND break planks for wood         |
| No land visible at all          | Use F3 to navigate north/south until land appears      |
| Kelp forest nearby              | Use kelp as a landmark — land is usually adjacent      |

> [!TIP]
> In MCSR Ranked, seeds with buried treasure are curated to have land within a reasonable distance. If you see no trees, open F3 and watch the biome label in the top-left of the F3 readout as you move — it updates in real time and will show when you enter a land biome.

### Drowning Risk

Managing oxygen underwater is a core skill for buried treasure seeds:

- **Never** dive to the bottom if the water is >20 blocks deep without planning your ascent.
- On Java Edition, placing a **door** underwater creates a 1-block air space — craft one if you have wood before diving deep.
- The **Respiration** enchantment is not accessible this early, so rely entirely on breath management.
- Always make your last dive the one where you open and loot the chest — do not open the chest, run out of breath, and have to resurface mid-looting.

### Swimming Efficiency

- Use **sprint-swimming** (hold W + Space in water) at all times — it is significantly faster than regular swimming.
- **Dolphin's Grace** status effect (obtained by swimming near dolphins) greatly increases swim speed. If dolphins are nearby, swim alongside them to their benefit.
- Avoid swimming in a straight line on the surface if the destination is directly below — **dive at an angle** to cover horizontal distance while descending.

### No Immediate Food Source

In ocean biomes, your only food sources before the chest are:
- Raw cod/salmon dropped by fish mobs (requires punching them).
- Kelp (minimal nutrition when cooked).
- The chest itself — prioritize getting to it quickly.

Do not sprint excessively before reaching the chest if your hunger is already low — sprinting drains hunger faster.

---

## Building the Portal

Once you have an **iron bucket**, **lava**, and **flint and steel**, build your nether portal using one of these methods:

### Water + Lava Mold Method (Recommended)

This is the fastest portal construction method for most buried treasure runs:

1. Find a **lava pool** on the surface or just underground.
2. Construct a **2×3 frame mold** out of dirt or cobblestone:
   - Place dirt/cobble in the shape of a portal frame negative.
3. Pour **water** into the mold to convert surface lava into obsidian.
4. Break the mold blocks away, leaving the obsidian frame.
5. Light the interior with flint and steel.

This creates a **functional 2×3 nether portal** using only a water bucket and lava, with zero obsidian mining required.

### Manual Obsidian Mining

If a deep lava lake is your only option:

1. Pour water over the lava lake to create an obsidian platform.
2. Mine **10 obsidian** with your iron pickaxe (takes ~15 seconds per block without efficiency).
3. Construct the standard 4×5 portal frame (or compact 2×3 minimum).
4. Light with flint and steel.

> [!TIP]
> The mold method is **always preferred** over mining obsidian in a speedrun. Mining 10 obsidian takes over 2 minutes. The mold method takes under 30 seconds once you have materials.

### Flint and Steel vs. Fire Charge

- **Flint and Steel** — requires 1 iron ingot + 1 flint (obtained from gravel). Gravel is abundant on ocean floors.
- **Fire Charge** — found in some chest loot tables; use immediately if available.
- **Wood + lava trick** — place a wood log adjacent to lava to ignite a portal naturally. Use this only as an emergency if you have no other lighter.

---

## Inventory Checklist

Before entering the nether portal, verify you have all of the following:

### Essential Items

- [ ] **Iron Pickaxe** — for mining gold, nether quartz, and other nether materials
- [ ] **Iron Bucket** (empty or with water) — for emergency use in the nether
- [ ] **Flint and Steel** or **Fire Charge** — to relight the portal if broken by a ghast fireball
- [ ] **Food** — at least 6–8 pieces of any food (cooked fish preferred)
- [ ] **Sword** — stone or iron; needed for nether mob combat
- [ ] **Crafting Table** — in inventory for emergency nether crafting

### Recommended Items

- [ ] **Gold Ingots** (from chest or mined) — for piglin bartering at a bastion
- [ ] **Blocks for bridging** — cobblestone or dirt (16–32 blocks)
- [ ] **Torches** — for lighting your path and nether navigation
- [ ] **Spare Wood/Planks** — for emergency nether crafting
- [ ] **Shield** — if you had sufficient iron and wood

### Leave Behind

- ❌ Heart of the Sea — no use in speedrun
- ❌ Prismarine Crystals/Shards — no use
- ❌ Emeralds — no use without village trading
- ❌ Excess dirt (keep only 16 for bridging)
- ❌ Chainmail/Leather armor if full iron armor obtained

---

## Tips & Tricks

### General

- **Always open F3 at spawn.** On buried treasure seeds, coordinates are everything. Do not delay this — bind F3 to a convenient key and press it within the first 2 seconds.
- **Identify the biome before moving.** The F3 display shows your current biome in real time. If it reads "Ocean" or "Beach," you are almost certainly on a buried treasure seed.
- **Memorize the chunk-9,9 rule.** Buried treasure always spawns at chunk-relative coordinates (9, ~9, 9). Once you identify which chunk to target, finding the exact column to dig is instant.

### Underwater Technique

- **Dig a 2×2 hole if needed.** If you are slightly off on coordinates, a wider hole gives more margin to locate the chest visually.
- **Gravel and sand break equally fast by hand** — about 0.75 seconds each. There is no meaningful difference, so just dig whatever is in front of you.
- **Gamma settings matter.** Set your Minecraft gamma to 5.0 (or use the Sodium/Iris gamma slider) so the ocean floor is bright and you can spot the chest texture immediately.

### Loot Optimization

- **Only take what you need.** Inventory management in the early speedrun is critical. A cluttered inventory causes fumbles at the crafting table.
- **Eat immediately after surfacing.** Starting hunger regeneration early keeps you healthy for the sprint to find wood and lava.
- **If you get TNT, keep 1–2 pieces.** TNT can blast open underground lava lakes, saving significant digging time when searching for lava.

### Time Saves

- **Scan while swimming.** While swimming to the treasure location, look around for shipwrecks, tree-covered islands, ravines, and surface lava. Every observation now saves backtracking later.
- **Collect gravel on the way up.** As you ascend from the dig, break 2–3 gravel blocks to get flint. You need flint for flint and steel, and ocean floor gravel is free and abundant.
- **Pre-place your crafting table.** As soon as you get wood and exit the water, immediately craft and place the crafting table. Do not carry it in your inventory — leave it placed and come back if needed.

### Common Mistakes to Avoid

| Mistake                              | Consequence                                        | Fix                                                   |
|--------------------------------------|----------------------------------------------------|-------------------------------------------------------|
| Not opening F3 immediately           | Lost time orienting yourself                       | Bind F3 and press it within 2 seconds of spawning     |
| Drowning while digging               | Death, run reset, massive time loss                | Always resurface when 3–4 bubbles remain              |
| Taking Heart of the Sea              | Wasted inventory slot                              | Leave it — it has zero speedrun value                 |
| Forgetting to get wood first         | Stranded in ocean with no crafting table           | Scan for trees before diving; plan the path           |
| Digging in the wrong chunk spot      | Wasted dives, wasted breath, extended run time     | Double-check F3 chunk coordinates before diving       |
| Sprinting with low hunger            | Hunger damage mid-swim, possible death             | Do not sprint until you have eaten                    |
| Not crafting flint and steel         | Cannot light nether portal without improvising     | Always collect flint from gravel on the ocean floor   |
| Mining obsidian instead of mold build| 2+ minutes of wasted time                         | Always use the water+lava mold method when possible   |

---

## Summary

Buried treasure seeds are a powerful but demanding overworld type exclusive to high-Elo MCSR Ranked play. They reward players who are comfortable with:

- **F3 coordinate navigation** — no map, no visual structure, just numbers
- **Efficient underwater breath management** — every second underwater counts
- **Flexible post-loot routing** — finding wood, lava, and food in an ocean biome
- **Fast inventory management** — knowing exactly what to take and what to leave

Mastering buried treasure seeds is a strong signal of overworld competency. Once you can consistently execute a buried treasure start in under **4–5 minutes** before nether entry, you are well-positioned to compete and win at 1200+ Elo.

---

*Page maintained by the MCSR Ranked Wiki contributors. For corrections or additions, open an issue or pull request on the wiki repository.*
