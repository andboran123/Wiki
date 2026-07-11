# Oneshot — Ender Dragon Kill Strategy

> [!NOTE]
> The Oneshot is an **extremely rare and situational** technique in MCSR Ranked (RSG). It is not a strategy you should plan around in ranked play. This page exists for educational purposes and to explain what you may occasionally see in impressive runs. Your primary focus should be [One Cycle](end_one_cycle.md) or [Zero Cycle](end_zero_cycle.md).

---

## Table of Contents

1. [What Is the Oneshot?](#what-is-the-oneshot)
2. [The Physics — How It Works](#the-physics--how-it-works)
3. [Rarity and Use Case](#rarity-and-use-case)
4. [The Setup](#the-setup)
5. [When It Can Happen Naturally](#when-it-can-happen-naturally)
6. [How to Attempt It](#how-to-attempt-it)
7. [Practical Advice for MCSR Ranked](#practical-advice-for-mcsr-ranked)
8. [Notable Runs](#notable-runs)
9. [Tips](#tips)

---

## What Is the Oneshot?

The **Oneshot** (also called the **arrow oneshot** or **tail oneshot**) is a technique where a single arrow kills the Ender Dragon instantly — all **200 HP** in one hit.

This is possible because Minecraft's damage formula for projectiles takes into account **projectile velocity**. Normally, an arrow deals a fixed damage range based on bow charge level. However, if an arrow's velocity is **dramatically amplified** by an external force — specifically the Ender Dragon's own tail sweep knockback — the resulting arrow can reach a speed at which the damage formula outputs a value large enough to kill the dragon outright.

In other words: the dragon's own attack becomes the weapon that kills it.

---

## The Physics — How It Works

To understand the oneshot, you need to understand two Minecraft mechanics: **projectile damage scaling** and **the dragon's tail knockback**.

### Projectile Damage Scaling

In Minecraft, the damage dealt by an arrow is not simply a fixed number. It is calculated as:

```
Damage = (velocity * 2 + 1) rounded to nearest integer
```

A normally shot arrow from a fully charged bow travels at approximately **3 blocks/tick**, dealing roughly **6–9 damage**. But this formula has no hard cap — if the velocity is artificially multiplied by a large factor, the damage output scales proportionally.

### The Dragon's Tail Sweep

The Ender Dragon has a **tail sweep attack** that applies a knockback effect to players and entities in a wide radius around its tail position. This knockback is applied as a velocity vector.

When an arrow (which is itself a physics entity) is in the path of the tail sweep at the exact moment the sweep executes, the game applies the knockback velocity to the **arrow entity**. Since the arrow is already traveling, this additional velocity is added — **multiplying the arrow's total velocity** by a large factor.

### The Result

An arrow with velocity boosted by the tail knockback can reach speeds of **hundreds of blocks per tick** — far beyond any normal arrow. When this hyper-velocity arrow then strikes the dragon (specifically the head hitbox), the damage formula produces a value far exceeding 200 HP, instantly killing it.

> [!NOTE]
> This is not a glitch in the sense of an exploit or dupe — it is the game's physics simulation working as coded. The damage formula legitimately produces massive numbers from high-velocity projectiles. It is legal in all MCSR Ranked categories.

### The Timing Constraint

For the tail knockback to apply to the arrow:
- The arrow must be in flight (already shot).
- The tail sweep must execute at the precise moment (within approximately **1 game tick = 1/20th of a second**) of the arrow passing through the tail sweep radius.
- This is an extraordinarily tight timing window, making unintentional oneshots extremely rare and intentional ones nearly impossible without frame-perfect setup.

---

## Rarity and Use Case

### In MCSR Ranked (RSG — Random Seed Glitchless)

In Random Seed runs — the format used in MCSR Ranked — the oneshot is:

- **Not a planned strategy.** The variables required (bow, arrows, dragon position, tail timing) are too RNG-dependent.
- **A lucky occurrence.** If it happens, it is typically during normal combat when a runner is using their bow to shoot crystals or deal supplemental damage.
- **A bonus, not a plan.** Runners who achieve an unintentional oneshot in a ranked run are usually as surprised as their viewers.

### In SSG (Set Seed Glitchless)

In Set Seed runs, the oneshot is:

- **A viable planned technique.** Since everything about the run is known in advance, runners can:
  - Know whether the seed provides a bow and arrows.
  - Know the dragon's tail sweep timing (same every seed).
  - Practice the exact arrow fire timing to coincide with the sweep.
- **Used in competitive world record runs.** Some top SSG times incorporate intentional oneshot attempts.
- **Still not guaranteed.** Even with practice, the 1-tick window means it's roughly a 40–60% success rate even for practiced runners.

> [!WARNING]
> Do **not** attempt to incorporate oneshot into your MCSR Ranked strategy unless you are already sub-9 minutes and looking for marginal gains from situational opportunism. The opportunity cost of setting up a oneshot attempt and failing is too high.

---

## The Setup

For those who wish to understand or attempt the oneshot:

### Required Items

| Item | Notes |
|---|---|
| Bow | Must be at least partially charged. Full charge provides most velocity. |
| Arrows | At least 1 arrow. |
| No End Crystals required | The oneshot can be attempted while crystals are still active, though the dragon heals fast. |

### Position Requirements

- You must be positioned **near the dragon's tail** during its flight phase (not the perch).
- The tail is at the **rear of the dragon**, extending behind its body as it flies.
- You need to be within the range of the tail's sweep hitbox — roughly **5–10 blocks from the tail tip**.

### The Setup Risk

Getting near the dragon's tail during flight is inherently dangerous:
- The tail sweep itself deals **knockback and damage** to the player.
- You can be knocked into the void.
- Endermen in the area add additional hazard.

This is another reason oneshot is not pursued deliberately in ranked RSG — the setup position is genuinely dangerous.

---

## When It Can Happen Naturally

The most common way a oneshot occurs in ranked play is **entirely unplanned**:

### Scenario: Crystal Shooting

A runner is shooting arrows at caged crystals near a tall pillar. The dragon happens to fly its tail through the arrow's path at the exact moment of the tail sweep. The arrow velocity is boosted and hits the head — oneshot.

### Scenario: Combat Defense

A runner is using their bow to deal supplemental damage during the perch or a flyby. An arrow they fire into the dragon's body area happens to intersect the tail sweep timing. Oneshot.

### Scenario: Node Arrow Volley

During a zero cycle or ground zero attempt, a runner also fires arrows at the dragon's approaching head. One of the arrows passes through the tail sweep zone during the sweep. Oneshot.

> [!NOTE]
> In all these scenarios, the runner typically did not intend the oneshot. It is a consequence of the game's physics interacting in a specific way. The "unintentional oneshot" is one of the most celebrated moments in MCSR Ranked streaming.

---

## How to Attempt It

For runners curious about attempting the oneshot deliberately:

### Step 1: Acquire a Bow and Arrows

- In RSG, you need a bow from a chest (bastion remnant, village fletcher, shipwreck, etc.) or crafted if you find bones and feathers.
- Arrows from skeletons, chests, or crafting.
- Even **1 arrow** is enough for a single attempt.

### Step 2: Enter the End

- Proceed with normal End entry.
- Keep the bow in your hotbar with arrows.

### Step 3: Wait for the Dragon's Tail to be Near You

- Watch the dragon's flight pattern.
- The tail extends backward from the body — identify when the dragon is flying such that its tail sweeps through your area.

### Step 4: Fire Just Before the Sweep

- Pull back the bow to full charge.
- Release the arrow **just before** the tail sweep executes — the arrow needs to be in flight during the sweep, not fired afterward.
- The timing is approximately **1–3 ticks** (0.05–0.15 seconds) before the visible sweep animation.

### Step 5: The Outcome

Genuinely — the timing is tight enough that intentional setup has roughly a:
- ~15–25% success rate for players who have never practiced it.
- ~40–60% success rate for players who have extensively practiced in SSG contexts.

If the oneshot connects, the dragon death animation begins immediately with no additional steps required. One arrow, one hit, run over.

> [!TIP]
> If you have a bow in a ranked run and the dragon's tail happens to be near you during your crystal clearing route — **take the shot.** It costs you one arrow and less than a second. If it works, you have one of the most exciting clips in your ranked history.

---

## Practical Advice for MCSR Ranked

Here is the realistic guidance for how to incorporate oneshot knowledge into your ranked play:

### Don't Build Your Strategy Around It

The oneshot is not reliable enough to plan around in RSG. Your End strategy should be:
1. **One Cycle** (primary, always have this ready)
2. **Zero Cycle** (if you've practiced it)
3. **Oneshot** (opportunistic only — if the arrow setup presents itself naturally)

### Do Take Shots of Opportunity

If you have a bow and arrows, and the dragon's tail is near you during normal combat or crystal clearing — fire the arrow. There is no meaningful downside. It costs one arrow and one second. The upside is a free run-ending oneshot.

### Do Bring a Bow

Even if you never attempt the oneshot, a bow is useful in The End for:
- Shooting caged crystals from a distance.
- Dealing supplemental damage to the dragon during the perch.

A bow is a **net positive** item to bring into the End regardless of oneshot potential.

### Know It Exists

Understanding the oneshot helps you:
- Recognize what happened if it occurs in your own run.
- Appreciate it in other runners' runs.
- Understand SSG category strategies if you ever explore that format.

---

## Notable Runs

> [!NOTE]
> This section intentionally does not name specific world record times, as these change frequently. Refer to [speedrun.com/mc](https://www.speedrun.com/mc) and the MCSR Ranked leaderboard for current records.

### SSG World Record Runs

Many competitive SSG (Set Seed Glitchless) world record runs for the Any% category incorporate planned oneshot attempts. Since the seed is known:
- The bow location is known in advance.
- The dragon's tail timing is rehearsed extensively.
- The oneshot success rate for top SSG runners on practiced seeds can reach 60%+.

These runs often end dramatically — a single arrow followed immediately by the dragon death animation and credits — which is part of why oneshot runs generate significant viewership.

### RSG Ranked Highlights

Unintentional oneshots in MCSR Ranked runs are periodic highlights on the MCSR Ranked clip channels and Discord. The combination of:
- Having a bow (already moderately rare in an optimized RSG run),
- Being in the right position at the right time,
- The 1-tick timing aligning randomly,

...makes each occurrence a genuinely memorable and clip-worthy event. If you are fortunate enough to achieve one, it tends to be one of the most-clipped moments in your ranked history.

---

## Tips

> [!TIP]
> **Always carry a bow in The End.** Even a weak bow with 1–3 arrows has value — caged crystals, supplemental damage, and oneshot opportunity. The weight cost is zero in The End context.

> [!TIP]
> **Watch SSG runs to understand intentional oneshots.** Seeing a runner deliberately set up the position, fire, and land the hit gives you the clearest visual understanding of what the technique looks like when it works.

> [!TIP]
> **Don't use your arrow stockpile chasing the oneshot.** If you fire 2–3 arrows and don't hit it, the opportunity has passed. Move on to your primary kill strategy. You don't have arrows to waste.

> [!TIP]
> **Know the sound.** A successful tail-boosted arrow makes a distinctly more impactful sound than a regular arrow hit. Experienced players can sometimes identify a "boosted" arrow hit audibly before the damage number confirms it.

> [!TIP]
> **Learn your primary strategies first.** One Cycle → Zero Cycle → Ground Zero → Oneshot awareness is the correct learning progression. Skipping to "oneshot practice" before having a reliable kill strategy is a common beginner trap.

> [!TIP]
> **If you're going for it, go full charge.** A fully charged bow arrow has more base velocity. More base velocity means the tail boost multiplies to a higher final speed, improving your chances of crossing the kill threshold.

---

## Comparison: Oneshot vs. Other Strategies

| Factor | Oneshot | Zero Cycle | One Cycle |
|---|---|---|---|
| Time to kill (if successful) | ~5–10 seconds | ~30–60 seconds | ~60–90 seconds |
| Reliability in RSG | <5% | ~50–70% (practiced) | ~85–95% (practiced) |
| Required items | Bow + arrows | Beds + obsidian | Beds + obsidian |
| Recommended for ranked | Situational/bonus | Intermediate+ | All levels |
| Learning priority | Last | Third | First |

---

*Last updated: July 2026 | Part of the MCSR Ranked Wiki — End Dimension Section*
*← [Ground Zero](end_ground_zero.md) | [Back to End Overview](end_index.md)*
