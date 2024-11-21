
# 🌀 Gamestorm Backpack

A free and lightweight script for adding persistent backpacks to your server using `ox_inventory`.

---

## ✨ Features
- **0.0 ms Usage**: Optimized for performance.
- **Persistent Backpack Prop**: Automatically adds a backpack to the player's back when in inventory.
- **Customizable Parameters**: Easily configure item names and storage capacities.
- **Framework Compatibility**: Works seamlessly with `ox_core`, `ESX`, `QBCore`, and any other framework supporting `ox_inventory`.

---

## 🚀 Installation

### Follow these simple steps:
1. **Download** the script from the [Gamestorm Backpack Repository](https://github.com/GAMESTORMZONE/gamestorm-backpack.git).
2. **Add the Backpack Item** to your inventory as described in the [Extra Information](#extra-information) section below.
3. **Add Backpack Image** to your inventory images:
   - Copy the image located at `gamestorm_backpack\_inventory_images\backpack.png` to your inventory image directory.
4. **Place the Script** in your `resources` directory.
5. Add the following line to your `server.cfg` file:
   ```bash
   ensure gamestorm_backpack
   ```
   - Ensure this line is placed **after** `ox_lib` but **before** `ox_inventory`.

---

## 📜 Dependencies
- [ox_inventory](https://github.com/overextended/ox_inventory)

---

## 🔧 Extra Information

To add the backpack item, include this in your `ox_inventory/data/items.lua` file:
```lua
['backpack'] = {
    label = 'Backpack',
    weight = 220,
    stack = false,
    consume = 0,
    client = {
        export = 'gamestorm_backpack.openBackpack'
    }
},
```

---

## 🎥 Preview

Check out how it works in the [Live Preview](https://gamestormzone.github.io/photos.html).

---

## 🛠️ Support

If you need assistance or want to stay updated, join our **[Discord Server](https://discord.gg/SR9S6GgNME)**.

<a href='https://discord.gg/SR9S6GgNME'>
  <img src='https://github.com/GAMESTORMZONE/gamestorm-backpack/blob/main/backpack.png' alt='Discord Banner'>
</a>
