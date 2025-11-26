# Essential Commands

A complete reference of all player commands on Oakheart, organized by category.

---

## Navigation & Teleportation

| Command | Description | Notes |
|---------|-------------|-------|
| `/spawn` | Return to Oakheart village | Always available |
| `/wild` or `/rtp` | Random teleport to wilderness | Find a spot to build |
| `/back` | Return to last location | Works after death |
| `/home <name>` | Teleport to a saved home | |
| `/homes` | Open homes GUI menu | |

### Teleport Requests

| Command | Description |
|---------|-------------|
| `/tpa <player>` | Request to teleport to a player |
| `/tpahere <player>` | Request a player to teleport to you |
| `/tpaccept` | Accept a teleport request |
| `/tpdeny` | Deny a teleport request |

---

## Homes

| Command | Description | Default Limit |
|---------|-------------|---------------|
| `/sethome <name>` | Save current location as home | 1 (Rank 1) |
| `/home <name>` | Teleport to a home | |
| `/homes` | View all homes in GUI | |
| `/removehome <name>` | Delete a home | Alias: `/delhome` |

**Home limits increase with rank:** 1 → 15 homes by Rank 20

---

## Land Claims

### Basic Claiming

| Command | Description |
|---------|-------------|
| `/lands create <name>` | Create a new land |
| `/lands claim` | Claim the chunk you're in |
| `/lands unclaim` | Unclaim a chunk |
| `/lands view` | Toggle chunk border display |
| `/lands map` | View ASCII map of claims |
| `/lands menu` | Open main lands GUI |

### Land Management

| Command | Description |
|---------|-------------|
| `/lands info` | View info about current land |
| `/lands list` | List all your lands |
| `/lands rename <name>` | Rename your land |
| `/lands delete` | Delete your land (removes all claims) |
| `/lands setspawn` | Set land's spawn point |
| `/lands spawn` | Teleport to land spawn |

### Trusting Players

| Command | Description |
|---------|-------------|
| `/lands trust <player>` | Add player to your land |
| `/lands untrust <player>` | Remove player from your land |
| `/lands setrole <player> <role>` | Set player's role |

### Selection Mode

| Command | Description |
|---------|-------------|
| `/lands selection` | Enter selection mode |
| `/lands assign <name>` | Create sub-area from selection |

---

## Player Warps

| Command | Description | Rank Required |
|---------|-------------|---------------|
| `/warp` | Open player warps menu | Any |
| `/warp <name>` | Teleport to a warp | Any |
| `/warp set` | Create a warp | Rank 2+ |
| `/warp remove <name>` | Delete your warp | |
| `/warp desc <text>` | Set warp description | |
| `/warp icon` | Set warp icon | |
| `/warp category` | Set warp category | |

**Warp limits:** 0 → 15 warps by Rank 20

---

## Economy & Trading

| Command | Description |
|---------|-------------|
| `/trade <player>` | Open safe trading GUI |
| `/vote` | Open voting sites menu |

### Shops

Interact with NPCs at spawn to buy/sell items. Player shops are created by purchasing a **Shopkeeper Spawn Egg** from Quillfeather the Scribe at spawn (100 emeralds). See [Player Shops](../economy/player-shops.md) for details.

**Shop limits:** 0 → 30 shops by Rank 20 (requires Rank 2+ to create shops)

---

## Communication

| Command | Description | Aliases |
|---------|-------------|---------|
| `/msg <player> <message>` | Private message | /tell, /w, /pm |
| `/reply <message>` | Reply to last PM | /r |
| `/ignore <player>` | Block player's messages | |
| `/mail` | Send/read mail | |

### Chat Features

- Type `[item]` to link held item in chat
- Chat syncs with Discord

---

## Utility Commands (Rank Unlocks)

These commands unlock as you rank up through voting or store ranks.

| Command | Description | Rank |
|---------|-------------|------|
| `/condense` | Convert items to blocks | 3 |
| `/lay` | Lay down animation | 4 |
| `/sit` | Sit on stairs/slabs | 5 |
| `/feed` | Restore hunger | 6 |
| `/loom` | Open loom anywhere | 7 |
| `/skulls` | Decorative skull menu | 7 |
| `/craft` | Open crafting table | 8 |
| `/near` | See nearby players | 9 |
| `/armorstand` | Armor stand editor | 9 |
| `/bellyflop` | Fun emote | 11 |
| `/stonecutter` | Open stonecutter | 12 |
| `/jump` | Fun emote | 13 |
| `/grindstone` | Open grindstone | 14 |
| `/crawl` | Fun emote | 15 |
| `/anvil` | Open anvil | 16 |
| `/ptime` | Set personal time | 17 |
| `/smithingtable` | Open smithing table | 18 |
| `/enderchest` | Access ender chest | 19 |

### Store Rank Exclusive

| Command | Description | Rank |
|---------|-------------|------|
| `/dispose` | Trash items | Ember+ |
| `/cartographytable` | Open cartography | Mythic+ |
| `/heal` | Full health restore | Ascend |

---

## Voting & Ranks

| Command | Description |
|---------|-------------|
| `/vote` | Open voting sites |
| `/prestige` | Prestige (Rank 20 only) |
| `/prestige stats` | View your prestige info |
| `/prestige top` | View prestige leaderboard |

---

## Combat

| Command | Description |
|---------|-------------|
| `/pvp` | Toggle PvP mode |

Both players must have PvP enabled for combat.

---

## Social & Misc

| Command        | Description                                           |                     |
| -------------- | ----------------------------------------------------- | ------------------- |
| `/ping`        | Check your connection                                 |                     |
| `/playtime`    | View your playtime                                    |                     |
| `/playtimetop` | Playtime leaderboard                                  |                     |
| `/afk`         | Toggle AFK status                                     |                     |
| `/tutorial`    | Restart the tutorial                                  |                     |
| `/overflow`    | View overflow inventory                               | Alias: /of          |
| `/claimchunk`  | Withdraw a chunk from your limit into a physical item | Must have >4 chunks |

---

## Staff Assistance

For staff help, open a ticket on **Discord: discord.gg/Oakheart**

---

## Quick Reference Card

```
ESSENTIALS
/spawn              Return to village
/wild               Go to wilderness
/back               Return to last location

HOMES
/sethome <name>     Save location
/home <name>        Teleport to home
/homes              View all homes

CLAIMS
/lands create <n>   Create land
/lands claim        Claim chunk
/lands view         See borders
/lands menu         Open GUI

WARPS
/warp               Browse warps
/warp set           Create warp (Rank 2+)

SOCIAL
/msg <player> <m>   Private message
/trade <player>     Safe trading

VOTING
/vote               Vote for rewards
/prestige           Prestige (Rank 20)
```

---

## Related Pages

- [New Player Guide](new-player-guide.md) — Getting started
- [Ranks Overview](../ranks/overview.md) — Command unlocks
- [Claiming Overview](../claiming/overview.md) — Land commands
