# Player Warps

Player warps let you create teleport points that other players can use to visit your builds, shops, farms, and more.

---

## Requirements

**Minimum Rank:** Vote Rank 2 (Sprout) or any Store Rank

You must reach at least Rank 2 to create warps. This requires just **5 votes**—achievable on your first day!

---

## Warp Limits by Rank

| Rank | Warps Allowed |
|------|---------------|
| 1 (Acorn) | 0 |
| 2-3 | 1 |
| 4-5 | 2 |
| 6-7 | 3 |
| 8-9 | 4 |
| 10-11 | 5 |
| 12-13 | 6 |
| 14-15 | 7 |
| 16-17 | 8 |
| 18-19 | 9 |
| 20 (Yggdrasil) | 10 |

---

## Creating Your First Warp

### Step 1: Choose a Location

Stand exactly where you want players to teleport. Consider:
- Is the landing spot safe?
- Can visitors clearly see what this warp is for?
- Is it within your claimed land?

### Step 2: Create the Warp

```
/pwarp set <name>
```

Example: `/pwarp set MyShop`

{% hint style="info" %}
**Your first warp is free!** Additional warps cost 20 emeralds each.
{% endhint %}

### Step 3: Customize (Optional)

Set a description, icon, and category to help others find your warp.

---

## Commands

### Basic Commands

| Command | Description |
|---------|-------------|
| `/pwarp` | Open the warps browser GUI |
| `/pwarp <name>` | Teleport to a specific warp |
| `/pwarp list` | View all available warps |
| `/pwarp set <name>` | Create a new warp |
| `/pwarp remove <name>` | Delete your warp |

### Customization Commands

| Command | Description |
|---------|-------------|
| `/pwarp desc <text>` | Set warp description |
| `/pwarp icon` | Set the warp's icon (from GUI) |
| `/pwarp category` | Choose warp category |
| `/pwarp rename <old> <new>` | Rename a warp |
| `/pwarp reset <name>` | Reset warp to current location |

### Access Control

| Command | Description |
|---------|-------------|
| `/pwarp lock <name>` | Make warp private |
| `/pwarp password <name> <pass>` | Set password for warp |
| `/pwarp whitelist <name> <player>` | Allow specific player access |
| `/pwarp ban <name> <player>` | Ban player from your warp |

### Management

| Command | Description |
|---------|-------------|
| `/pwarp favourite <name>` | Add warp to favorites |
| `/pwarp rate <name>` | Rate another player's warp |
| `/pwarp managers <name> <player>` | Add co-manager to warp |
| `/pwarp setowner <name> <player>` | Transfer warp ownership |

---

## Warp Categories

When creating a warp, choose a category to help players find it:

| Category | Best For |
|----------|----------|
| **Shops** | Player shops, trading posts |
| **Farms** | Public or showcase farms |
| **Grinders** | Mob grinders, XP farms |
| **Special** | Unique builds, attractions |
| **Towns** | Community areas, towns |

More categories may be added as the server grows.

---

## Warp Costs

| Action | Cost |
|--------|------|
| First warp | **Free** |
| Additional warps | 20 emeralds each |

---

## Sponsored Warps

Want premium visibility for your warp? Rent a **sponsored slot** to appear at the top of the warp menu!

| Slot | Duration | Cost |
|------|----------|------|
| Sponsored Slot 1 | 7 days | 150 emeralds |
| Sponsored Slot 2 | 3 days | 75 emeralds |
| Sponsored Slot 3 | 1 day | 30 emeralds |

Sponsored warps appear prominently in the warp browser, driving more visitors to your location.

---

## Warp Tips

### Naming Your Warp

**Do:**
- Use clear, descriptive names: `IronFarm`, `DiamondShop`, `MyTown`
- Keep it short and memorable
- Use relevant keywords

**Don't:**
- Use misleading names
- Include inappropriate words
- Copy other players' warp names

### Warp Location Best Practices

1. **Safe landing** — No lava, long drops, or hostile mobs at spawn point
2. **Clear signage** — Put signs explaining what visitors can do
3. **Claimed land** — Set warps inside your claims for security
4. **Accessible** — Don't make visitors solve puzzles to leave

### Growing Your Warp's Popularity

1. **Good description** — Explain what visitors will find
2. **Custom icon** — Stand out in the menu
3. **Correct category** — Help the right people find you
4. **Keep it stocked** — If it's a shop, maintain inventory
5. **Ask for ratings** — Good ratings boost visibility

---

## Warp Etiquette

### As a Warp Owner

- Keep your warp functional and maintained
- Don't create trap warps that harm visitors
- Update or remove warps you no longer maintain
- Respond to questions about your warp

### As a Visitor

- Respect the warp owner's builds
- Don't grief or steal (against server rules!)
- Leave a rating if you enjoyed your visit
- Report problematic warps to staff

---

## Troubleshooting

**"You've reached your warp limit"**
- You need a higher rank for more warps
- Vote to rank up, or remove unused warps

**"You need 20 emeralds"**
- First warp is free; additional warps cost emeralds
- Sell items at spawn shops to earn emeralds

**"A warp with that name already exists"**
- Choose a different name
- Names must be unique server-wide

**"You can't set warps here"**
- You may be in a restricted area
- Make sure you're in the survival world

---

## Private Warps

Want a warp just for friends? Use access control:

1. Create your warp: `/pwarp set SecretBase`
2. Lock it: `/pwarp lock SecretBase`
3. Whitelist friends: `/pwarp whitelist SecretBase FriendName`

Or set a password:
1. `/pwarp password MyWarp secretcode`
2. Share the password only with trusted players

---

## Related Pages

- [Ranks Overview](../ranks/overview.md) — Warp limits per rank
- [Economy Overview](../economy/overview.md) — Earning emeralds for warps
- [Player Shops](../economy/player-shops.md) — Setting up shops at warps
