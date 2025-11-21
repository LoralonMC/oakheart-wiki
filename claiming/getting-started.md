# Getting Started with Claims

Protect your builds with Oakheart's chunk-based claiming system. This guide walks you through creating your first claim.

---

## Step 1: Find Your Spot

Use `/wild` to teleport to a random location in the wilderness. Look for a good spot to build!

{% hint style="info" %}
Leave at least 64 blocks between your claim and others to avoid conflicts.
{% endhint %}

---

## Step 2: Create Your Land

Once you've found your spot, create a land with a name:

```
/lands create MyBase
```

Replace "MyBase" with whatever you want to call your claim.

---

## Step 3: Claim Your First Chunk

Stand in the chunk you want to protect and run:

```
/lands claim
```

{% hint style="success" %}
**Done!** That 16x16 chunk is now protected from bedrock to sky limit. Only you can build or break blocks there.
{% endhint %}

---

## Step 4: See Your Claim

Toggle chunk border visualization:

```
/lands view
```

- **Green particles** = Your claimed chunks
- **Red particles** = Someone else's claim
- **No particles** = Unclaimed wilderness

---

## Step 5: Claim More Chunks

You start with **4 chunks** and earn +1 per hour for your first 4 hours = **8 free chunks total**.

To claim more chunks, walk into any unclaimed chunk and run `/lands claim`. Your chunks don't need to be connected — claim wherever you need!

---

## Useful Commands

| Command | What It Does |
|---------|--------------|
| `/lands create <name>` | Create a new land |
| `/lands claim` | Claim the chunk you're in |
| `/lands view` | Toggle chunk borders |
| `/lands menu` | Open the lands GUI |
| `/lands map` | Open map GUI of nearby claims |
| `/lands setspawn` | Set your land's spawn point |
| `/lands spawn` | Teleport to your land |

---

## What's Protected?

Within your claim:
- Blocks can't be broken or placed by others
- Chests, barrels, and containers are locked
- Animals can't be killed by others
- Item frames and paintings are safe
- Redstone can't be triggered by outsiders

---

## Next Steps

- [Claim Chunks](claim-chunks.md) — Get more chunks
- [Sub-Areas](sub-areas.md) — Create different zones
- [Land Management](land-management.md) — Trust players, set roles
- [Claiming Overview](overview.md) — Full reference

---

## Quick Tips

1. **Claim immediately** — Don't build first and claim later
2. **Use all 8 free chunks** — More protection is better
3. **Set a spawn** — Makes returning easy with `/lands spawn`
4. **Trust carefully** — Only add players you fully trust
