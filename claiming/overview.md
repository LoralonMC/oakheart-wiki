# Claiming Overview

Oakheart uses a **chunk-based claiming system** to protect your builds from griefing. When you claim land, only you and trusted players can build, break blocks, or access containers within that area.

---

## Quick Start

### Creating Your First Claim

1. **Find a spot** — Use `/wild` to teleport to the survival world
2. **Create your land** — `/lands create <name>` (e.g., `/lands create MyBase`)
3. **Claim the chunk** — `/lands claim` while standing in the chunk
4. **View your claim** — `/lands view` to see chunk borders

{% hint style="success" %}
**Done!** That chunk is now protected. Only you can build or break blocks there.
{% endhint %}

---

## Chunk Limits

### Starting Chunks

| Source | Chunks |
|--------|--------|
| Initial (new player) | 4 |
| Playtime bonus (first 4 hours) | +4 |
| **Total free chunks** | **8** |

You earn +1 chunk per hour of playtime for your first 4 hours on the server.

### Getting More Chunks

**Claim Chunk items** increase your maximum chunks by +1 each when used.

| Source | How to Get |
|--------|-----------|
| **Spawn** | Buy from Quillfeather the Scribe for emeralds |
| **Voting** | Rank-up rewards, Token Trader |
| **Crates** | Vote Crate, Paid Crates |
| **Store** | Direct purchase |
| **Events** | Special server events |
| **Rank-ups** | Bonus chunks at milestone ranks |

{% hint style="info" %}
**Claim Chunks are items!** Right-click them to permanently increase your claim limit. They're tradeable, so you can buy them from other players too.
{% endhint %}

### Bonus Chunks from Ranks

Milestone vote ranks give bonus claim chunks on rank-up:

| Rank | Bonus Chunks |
|------|--------------|
| Rank 5 (Bud) | +2 |
| Rank 10 (Root) | +4 |
| Rank 15 (Willow) | +6 |
| Rank 20 (Yggdrasil) | +8 |

**Total from ranking to 20:** 20 bonus claim chunks!

---

## Essential Commands

### Basic Claiming

| Command                | Description                           |
| ---------------------- | ------------------------------------- |
| `/lands create <name>` | Create a new land with the given name |
| `/lands claim`         | Claim the chunk you're standing in    |
| `/lands unclaim`       | Unclaim the chunk you're standing in  |
| `/lands view`          | Toggle chunk border visualization     |
| `/lands map`           | View map of nearby claims             |

### Land Management

| Command                | Description                                  |
| ---------------------- | -------------------------------------------- |
| `/lands menu`          | Open the main lands GUI                      |
| `/lands info`          | View information about current land          |
| `/lands rename <name>` | Rename your land                             |
| `/lands delete`        | Delete your entire land (removes all claims) |
| `/lands setspawn`      | Set the land's spawn point                   |
| `/lands spawn`         | Teleport to a land's spawn                   |

### Trusting Players

| Command | Description |
|---------|-------------|
| `/lands trust <player>` | Add a player to your land |
| `/lands untrust <player>` | Remove a player from your land |
| `/lands setrole <player> <role>` | Set a player's role in your land |

### Selection Claiming

| Command                          | Description                  |
| -------------------------------- | ---------------------------- |
| `/lands selection`               | Enter selection mode         |
| `/lands selection assign <name>` | Assign selection to sub-area |
| `/lands claim`                   | Claim selected area          |

---

## Trust System

### Roles

You can assign different permission levels to trusted players:

| Role | Permissions |
|------|-------------|
| **Visitor** | Can only interact with doors/buttons |
| **Member** | Can build, break, and access containers |
| **Admin** | Can manage land settings and trust others |

### Trusting a Player

```
/lands trust PlayerName
```

By default, trusted players become Members.

### Setting Roles

```
/lands setrole PlayerName Admin
```

---

## Claim Visualization

### View Mode

Use `/lands view` to toggle chunk border visualization:
- **Green particles** = Your claimed chunks
- **Red particles** = Someone else's claim
- **No particles** = Unclaimed wilderness

### Land Map

Use `/lands map` for a GUI showing:
- Your claims
- Nearby player claims
- Wilderness areas

---

## Claiming Rules

### Do's

- Claim all builds you want protected
- Leave reasonable space between claims (64+ blocks from others)
- Trust only players you know
- Use `/lands view` to check boundaries before building

### Don'ts

- Don't claim around others to box them in
- Don't build offensive structures
- Don't bypass claim protections using exploits
- Don't claim excessive wilderness you won't use

{% hint style="warning" %}
**Respect boundaries!** Building too close to others (within 64 blocks) without permission may result in staff intervention.
{% endhint %}

---

## Claim Expiration

### Standard Claims
Claims from inactive players (90+ days offline) may be removed by staff after review.

{% hint style="info" %}
**Going on a break?** Let staff know via Discord if you'll be away for an extended period. We'll note your account.
{% endhint %}

---

## Claim Protection

### What's Protected

Within your claim:
- Blocks cannot be broken or placed by others
- Containers cannot be accessed (chests, barrels, etc.)
- Animals cannot be killed by others
- Item frames and paintings are protected
- Redstone cannot be triggered by outsiders

### What's NOT Protected

- Mobs can still spawn and damage you
- Environmental damage (creeper/wither explosions) can occur

---

## Claim Disputes

If you have issues with a neighboring claim:

1. **Talk to the player first** — Most issues resolve through communication
2. **Open a Discord ticket** — If you can't resolve it, contact staff
3. **Provide coordinates** — Give exact locations of the dispute

**Never** resolve disputes through griefing or harassment.

---

## Tips for New Players

1. **Claim immediately** — Don't wait until you've built something
2. **Use all 8 free chunks** — More protection = better
3. **Set a spawn** — `/lands setspawn` makes returning easy
4. **Trust carefully** — Only add players you fully trust
5. **Expand smartly** — Plan your base layout before claiming
6. **Check borders** — Use `/lands view` regularly

---

## FAQ

**Q: Can someone grief my unclaimed build?**
A: Technically unclaimed builds are unprotected, but griefing them is still against server rules. Always claim to be safe!

**Q: What happens if I run out of claim chunks?**
A: You can't claim more until you get Claim Chunk items (from voting, crates, store, or trading).

**Q: Can I unclaim and reclaim elsewhere?**
A: Yes! `/lands unclaim` returns that chunk to your available pool.

**Q: Do claims extend underground?**
A: Yes! Claims protect from bedrock to sky limit (full vertical chunk).

**Q: Can mobs spawn in my claim?**
A: Yes, mob spawning is not affected by claims. Use torches/lighting to prevent spawns.

**Q: How do I leave someone else's land?**
A: Use `/lands leave` while in their land.

---

## Related Pages

- [Getting Started with Claims](getting-started.md) — Step-by-step claiming tutorial
- [Claim Chunks](claim-chunks.md) — How to get more chunks
- [Land Management](land-management.md) — Advanced land features
