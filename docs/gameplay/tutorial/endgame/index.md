# Endgame

The Endgame is the final phase of an MCSR Ranked run. It begins when you craft your **Eyes of Ender** and ends the moment the Ender Dragon dies and the credits roll. Despite being the last phase, it is the one that most often determines the winner of a close match — a player with a one-minute Nether advantage can easily throw the race with poor stronghold navigation or a messy dragon fight.

This page covers what you need entering the Endgame, the three steps to complete it, and the tools that make it consistent.

---

## Prerequisites: What You Need Before Endgame

Before leaving the Nether, you should have accumulated the following:

| Resource | Minimum | Recommended | Notes |
|---|---|---|---|
| **Blaze Rods** | 4 | 7 | Each rod crafts 2 Blaze Powder; you need 7–12 powder total (crafting + fuel) |
| **Ender Pearls** | 7 | 10–12 | One Eye of Ender is consumed per throw and some break; need minimum 7 to enter portal |
| **Eyes of Ender** | 7 (crafted) | 10–12 | Minimum 12 for the portal frame, but pre-filled slots reduce this |
| **End Portal Frames (pre-filled)** | variable | — | Strongholds always spawn with 0–3 Eyes pre-inserted randomly |

### Crafting Breakdown
- **1 Blaze Rod → 2 Blaze Powder**
- **1 Blaze Powder + 1 Ender Pearl → 1 Eye of Ender**
- You need **12 Eyes of Ender** to fill the End Portal frame (but frames often have 1–3 pre-filled)
- You need **extra Eyes** for throws during blind travel (they break ~80% of the time)

> **Minimum viable:** 4 Blaze Rods + 10 Ender Pearls = 8 Eyes for throwing + 8 for the frame. Aim for this as your floor, not your ceiling.

---

## The Three Steps of Endgame

### Step 1: Locate the Stronghold (Blind Travel)

Strongholds are hidden underground structures that contain the **End Portal**. There is no map marker — you must find one using Eyes of Ender.

**How it works:**
1. Craft your Eyes of Ender.
2. Throw one into the air. It floats in the direction of the nearest Stronghold, then either drops (retrievable) or breaks.
3. Note the direction and your coordinates from **F3**.
4. Move in that direction, then throw again from a new position.
5. **Triangulate** using two or more throws to pinpoint the Stronghold's X/Z coordinates.
6. Dig down at the estimated location.

This process is called **"blind travel"** and is the single highest-skill step in a speedrun. Precise triangulation saves 30–90 seconds over rough estimation.

#### Ninjabrain Bot
**Ninjabrain Bot** is the essential tool for this step. It is a desktop overlay that reads your F3 position and angle data and calculates the exact stronghold coordinates after each throw. It tells you:
- The estimated X/Z position of the Stronghold center
- The certainty percentage of that estimate
- The direction and distance to travel

Download: [github.com/Ninjabrain1/Ninjabrain-Bot](https://github.com/Ninjabrain1/Ninjabrain-Bot)

See the full guide: [Blind Travel & Eye Throws →](./endgame/blind_travel.md)

---

### Step 2: Navigate the Stronghold

Once you dig into the Stronghold, you need to find the **End Portal Room** as quickly as possible. Strongholds are large, procedurally generated structures with many dead ends, stairways, libraries, and corridors. Navigating them efficiently is a learnable skill.

Key tips for beginners:
- **Follow the stairs downward** — the portal room is always below the surface level of the Stronghold.
- **Break through walls** if a hallway is blocked; the fastest path is often not the intended one.
- **Listen for Silverfish** — they spawn near the End Portal room in large numbers and can indicate you are close.
- **Light your way** — carry torches or use a fire aspect sword. A dark Stronghold causes many avoidable deaths.
- The **End Portal Room** is recognizable by its lava pool, iron bars, and the portal frame in the center.

Common Stronghold navigation patterns are documented in: [Stronghold Navigation →](./endgame/stronghold.md)

---

### Step 3: Kill the Ender Dragon

After placing your final Eyes of Ender into the portal frame and leaping through, you arrive in **The End** — a dark void island with the Ender Dragon circling above.

The fight has a fixed structure:
1. **Destroy the End Crystals** on top of the obsidian pillars — they heal the dragon. Shoot them with a bow or knock them off with a block/sword.
2. **Wait for the Dragon to perch** on the central fountain. It will lower its head and become vulnerable.
3. **Hit the Dragon's head** (the only damageable hitbox while perched). A bed explosion is the fastest method — place a bed next to the fountain, stand behind cover, and right-click it to trigger the explosion.
4. Repeat until the Dragon dies and the credits roll.

> **Beginner Note:** Bed explosions deal massive damage but can kill you if misused. Practice the timing carefully. A sword + bow approach is slower but safer while learning.

Full dragon fight mechanics and bed pop strategy: [Dragon Fight →](./endgame/dragon_fight.md)

---

## Key Tool: Ninjabrain Bot

Ninjabrain Bot deserves emphasis beyond just the blind travel step. It is one of the few external tools that is **allowed and encouraged** in MCSR Ranked competition. Setting it up correctly before your first ranked session is strongly recommended.

**Setup checklist:**
- [ ] Download and install Ninjabrain Bot
- [ ] Enable F3 reading in its settings (it must detect your game window)
- [ ] Set your FOV in the bot to match your in-game FOV
- [ ] Practice throwing Eyes of Ender on a test world and confirm the bot is reading your position
- [ ] Configure the overlay position so it does not block your game HUD

Refer to: [Blind Travel & Eye Throws →](./endgame/blind_travel.md) for a full setup walkthrough.

---

## Endgame Subpages

- [Blind Travel & Eye Throws →](./endgame/blind_travel.md) — Triangulation technique, Ninjabrain Bot setup, throw optimization
- [Stronghold Navigation →](./endgame/stronghold.md) — Layout patterns, routing through rooms, portal room recognition
- [Dragon Fight →](./endgame/dragon_fight.md) — Crystal destruction, perch timing, bed pop strategy, one-cycle and two-cycle

---

*Previous phase: [Nether Index →](./nether_index.md)*  
*Back to: [Tutorial Index →](./tutorial_index.md)*
