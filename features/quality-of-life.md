# Quality of Life Features

Oakheart includes several quality-of-life features to make your gameplay smoother and more enjoyable.

---

## Player Settings

Use `/settings` to open a GUI with gameplay toggles you can customize:

| Toggle | What It Does |
|--------|-------------|
| **Phantom Spawning** | Stop phantoms from targeting you |
| **PVP** | Toggle player combat (opt-in) |
| **TP Requests** | Toggle receiving teleport requests |
| **Private Messages** | Toggle receiving PMs |
| **Trade Requests** | Toggle receiving trade requests |
| **Server Announcements** | Toggle timed server messages in chat |
| **Scoreboard Display** | Toggle the sidebar scoreboard |
| **TPS Bossbar** | Toggle the TPS/MSPT/ping bossbar |
| **Player Locator** | Show/hide your location to other players |

You can also manage **Join/Leave Messages** and **NPC Dialogue** from the settings menu.

### NPC Dialogue Toggle

The first time you talk to a key spawn NPC, they walk you through a short introduction. Once you've heard it, you can skip future dialogue and go straight to their menu.

**NPCs that support skip:**
- **Hammerhand the Smith**
- **Stonebeard the Miner**
- **Willowbark the Lumberjack**
- **Seedsower the Farmer**
- **Moonwhisper the Alchemist**
- **Tidecaller the Fisherman**

The toggle remembers per-NPC, so you only skip ones you've actually heard. Re-enable in `/settings` if you want the full intro again later.

{% hint style="info" %}
**Phantom note:** When phantoms are toggled off, your sleep deprivation still builds up — phantoms simply won't spawn for *you*. You can still encounter phantoms spawned by other players.
{% endhint %}

---

## Invisible Item Frames

Create cleaner displays by making item frames invisible while keeping the item visible.

### How to Craft

Surround a {{item:phantom_membrane}} with item frames in a crafting table:

**Normal Invisible Frame:**

```crafting
item_frame, item_frame, item_frame
item_frame, phantom_membrane, item_frame
item_frame, item_frame, item_frame
=> invisible_item_frame
```

**Glow Invisible Frame:**

```crafting
glow_item_frame, glow_item_frame, glow_item_frame
glow_item_frame, phantom_membrane, glow_item_frame
glow_item_frame, glow_item_frame, glow_item_frame
=> invisible_glow_item_frame
```

### Use Cases

- **Map walls** — Seamless map displays
- **Decorations** — Floating items as decoration
- **Shops** — Clean item displays for player shops
- **Museums** — Display items without visible frames

---

## Overflow Inventory

A safety net for when your inventory is full. Instead of items dropping on the ground (and risking despawn or theft), they go into your personal overflow until you're ready to claim them.

### Commands

| Command | Description |
|---------|-------------|
| `/overflow` (or `/of`) | Open your overflow inventory |
| `/overflow count` | See how many items are waiting |
| `/overflow claimall` | Claim everything at once |

### When Overflow Activates

- Mob drops you couldn't pick up (within ~5 blocks of where they fell)
- Crate rewards when inventory is full
- Rank-up rewards and trade outputs
- Any server- or plugin-given items

### Things to know

- Storage is **unlimited** — no cap, no expiry
- Items **never auto-delete** even if you don't claim them
- Pickup radius is per-player — your overflow won't capture another player's drops
- Works with custom items the same as vanilla

{% hint style="warning" %}
**Check regularly!** Items in overflow don't despawn, but it's easy to forget they're there.
{% endhint %}

---

## Explosion Rebuild

Creeper holes and other mob explosions automatically rebuild themselves so they don't permanently scar the world.

### What rebuilds

| Source | Rebuilds? |
|--------|-----------|
| Creepers | ✅ Yes |
| Ghast fireballs | ✅ Yes |
| Wither skull projectiles | ✅ Yes |
| Wither spawn explosion | ✅ Yes |
| **TNT** | ❌ No (intentional — keeps redstone & farms working) |
| **End Crystals** | ❌ No (intentional) |

Blocks return from the top down with a small cloud particle effect — the area heals on its own, no command needed. Items dropped by the explosion are not affected.

{% hint style="info" %}
**Why TNT is excluded:** TNT blasts in your own builds (cobblestone generators, mob farms, demolition projects) work as expected — only mob-caused damage gets reverted.
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
| `/spin` | Spin on the spot | Phoenix |

---

## Jump

Quickly teleport in the direction you're looking.

### Command

```
/jump
```

**Rank Required:** Rank 13 (Glade)

Teleports you approximately 30 blocks in the direction you're looking. Useful for quickly crossing gaps or reaching distant ledges.

{% hint style="warning" %}
**Be careful!** Make sure there's solid ground where you're aiming, or you might fall.
{% endhint %}

---

## Useful Commands

