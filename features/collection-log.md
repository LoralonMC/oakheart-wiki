# Collection Log

A per-player tracker for everything you've collected on Oakheart — blocks, items, mobs, biomes, structures, effects, and enchantments, plus every custom collectible (plushies, figures, cards, pets, tools, and more). Always running in the background; check in any time to see how much of the world you've experienced.

Long-term, no pressure, completionist-friendly.

{% hint style="info" %}
The Collection Log is **bragging rights**, not a reward path. Filling it out doesn't grant items or currency — it ranks you on the leaderboard and shows you the breadth of what's on the server.
{% endhint %}

---

## Opening the Log

`/log`

A multi-tab GUI opens. Each tab is a category — items you've collected show with a checkmark; missing ones are greyed out so you can see what's left to chase.

---

## Categories

| Category | What it tracks |
|----------|----------------|
| **Blocks** | Every placeable block. Wool colors count separately, etc. |
| **Items** | Everything that lives in inventory. Includes every custom item (plushies, figures, cards, vouchers, tools). |
| **Entities** | All living creatures — with **variants counted separately** (see below). |
| **Biomes** | Every biome you've stood in. Polled while you walk. |
| **Structures** | Every generated structure you've entered (villages, monuments, ancient cities, etc.). |
| **Effects** | Every status effect you've ever had applied. |
| **Enchantments** | Every enchantment you've owned (on tools or as books). |

---

## Variants Count Separately

This is the multiplier. Most servers count "sheep" as one entry. Oakheart enumerates the runtime registry and splits variants:

- **Sheep** — all 16 wool colors are separate entries
- **Cows** — temperate / cold / warm climate variants
- **Villagers** — type × profession (a desert farmer and a swamp farmer are different entries)
- **Horses** — color × style combinations
- **Tropical fish** — 22 named presets
- **Painting motifs** — every named painting variant
- **Wolves, frogs, axolotls, cats, llamas, parrots, pandas, foxes, rabbits, mooshrooms** — color/type variants
- **Chickens, pigs** — climate variants

You may think you've collected sheep. There are 15 more to chase.

---

## Sets

Sets are themed groupings that cut across categories — collection challenges with their own completion meters.

**Nog's Menagerie pools:**
- Plushies, Figures, Adorables, Trading Cards, Card Boosters

**Trading card decks:**
- Haunted Hellscape, Mortal Monsters, Nascent Nature, The Menagerie, Wonderful World, Starter Pack

**Furniture sets:**
- Chess Set, Halloween Decor, Christmas Decor, Graveyard Decor, Lunar New Year

**Vanilla classics:**
- Music Discs, Armor Trims, Wool Colors, Concrete Colors, Glazed Terracotta, Stained Glass, Beds, Banners, Carpets, Candles, Saplings, Mob Heads, Flowers

**Plugin-specific:**
- Crate Keys, Oak Tools, Pet Vouchers, Chat Tags

Each set has its own browser tab so you can see what's near completion vs. what's barely started.

---

## Toasts

When you collect something new, the log can pop a Minecraft advancement toast in the top-right corner. Three modes:

| Mode | When you see toasts |
|------|---------------------|
| **On** | Every new entry (default) |
| **Milestones** | Every 25 entries + category completions + full-log completion |
| **Off** | Never |

Switch via:

`/log toast on`
`/log toast milestones`
`/log toast off`

If per-entry feels noisy, drop to `milestones` for fewer notifications without losing the major completion popups.

---

## Leaderboard

A global leaderboard shows the top collectors server-wide, with rankings per category too. Your own rank is always pinned at the bottom of the view so you know exactly where you stand.

The board updates every 60 seconds.

---

## Search & Recent Activity

- **Search** — Hit the search button in the GUI, type a query in chat, and the log shows matching entries across all categories.
- **Recent Activity** — A tab showing your most recent collections, sorted by timestamp. Handy when a toast pops and you want to know what just got added.

---

## Viewing Other Players' Logs

```
/log <player>
```

Read-only view of someone else's collection log. Useful for comparing progress with friends, or for seeing what completionists are chasing next.

---

## Commands Quick Reference

| Command | Description |
|---------|-------------|
| `/log` | Open your collection log |
| `/log <player>` | View another player's log (read-only) |
| `/log toast <on\|off\|milestones>` | Toggle toast preference |

---

## Related Pages

- [Pets](pets.md) — Pet vouchers count toward your log
- [Cosmetics](cosmetics.md) — Most cosmetic items have log entries
- [Toy Store](../traders/toy-store.md) — Where to buy plushies, figures, adorables, and cards
- [Crates Overview](../crates/overview.md) — Crate items count toward your log
