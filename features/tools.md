# Building Tools

Oakheart has three custom building tools designed for survival mode: the {{item:file}}, the {{item:trowel}}, and the {{item:wand}}. All are craftable and work with your claims.

{% hint style="info" %}
**Don't want to craft?** These tools are also available from the [Token Trader](../traders/token-trader.md) ({{item:vote_token:60-70}}) and as drops from Paid Crates (Daisy, Rose, and Lily tiers).
{% endhint %}

---

## File

A precision tool for editing block states without breaking and replacing blocks.

### What It Does

Right-click supported blocks to modify their appearance:

| Block Type | What You Can Change |
|------------|---------------------|
| Fences, Glass Panes, Iron Bars | Toggle individual connections |
| Walls | Adjust heights and connections |
| Stairs | Change shape (Shift + right-click for top/bottom) |
| Logs & Pillars | Cycle X/Y/Z axis orientations |
| Slabs | Toggle top/bottom placement |
| Directional Blocks | Change facing (observers, pistons, dispensers, droppers) |

### How to Craft

```crafting
_,_,iron_ingot
_,iron_ingot,_
stick,_,_
=> file
```

### Tips

- Uses durability per edit
- Supports Mending and Unbreaking enchantments
- Repair with {{item:iron_ingot}} in an anvil
- Works with your claimed land

---

## Trowel

A smart building tool that randomly places blocks from your inventory — perfect for natural-looking paths, walls, and floors.

### What It Does

1. Fill an inventory row with different block types (e.g., stone, cobblestone, andesite)
2. **Shift + right-click** to select which row to pull from (Hotbar, Row 1, 2, or 3)
3. **Right-click** to place a random block from that row

Each placement consumes one block from your inventory.

### How to Craft

```crafting
_,_,iron_ingot
_,iron_ingot,iron_ingot
stick,_,_
=> trowel
```

### Tips

- Great for paths, floors, and natural-looking builds
- Automatically skips incompatible items (doors, beds, signs)
- Uses durability per placement
- Supports Mending and Unbreaking enchantments
- Repair with {{item:iron_ingot}} in an anvil

---

## Builder's Wand

A smart building tool that extends surfaces by placing blocks along the face you're looking at — perfect for quickly building walls, floors, and ceilings.

### What It Does

1. **Right-click** a block face to extend it by placing matching blocks from your inventory
2. **Shift + right-click** to cycle between placement modes:
   - **Face** — fills a flat area on the clicked face
   - **Line** — extends a single row along one axis

Each placement consumes blocks from your inventory and supports up to 64 blocks per use.

### How to Craft

```crafting
_,iron_ingot,iron_ingot
_,stick,iron_ingot
stick,_,_
=> wand
```

### Tips

- Preview shows a glow outline before placing
- Supports undo (up to 5 recent placements, expires after 5 minutes)
- Uses durability per placement
- Supports Mending and Unbreaking enchantments
- Repair with {{item:iron_ingot}} in an anvil

---

## Repair

All tools can be repaired:

- **Anvil + {{item:iron_ingot}}** — Standard repair
- **Combine two tools** — Merges durability with a 5% bonus
- **Enchanted books** — Add Mending or Unbreaking

---

## Related Pages

- [Homes](homes.md)
- [Player Warps](player-warps.md)