| Command | Description | Rank Required |
|---------|-------------|---------------|
| `/feed` | Restore your hunger and saturation | Rank 6 |
| `/near` | See nearby players | Rank 9 |
| `/heal` | Fully restore your health | Rank 20 |

---

## Portable Workstations

Access crafting interfaces anywhere without placing blocks.

| Command | Description | Rank Required |
|---------|-------------|---------------|
| `/craft` | Open crafting table (aliases: `/wb`, `/workbench`) | Rank 8 |
| `/loom` | Open loom | Rank 7 |
| `/stonecutter` | Open stonecutter | Rank 12 |
| `/grindstone` | Open grindstone | Rank 14 |
| `/anvil` | Open anvil | Rank 16 |
| `/smithingtable` | Open smithing table | Rank 18 |
| `/cartographytable` | Open cartography table | Rank 2 |

---

## Personal Time

Control your personal day/night cycle without affecting other players.

### Command

```
/ptime <time>
```

**Rank Required:** Rank 17 (Yewshade)

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

## Personal Weather

Control your personal weather without affecting other players.

### Command

```
/pweather <type>
```

**Rank Required:** Rank 17 (Yewshade)

### Options

| Value | Effect |
|-------|--------|
| `sun` | Always clear skies for you |
| `rain` | Always raining for you |
| `reset` | Return to server weather |

{% hint style="info" %}
This only changes what *you* see. Other players and weather mechanics follow server weather.
{% endhint %}

---

## Remote Ender Chest

Access your ender chest from anywhere.

### Command

```
/enderchest
```

**Rank Required:** Rank 19 (Gloaming)

Aliases: `/ec`

---

## Item Condensing

Quickly convert items into their block form.

### Command

```
/condense
```

**Rank Required:** Rank 3 (Orchard)

### What It Does

Converts items in your inventory to their block form:
- {{item:diamond:9}} → {{item:diamond_block}}
- {{item:iron_ingot:9}} → {{item:iron_block}}
- {{item:gold_ingot:9}} → {{item:gold_block}}
- {{item:emerald:9}} → {{item:emerald_block}}
- And more...

---

## Disposal

Quickly destroy unwanted items.

### Command

```
/dispose
```

**Rank Required:** Rank 10 (Hollow) or Squirrel Store Rank+

Aliases: `/trash`

Opens a virtual trash can. Any items placed inside are permanently destroyed when you close it.

{% hint style="danger" %}
**Warning:** Items destroyed with `/dispose` cannot be recovered!
{% endhint %}

---

## Decorative Heads

```
/heads
```

**Rank Required:** Rank 7 (Bracken)

Opens a menu with hundreds of decorative head designs for building. Great for custom furniture, signs, and decoration details.

---

## Armor Stand Editor

Customize armor stands with poses and settings.

### Command

```
/armorstand
```

**Rank Required:** Rank 9 (Fernbrake)

### Features

- Adjust arm and leg positions
- Toggle visibility options
- Set custom poses
- Create detailed displays

---

## World Map

View the live server map in your browser at **[oakheart.net/map](https://oakheart.net/map)**.

### What You'll See

- **Live player positions** — everyone online right now; click a name in the side panel to jump to them
- **Land claims** — claim boundaries drawn on the map; click one to see who owns it
- **Every world** — switch between Overworld, Spawn, Nether, and The End
- The world border and full explored terrain

### Measure: The Builder's Planning Tool

The ruler button (📏 *Measure distance*) in the top corner turns the map into a layout tool. It's the fastest way to plan a large build before you place a single block.

- **Click to place points.** Each one snaps to a block and shows its exact X, Z coordinates
- **Drag a point** to move it, or **right-click** it to remove it
- **Click a line** to insert a new point partway along it
- **Click your first point again** to close the shape, which gives you the enclosed area
- Every segment is labelled with its length, plus a running total
- In the Overworld it also shows the **Nether equivalent** distance, and in the Nether the Overworld equivalent, which makes portal linking much easier
- **Copy** puts the whole thing on your clipboard: total distance, area, and every corner coordinate, ready to paste into Discord

Press `Esc` to cancel a measurement in progress.

> The map is top-down only, so it plans footprints, plot sizes, and distances. It won't show you height or elevation.

### Bookmarks

Open the side panel and use the **+** next to Bookmarks to save wherever you're looking, then click it later to jump straight back. Bookmarks live in your own browser, so they're private to you and don't follow you to another device.

### Sharing and Fullscreen

The link button copies a URL pointing at exactly the view you're on, so you can send someone a spot instead of describing it. The corner button goes fullscreen.

### Hiding Your Location

If you'd rather not show up on the map, turn on the map-hidden option in your in-game Player Settings menu. You'll still show in the online player list, but your position won't be shared.

---

## Related Pages

- [Ranks Overview](../ranks/overview.md) — When commands unlock
- [Building Tools](tools.md) — File and Trowel
- [Homes](homes.md) — Teleportation
