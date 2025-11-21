# Sub-Areas

Sub-areas allow you to create **zones within your land** that have different permissions from the main area. This is useful for public shops, community farms, or restricted sections.

---

## What Are Sub-Areas?

A sub-area is a **3D zone** within your claimed land with its own permission settings. Unlike chunks (which are column-based), sub-areas are defined by specific blocks, giving you precise control over smaller regions.

Think of it as "rooms" within your "house":

- **Main land** = Your house (default permissions for all blocks not in a sub-area)
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

### Step 1: Create the Area in Menu

```
/lands menu
```

Navigate to the **Areas** section and click the "Add Area" button. Enter a name for your sub-area in chat.

### Step 2: Enter Selection Mode

```
/lands selection
```

This allows you to define the boundaries of your sub-area.

### Step 3: Select the Boundaries

- **Left-click** a block to set the first corner
- **Right-click** a block to set the second corner

The selection covers all blocks between these two points in 3D space.

### Step 4: Assign the Selection

```
/lands selection assign <area-name>
```

Example: `/lands selection assign PublicShop`

{% hint style="info" %}
**Sub-areas must be within your claimed land!** You can't create a sub-area in wilderness or someone else's claim.
{% endhint %}

---

## Managing Sub-Areas

### Accessing Sub-Area Settings

Open the lands menu to see all your sub-areas:

```
/lands menu
```

Navigate to the **Areas** section to manage them.

You can also access a specific sub-area's menu by standing inside it and using:

```
/lands menu here
```

From the menu, you can trust players, set flags, and manage the sub-area's settings.

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

Use `/lands menu` and navigate to the Areas section, or use `/lands menu here` while standing in the sub-area to adjust its flags through the GUI.

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

3. **Create the sub-area via menu**
   - Open `/lands menu`
   - Go to **Areas** → **Add Area**
   - Type `Shop` in chat

4. **Enter selection mode**
   ```
   /lands selection
   ```

5. **Select the shop interior** (left-click one corner, right-click opposite corner)

6. **Assign the selection to your area**
   ```
   /lands selection assign Shop
   ```

7. **Configure permissions** via `/lands menu here` while in the shop:
   - Enable `INTERACT_VILLAGER` for Visitors
   - Enable `INTERACT_DOOR` for Visitors
   - Keep `BLOCK_BREAK` disabled for Visitors

Now anyone can enter your shop, open doors, and trade with your shopkeepers, but they can't break anything!

---

## Example: Community Farm Sub-Area

1. **Create the area** via `/lands menu` → Areas → Add Area → name it `Farm`
2. **Select and assign** using `/lands selection` then `/lands selection assign Farm`
3. **Enable for Visitors:**
   - `INTERACT_GENERAL` (use hoes)
   - `BLOCK_BREAK` for specific blocks (crops only if supported)
4. **Keep disabled:**
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
