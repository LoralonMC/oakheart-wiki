# Tools

Oakheart has custom tools split into two categories: **building tools** for creative construction, and **harvesting tools** for efficient resource gathering.

{% quicknav %}
Building Tools: file, trowel, wand#builders-wand
Sickle: iron_sickle#sickle
Harvesting Tools: excavator#excavation-shovel, vein-miner#vein-miner-pickaxe, lumberjack#lumberjacks-axe
{% endquicknav %}
 
---

## Building Tools

Three craftable tools designed for survival building. All use iron durability, support Mending and Unbreaking enchantments, and can be repaired with {{item:iron_ingot}} in an anvil.

{% hint style="info" %}
**Don't want to craft?** Building tools are also available from the [Token Trader](../traders/token-trader.md) for {{item:vote_token:60-70}}.
{% endhint %}

### File

A precision tool for editing block states without breaking and replacing blocks.

Right-click supported blocks to modify their appearance:

| Block Type                     | What You Can Change                                      |
| ------------------------------ | -------------------------------------------------------- |
| Fences, Glass Panes, Iron Bars | Toggle individual connections                            |
| Walls                          | Adjust heights and connections                           |
| Stairs                         | Change shape (Shift + right-click for top/bottom)        |
| Logs & Pillars                 | Cycle X/Y/Z axis orientations                            |
| Slabs                          | Toggle top/bottom placement                              |
| Directional Blocks             | Change facing (observers, pistons, dispensers, droppers) |

```crafting
_,_,iron_ingot
_,iron_ingot,_
stick,_,_
=> file
```

### Trowel

A smart building tool that randomly places blocks from your inventory — perfect for natural-looking paths, walls, and floors.

1. Fill an inventory row with different block types (e.g., stone, cobblestone, andesite)
2. **Shift + right-click** to select which row to pull from (Hotbar, Row 1, 2, or 3)
3. **Right-click** to place a random block from that row

Each placement consumes one block from your inventory.

```crafting
_,_,iron_ingot
_,iron_ingot,iron_ingot
stick,_,_
=> trowel
```

### Builder's Wand

A smart building tool that extends surfaces by placing blocks along the face you're looking at — perfect for quickly building walls, floors, and ceilings.

1. **Right-click** a block face to extend it by placing matching blocks from your inventory
2. **Shift + right-click** to cycle between placement modes:
   - **Face** — fills a flat area on the clicked face
   - **Line** — extends a single row along one axis

Each placement consumes blocks from your inventory and supports up to 64 blocks per use.

```crafting
_,iron_ingot,iron_ingot
_,stick,iron_ingot
stick,_,_
=> wand
```

**Tips:**

- Preview shows a glow outline before placing
- Supports undo (up to 5 recent placements, expires after 5 minutes)

---

## Sickle

A vanilla-style tiered tool that harvests mature crops in an area and automatically replants them. Higher tiers harvest a larger radius.

| Tier      | Radius       | Recipe Material           |
| --------- | ------------ | ------------------------- |
| Wooden    | Single block | Planks                    |
| Stone     | 3×3         | Cobblestone               |
| Iron      | 5×5         | Iron Ingots               |
| Gold      | 3×3         | Gold Ingots               |
| Diamond   | 7×7         | Diamonds                  |
| Netherite | 9×9         | Upgrade at smithing table |

```crafting
_,iron_ingot,iron_ingot
_,_,iron_ingot
_,stick,_
=> iron_sickle
```

**Tips:**

- Uses vanilla durability, enchanting, and repair — works just like a regular tool
- Supports Fortune (more crop drops) and Unbreaking
- Only harvests mature crops — leaves growing crops alone

---

## Harvesting Tools

Premium tools obtained from [Paid Crates](../crates/paid-crates.md) or the [Token Trader](../traders/token-trader.md). These are **consumable** — they have limited durability, cannot be enchanted, and cannot be repaired.

{% hint style="warning" %}
Harvesting tools are consumable. Once the durability runs out, the tool breaks permanently. Plan your uses wisely!
{% endhint %}

**Hold sneak** while breaking to mine a single block without activating the tool's ability. All drops go directly to your inventory.

| Tool               | Effect                          | Durability | Source                               |
| ------------------ | ------------------------------- | ---------- | ------------------------------------ |
| {{item:excavator}}  | 3×3 area dig                   | 500        | {{item:vote_token:60}} / Daisy Crate |
| {{item:vein-miner}} | Mine entire connected ore vein  | 750        | {{item:vote_token:70}} / Rose Crate  |
| {{item:lumberjack}}   | Fell an entire tree in one chop | 1000       | {{item:vote_token:70}} / Lily Crate  |

### Excavation Shovel

Breaks a 3×3 area of blocks when you mine a single block. Durability is consumed per block broken (9 per activation). Works on any shovel-mineable block.

### Vein Miner Pickaxe

Mines all connected ore blocks of the same type at once (up to 32 blocks). Deepslate and regular ore variants count as the same vein. Durability is consumed per ore block mined.

### Lumberjack's Axe

Fells an entire tree in one chop (up to 64 blocks). Only works on naturally generated trees — it checks for nearby leaves to prevent accidental use on builds. Durability is consumed per log broken.

---

## Related Pages

- [Token Trader](../traders/token-trader.md)
- [Paid Crates](../crates/paid-crates.md)
- [Homes](homes.md)
- [Player Warps](player-warps.md)