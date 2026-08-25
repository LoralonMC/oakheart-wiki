# Server Limits

Oakheart runs close to vanilla. This page lists exactly what's limited, so you never have to guess whether a farm stopped working because of us or because of Minecraft.

{% hint style="info" %}
**The short answer:** There is no plugin culling your mobs, and no limit on how many animals you can keep. Every limit below exists to stop lag machines, not to restrict normal building.
{% endhint %}

---

## Block Limits

These apply **per chunk** (a 16x16 column). A normal item sorter, farm, or storage room is nowhere near any of them.

| Block | Limit per chunk |
|-------|-----------------|
| **Hoppers** | 128 |
| **Beds** | 64 |
| **All other block entities** | 256 |

"Block entities" means blocks the server has to tick or store data for: chests, barrels, furnaces, droppers, dispensers, signs, banners, and similar. Ordinary building blocks like stone, wood, and glass are **not** limited in any way.

If you try to place a block past the limit, the server tells you and stops the placement. Nothing is deleted.

---

## Mob Spawning

| Category | Cap |
|----------|-----|
| **Hostile mobs** | 40 |
| **Animals** | Vanilla |
| **Axolotls** | Vanilla |
| **Fish and water mobs** | Slightly reduced |
| **Bats** | Off |

The hostile cap is 40 instead of Minecraft's 70. In exchange, the cap is **per player**, so nobody else's farm competes with yours. On a busy server this usually means *more* mobs for you, not fewer.

Two other things affect farm rates:

- **Hostile mobs despawn at 80 blocks** instead of 128.
- **Simulation distance is 6 chunks.** Anything further than that from a player is frozen, so a farm only runs while someone is near it.

---

## Entities That Behave Differently

A few things are deliberately changed. These surprise people, so they're worth knowing:

- **Armor stands don't move.** No gravity, no physics, no falling. They stay exactly where you put them. Armor stand physics is one of the worst lag sources in Minecraft, so it's off.
- **Loose projectiles are capped per chunk when that chunk unloads.** Arrows, ender pearls, snowballs, and fireballs cap at **20 per chunk**, and experience orbs at **50**. Anything beyond that is gone when the area reloads. This matters for arrow farms and pearl stasis chambers, so keep them tidy.
- **Dropped items despawn after 5 minutes**, same as vanilla.
- **Players don't take entity cramming damage.** Mobs still do.

---

## Redstone

There is **no limit on how much redstone you can place**. Build whatever you like.

There is a throttle for genuinely extreme cases: if a single chunk produces somewhere around 3,200 redstone updates per second, the server starts ignoring the excess until it calms down. It recovers on its own.

{% hint style="warning" %}
**You will not hit this by accident.** A clock, a flying machine, a big door, or a full sorting system are all far below it. If a contraption of yours suddenly stops responding, tell staff rather than tearing it down. We can check whether this is what happened.
{% endhint %}

---

## What This Means For Farms

Farms are welcome. Build them. To keep things smooth for everyone:

- **Turn farms off when you're not using them.** A lever on the input is enough.
- **Don't leave thousands of mobs alive in a holding cell.** Kill chambers should actually kill.
- **Sweep up loose arrows and items** around your builds.
- **Ask before building something enormous.** Staff would much rather help you design it than remove it later.

See [Server Rules](../rules.md) for the full policy on performance and lag machines.

---

{% hint style="success" %}
**Still not sure?** Ask in Discord. If a limit is affecting you, staff can check the exact numbers for your area and tell you what's going on.
{% endhint %}
