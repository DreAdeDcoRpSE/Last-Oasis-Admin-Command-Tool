# 🛠️ Last Oasis Admin Command Tool

A lightweight, browser-based utility designed for **Last Oasis** server administrators. Quickly generate complex admin commands without memorizing syntax, item IDs, or entity names. This tool runs entirely offline in your browser—no installation or server-side requirements needed.

**- Older image, but still similar**

<img src="https://github.com/user-attachments/assets/773c2c8b-3e3f-4650-aa05-acecd1678fc0" width="600" />



**- Command Listing**

<img src="https://github.com/user-attachments/assets/e41761b2-1a5c-4cf2-a80c-5c2b46757fbe" width="600" />


**- Search Feature**

<img src="https://github.com/user-attachments/assets/6a0a2fab-1d91-4b6c-8d42-5e4789edc0a9" width="600" />

## ✨ Features

- **📋 Command Generator:** Supports all major admin commands (`/GiveItem`, `/SpawnWalker`, `/Teleport`, `/SpawnLootsite`, etc.).
- **🔍 Search:** You can search for specific items and walker easily.
- **🎒 Item Database:** Extensive categorized lists for Weapons, Armor, Resources, Modules, Schematics, and more.
- **🐾 Entity Grids:** Visual selection grids for Walkers, Mobs, and Loot Sites.
- **⚙️ Customizable Sets:** Pre-configured Item Sets (e.g., Starter, PvP, Builder) editable via script.
- **🎨 Theme Support:** Toggle between **Dark** and **Light** modes.
- **📱 Responsive:** Works on desktop and mobile browsers.
- **🔒 Privacy:** Runs locally in your browser. No data is sent to any server.


## 🚀 Installation

1. Click the **Code** button at the top of this repository and select **Download ZIP**.
2. Extract the folder.
3. Locate `index.html` (or the main `.html` file).
4. Double-click to open it in your preferred web browser (Chrome, Firefox, Edge, etc.).

## 📖 How to Use

1. **Select Command:** Choose the desired admin command from the dropdown menu.
2. **Fill Parameters:** 
   - For items/mobs/walkers, click the desired item in the grid.
   - For numbers (Amount, Distance, Quality), use the input fields.
3. **Generate:** Click the **Get Command** button.
4. **Copy:** Click **Copy** to copy the generated string to your clipboard.
5. **Paste:** Paste into your server console or admin chat.

## ⚙️ Customization

This tool is designed to be easily edited to match your specific server configuration. Open the `.html` file in a text editor (like Notepad++ or VS Code) and locate the `gameData` object in the `<script>` section.

### Editing Item Sets
To change the presets for `/GiveItemSet` or `/EquipItemSet`, find the `itemSets` array:

```javascript
itemSets: [
    { name: "Starter Set", cmd: "1" }, 
    { name: "PvP Set", cmd: "2" }, 
    { name: "Builder Set", cmd: "3" }
]
```

### Adding Custom Data!

You can add new items, walkers, or mobs to the respective categories within `gameData`. Ensure you follow the `{ name: "Display Name", cmd: "InternalID" }` format.

## ⚠️ Important Notes

- **Unstable Items:** Items marked with a `*` (yellow highlight) may be deprecated or unstable in the current game version.
- **Distance Values:** A distance value of `25000` is approximately **1/4th of a grid square**.
- **Loot Site Quality:** As of the last update, the "Quality" parameter for `/SpawnLootsite` may not affect the generated loot.
- **Game Updates:** Command syntax or item IDs may change with game patches. Use with caution on live servers.

## 🤝 Contributing

Feel free to fork this repository and submit pull requests if you find bugs or want to add new commands/items to the database.

## 📄 License & Credits

- **Created for:** The Last Oasis Community
- **Created by:** coRpSE
- **Website:** [headshotdomain.net](https://www.headshotdomain.net)
- **Copyright:** © [headshotdomain.net](https://www.headshotdomain.net)

---

*May your walkers walk tall and your water sacks never leak.* 🐪💧
