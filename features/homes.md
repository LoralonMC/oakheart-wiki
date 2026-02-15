# Homes

Homes are personal teleport points that let you quickly return to your favorite locations. Unlike player warps, homes are private—only you can use them.

---

## Quick Start

### Setting a Home

Stand where you want to save, then:

```
/sethome <name>
```

Example: `/sethome base`

### Teleporting Home

```
/home <name>
```

Example: `/home base`

### Viewing All Homes

```
/homes
```

Opens a GUI showing all your saved homes.

---

## Home Limits by Rank

| Rank | Homes Allowed |
|------|---------------|
| 1 (Acorn) | 1 |
| 2 | 2 |
| 3 | 3 |
| 4 | 4 |
| 5 | 5 |
| 6 | 6 |
| 7 | 7 |
| 8 | 8 |
| 9 | 9 |
| 10-11 | 10 |
| 12-13 | 11 |
| 14-15 | 12 |
| 16-17 | 13 |
| 18-19 | 14 |
| 20 (Yggdrasil) | 15 |

**Store Ranks** give the same limits as their equivalent vote rank.

---

## Commands

| Command | Description | Alias |
|---------|-------------|-------|
| `/sethome <name>` | Save current location | |
| `/home <name>` | Teleport to home | |
| `/homes` | Open homes GUI | |
| `/removehome <name>` | Delete a home | `/delhome` |

---

## Home Names

### Naming Tips

- Use descriptive names: `base`, `farm`, `shop`, `nether`
- Keep names short for quick typing
- Names are case-insensitive (`Base` = `base`)

### Examples

| Home Name | Use Case |
|-----------|----------|
| `base` | Main base |
| `farm` | Your farm area |
| `shop` | Your player shop |
| `mine` | Mining spot |
| `nether` | Nether hub |
| `end` | End base/farm |
| `grinder` | Mob grinder |
| `storage` | Storage area |
| `spawn` | Near spawn shops |
| `project` | Current build project |

---

## Homes GUI

Use `/homes` to open a visual menu showing all your saved homes.

### Features

- **Click to teleport** — Select any home to go there
- **See coordinates** — View where each home is located
- **Custom icons** — (Rank 10+) Set custom icons for homes
- **Delete homes** — Remove unwanted homes from the GUI

### Home Icons (Rank 10+)

At Vote Rank 10 (Root) or Store Rank Squirrel+, you can set custom icons for your homes in the GUI:

1. Open `/homes`
2. Right-click a home
3. Select "Set Icon"
4. Choose an icon from the menu

This makes it easy to identify your homes at a glance.

---

## Overwriting Homes

If you use `/sethome <name>` with an existing name, it will update that home to your current location.

Example:
```
/sethome base        → Sets "base" at Location A
(move to new spot)
/sethome base        → Updates "base" to Location B
```

{% hint style="warning" %}
**Be careful!** There's no undo for overwriting a home. Make sure you're at the right location before using an existing name.
{% endhint %}

---

## Teleport Warmup

By default, home teleports have a short warmup period. Stay still while the countdown completes.

**Store Rank Benefit:** Hedgehog rank and higher have **instant teleports**—no warmup needed!

---

## Cross-Dimension Homes

You can set homes in different dimensions:

| Dimension | Can Set Homes? |
|-----------|---------------|
| Overworld | Yes |
| Nether | Yes |
| The End | Yes |
| Spawn World | No (use `/spawn`) |

---

## FAQ

**Q: Can other players use my homes?**
A: No, homes are private. Use player warps if you want others to visit.

**Q: Do homes expire?**
A: No, your homes persist indefinitely.

---

## Related Pages

- [Ranks Overview](../ranks/overview.md) — Home limits per rank
- [Player Warps](player-warps.md) — Public teleport points
- [Claiming Overview](../claiming/overview.md) — Protecting your home locations
