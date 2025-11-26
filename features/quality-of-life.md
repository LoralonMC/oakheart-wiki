# Quality of Life Features

Oakheart includes several quality-of-life features to make your gameplay smoother and more enjoyable.

---

## Phantom Toggle

Tired of Phantoms attacking you at night? Toggle them off!

### Command

```
/settings
```

Toggles whether Phantoms will target you. Your sleep deprivation still builds up, but Phantoms simply won't spawn for you.

{% hint style="info" %}
**Note:** This only affects Phantoms targeting *you*. You can still encounter Phantoms that were spawned by other players.
{% endhint %}

---

## Invisible Item Frames

Create cleaner displays by making item frames invisible while keeping the item visible.

### How to Craft

Surround a **Phantom Membrane** with item frames in a crafting table:

**Normal Invisible Frame:**
```
[Frame] [Frame] [Frame]
[Frame] [Membrane] [Frame]
[Frame] [Frame] [Frame]
```

**Glow Invisible Frame:**
```
[Glow Frame] [Glow Frame] [Glow Frame]
[Glow Frame] [Membrane] [Glow Frame]
[Glow Frame] [Glow Frame] [Glow Frame]
```

### Use Cases

- **Map walls** — Seamless map displays
- **Decorations** — Floating items as decoration
- **Shops** — Clean item displays for player shops
- **Museums** — Display items without visible frames

---

## Overflow Inventory

When you receive items but your inventory is full, they go to your overflow instead of being lost.

### Commands

| Command | Description |
|---------|-------------|
| `/overflow` | Open your overflow inventory |
| `/of` | Shortcut for `/overflow` |

### When Overflow Activates

- Crate rewards when inventory is full
- Rank-up rewards when inventory is full
- Any server-given items

{% hint style="warning" %}
**Check regularly!** Items in overflow don't despawn, but it's easy to forget they're there.
{% endhint %}

---

## Animal Traps

Capture animals in portable containers for easy transportation.

### How to Use

1. Place an Animal Trap on the ground
2. Lead or push an animal onto the trap
3. The animal is captured and stored in the trap item
4. Pick up the trap and place it elsewhere to release

### Supported Animals

Animal Traps work on passive animals including:
- Farm animals (cows, pigs, sheep, chickens)
- Horses, donkeys, and mules
- Wolves and cats
- Other passive mobs

{% hint style="info" %}
**Villagers and hostile mobs** cannot be captured with Animal Traps.
{% endhint %}

### Use Cases

- Moving animals to your farm
- Transporting horses across long distances
- Relocating pets safely
- Trading rare animal variants with other players

---

## Sitting, Laying & Crawling

Express yourself and relax with various positions.

### Sitting

| Command | Description | Rank Required |
|---------|-------------|---------------|
| `/sit` | Sit on the ground | Rank 5 |

You can also right-click on **stairs and slabs** to sit on them automatically.

### Laying

| Command | Description | Rank Required |
|---------|-------------|---------------|
| `/lay` | Lay down on the ground | Rank 4 |

### Crawling

| Command | Description | Rank Required |
|---------|-------------|---------------|
| `/crawl` | Enter crawling position | Rank 15 |

### Other Positions

| Command | Description | Rank Required |
|---------|-------------|---------------|
| `/bellyflop` | Bellyflop onto the ground | Rank 11 |

---

## Jump

Quickly teleport in the direction you're looking.

### Command

```
/jump
```

**Rank Required:** Rank 13 (Thicket)

Teleports you approximately 30 blocks in the direction you're looking. Useful for quickly crossing gaps or reaching distant ledges.

{% hint style="warning" %}
**Be careful!** Make sure there's solid ground where you're aiming, or you might fall.
{% endhint %}

---

## Portable Workstations

Access crafting interfaces anywhere without placing blocks.

| Command | Description | Rank Required |
|---------|-------------|---------------|
| `/craft` | Open crafting table | Rank 8 |
| `/loom` | Open loom | Rank 7 |
| `/stonecutter` | Open stonecutter | Rank 12 |
| `/grindstone` | Open grindstone | Rank 14 |
| `/anvil` | Open anvil | Rank 16 |
| `/smithingtable` | Open smithing table | Rank 18 |
| `/cartographytable` | Open cartography table | Mythic+ Store Rank |

---

## Personal Time

Control your personal day/night cycle without affecting other players.

### Command

```
/ptime <time>
```

**Rank Required:** Rank 17 (Oak)

### Options

| Value | Effect |
|-------|--------|
| `day` | Always daytime for you |
| `night` | Always nighttime for you |
| `reset` | Return to server time |
| `<number>` | Specific time (0-24000) |

{% hint style="info" %}
This only changes what *you* see. Other players and mob spawning follow server time.
{% endhint %}

---

## Remote Ender Chest

Access your ender chest from anywhere.

### Command

```
/enderchest
```

**Rank Required:** Rank 19 (Heartwood)

Aliases: `/ec`

---

## Item Condensing

Quickly convert items into their block form.

### Command

```
/condense
```

**Rank Required:** Rank 3 (Seedling)

### What It Does

Converts items in your inventory to their block form:
- 9 Diamonds → 1 Diamond Block
- 9 Iron Ingots → 1 Iron Block
- 9 Gold Ingots → 1 Gold Block
- 9 Emeralds → 1 Emerald Block
- And more...

---

## Disposal

Quickly destroy unwanted items.

### Command

```
/dispose
```

**Rank Required:** Ember Store Rank or higher

Opens a virtual trash can. Any items placed inside are permanently destroyed when you close it.

{% hint style="danger" %}
**Warning:** Items destroyed with `/dispose` cannot be recovered!
{% endhint %}

### Decorative Skulls

```
/skulls
```

**Rank Required:** Rank 7 (Leaf)

Opens a menu with hundreds of decorative skull designs for building.

---

## Armor Stand Editor

Customize armor stands with poses and settings.

### Command

```
/armorstand
```

**Rank Required:** Rank 9 (Branch)

### Features

- Adjust arm and leg positions
- Toggle visibility options
- Set custom poses
- Create detailed displays

---

## World Map

View the server world map in your browser.

### How to Access

Visit the server's Squaremap URL (check in-game or Discord for the link).

### Features

- Chunk claim boundaries
- World border
- Full world exploration

---

## Tips

1. **Check your overflow** — Don't lose valuable items
2. **Use portable workstations** — Save inventory space
3. **Toggle phantoms** — If they annoy you
4. **Invisible frames are craftable** — Stock up on phantom membranes
5. **Animal traps** — Easiest way to move farm animals

---

## Related Pages

- [Ranks Overview](../ranks/overview.md) — When commands unlock
- [Building Tools](tools.md) — File and Trowel
- [Homes](homes.md) — Teleportation
