# Sub-Areas

Sub-areas allow you to create **zones within your land** that have different permissions from the main area. This is useful for public shops, community farms, or restricted sections.

---

## What Are Sub-Areas?

A sub-area is a section of your claimed land with its own permission settings. Think of it as "rooms" within your "house":

- **Main land** = Your house (default permissions)
- **Sub-areas** = Individual rooms (custom permissions each)

### Common Use Cases

| Use Case | Example Setup |
|----------|---------------|
| **Public Shop** | Allow visitors to interact with shop NPCs |
| **Community Farm** | Let anyone harvest but not break blocks |
| **Private Storage** | Extra restrictions even for trusted members |
| **Guest Area** | Welcome zone with limited access |

---

## Creating Sub-Areas

### Step 1: Enter Selection Mode

```
/lands selection
```

This allows you to select an area within your land.

### Step 2: Select the Area

- **Left-click** a block to set the first corner
- **Right-click** a block to set the second corner

The selection covers all blocks between these two points (including vertically).

### Step 3: Create the Sub-Area

```
/lands assign <subarea-name>
```

Example: `/lands assign PublicShop`

{% hint style="info" %}
**Sub-areas must be within your claimed land!** You can't create a sub-area in wilderness or someone else's claim.
{% endhint %}

---

## Managing Sub-Areas

### View Sub-Areas

Open the lands menu to see all your sub-areas:

```
/lands menu
```

Navigate to the sub-areas section to manage them.

### Rename a Sub-Area

```
/lands rename <old-name> <new-name>
```

### Delete a Sub-Area

```
/lands delete <subarea-name>
```

This removes the sub-area but keeps the chunks claimed to your main land.

---

## Sub-Area Permissions

Each sub-area can have different flag settings from your main land.

### Common Flags

| Flag | Description |
|------|-------------|
| `BLOCK_BREAK` | Allow/deny breaking blocks |
| `BLOCK_PLACE` | Allow/deny placing blocks |
| `INTERACT_CONTAINER` | Allow/deny opening chests |
| `INTERACT_DOOR` | Allow/deny using doors |
| `INTERACT_VILLAGER` | Allow/deny trading with villagers |
| `INTERACT_GENERAL` | Allow/deny buttons, levers, etc. |
| `ATTACK_ANIMAL` | Allow/deny killing animals |

### Setting Flags

Use the lands menu (`/lands menu`) to adjust flags for specific sub-areas, or:

```
/lands edit <subarea-name>
```

Then modify settings through the GUI.

---

## Sub-Area Roles

Just like your main land, sub-areas can have different roles:

| Role | Typical Permissions |
|------|-------------------|
| **Visitor** | Only what you specifically enable |
| **Member** | Build, break, and access containers |
| **Admin** | Full control of the sub-area |

### Trust Players to Sub-Areas

You can trust players specifically to sub-areas without giving them access to your entire land.

---

## Example: Public Shop Sub-Area

Here's how to create a public shop area:

1. **Claim your land normally**
   ```
   /lands create MyBase
   /lands claim
   ```

2. **Build your shop building**

3. **Enter selection mode**
   ```
   /lands selection
   ```

4. **Select the shop interior** (left-click one corner, right-click opposite corner)

5. **Create the sub-area**
   ```
   /lands assign Shop
   ```

6. **Configure permissions** via `/lands menu`:
   - Enable `INTERACT_VILLAGER` for Visitors
   - Enable `INTERACT_DOOR` for Visitors
   - Keep `BLOCK_BREAK` disabled for Visitors

Now anyone can enter your shop, open doors, and trade with your shopkeepers, but they can't break anything!

---

## Example: Community Farm Sub-Area

1. **Create the sub-area** in your farm section
2. **Enable for Visitors:**
   - `INTERACT_GENERAL` (use hoes)
   - `BLOCK_BREAK` for specific blocks (crops only if supported)
3. **Keep disabled:**
   - `BLOCK_PLACE` (prevent random blocks)
   - `INTERACT_CONTAINER` (protect seed chests)

---

## Tips

1. **Plan before building** — Design your base with sub-areas in mind
2. **Test permissions** — Have a friend test that they can/can't do what you expect
3. **Use descriptive names** — "PublicShop" is better than "Area1"
4. **Don't over-complicate** — Start simple, add sub-areas as needed
5. **Keep valuable items outside sub-areas** — Extra security for important storage

---

## Troubleshooting

**"You don't have permission to create sub-areas"**
- Make sure you're the owner or admin of the land
- Verify you're selecting within your claimed chunks

**"Selection is outside your land"**
- Both corners must be within chunks you own
- Use `/lands view` to see your claim boundaries

**"Players can't access my shop"**
- Check that `INTERACT_VILLAGER` is enabled for Visitors
- Verify the shopkeeper NPC is inside the sub-area boundaries

---

## Related Pages

- [Claiming Overview](overview.md) — Basic claiming guide
- [Land Management](land-management.md) — Advanced land features
