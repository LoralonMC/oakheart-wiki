# Land Management

Advanced features for managing your land, trusting players, and organizing your claims.

---

## Trusting Players

### Adding Players

```
/lands trust <player>
```

Trusted players become **Members** by default, allowing them to build, break, and access containers in your land.

### Removing Players

```
/lands untrust <player>
```

---

## Roles

Assign different permission levels to trusted players:

| Role | Permissions |
|------|-------------|
| **Visitor** | Can only interact with doors and buttons |
| **Member** | Can build, break, and access containers |
| **Admin** | Can manage land settings and trust others |

### Setting Roles

```
/lands setrole <player> <role>
```

Example: `/lands setrole Steve Admin`

---

## Land Settings

### Renaming Your Land

```
/lands rename <new name>
```

### Setting a Spawn Point

```
/lands setspawn
```

Then use `/lands spawn` to teleport there.

### Deleting Your Land

```
/lands delete
```

{% hint style="danger" %}
This removes ALL your claims. Make sure you want to do this!
{% endhint %}

---

## Managing Claims

### Unclaiming Chunks

Stand in a chunk you own and run:

```
/lands unclaim
```

The chunk returns to your available pool.

### Viewing Your Claims

| Command | Description |
|---------|-------------|
| `/lands view` | Toggle chunk border particles |
| `/lands map` | Open map GUI of nearby claims |
| `/lands info` | Info about your land |

---

## Banning Players

Block specific players from entering your land:

```
/lands ban <player>
```

Unban with:

```
/lands unban <player>
```

---

## Land Menu

Open the full lands GUI for easy management:

```
/lands menu
```

From here you can:
- View and manage trusted players
- Adjust land settings
- See claim statistics
- Manage roles and permissions

---

## Claim Expiration

### Standard Claims
Claims from inactive players (90+ days offline) may be removed by staff after review.

### Permanent Claims
**Vote Rank 20 (Yggdrasil)** and **Store Rank Ascend** have permanent claims that never expire.

{% hint style="info" %}
**Going on a break?** Let staff know via Discord if you'll be away for an extended period.
{% endhint %}

---

## Command Reference

| Command | Description |
|---------|-------------|
| `/lands trust <player>` | Add player to your land |
| `/lands untrust <player>` | Remove player from land |
| `/lands setrole <player> <role>` | Set player's role |
| `/lands ban <player>` | Ban player from land |
| `/lands unban <player>` | Unban player |
| `/lands rename <name>` | Rename your land |
| `/lands setspawn` | Set land spawn point |
| `/lands spawn` | Teleport to land spawn |
| `/lands delete` | Delete entire land |
| `/lands unclaim` | Unclaim current chunk |
| `/lands menu` | Open lands GUI |
| `/lands info` | View land information |

---

## Related Pages

- [Claiming Overview](overview.md)
- [Getting Started with Claims](getting-started.md)
- [Sub-Areas](sub-areas.md)
- [Claim Chunks](claim-chunks.md)
