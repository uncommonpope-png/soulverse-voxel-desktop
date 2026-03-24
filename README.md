# 🌍 Soulverse Voxel Desktop App

**PLT Voxel World – Build, Forge Souls, Explore**

A polished voxel sandbox game with PLT (Profit, Love, Tax) resource system and soul forging mechanics.

---

## 🎮 Features

- **Infinite Procedural Terrain** - Generated with mathematical functions
- **PLT Resource System** - Profit 💰, Love ❤️, Tax ⚖️ bars with regeneration
- **Soul Forging** - Create souls with different PLT distributions
- **Quality Settings** - Low/Medium/High graphics options
- **Full Block Editing** - Place and break blocks with PLT cost/gain
- **Chunk Data Persistence** - World modifications stored in memory
- **World Save/Load** - Save your builds to localStorage, load across sessions
- **First-Person Controls** - WASD movement, mouse look
- **Post-Processing** - Bloom effects for visual polish

---

## 📦 Installation (Desktop App)

### Prerequisites
- Node.js 18+ installed

### Build Steps

```bash
# Navigate to the project folder
cd soulverse-voxel-desktop

# Install dependencies
npm install

# Run in development mode
npm start

# Build installers for your platform
npm run dist
```

### Output

After running `npm run dist`, installers will be in the `dist/` folder:

- **Windows:** `dist/Soulverse Voxel Setup X.X.X.exe`
- **macOS:** `dist/Soulverse Voxel-X.X.X.dmg`
- **Linux:** `dist/Soulverse Voxel-X.X.X.AppImage`

---

## 🎯 Controls

| Key | Action |
|-----|--------|
| **WASD** | Move |
| **SPACE** | Jump |
| **SHIFT** | Sprint |
| **MOUSE** | Look around |
| **LMB** | Break block (gain PLT) |
| **RMB** | Place block (cost PLT) |
| **1-5** | Select block type |
| **CLICK** | Lock pointer |

---

## 🧱 Block Types & PLT

| Block | Icon | PLT Effect |
|-------|------|------------|
| Grass | 🟩 | Free to place |
| Stone | ⬜ | Free to place |
| Profit Gold | 💰 | Costs 5 Profit to place, +2 when broken |
| Love Pink | ❤️ | Costs 5 Love to place, +2 when broken |
| Tax Blue | ⚖️ | Costs 5 Tax to place, +2 when broken |

---

## 💾 Save/Load System

| Button | Action |
|--------|--------|
| **Save World** | Saves all chunks, player position, PLT, souls to localStorage |
| **Load World** | Restores your saved world exactly as you left it |
| **Clear All** | Resets the world (terrain regenerates as you explore) |

**Save Data Includes:**
- All modified chunks (block placements/breaks)
- Player position and stats
- PLT resource levels
- Forged souls
- Selected block

**Storage:** Uses browser localStorage (persists across sessions)

---

## 🌐 Browser Version

Play online without installing:
https://uncommonpope-png.github.io/soulverse-voxel/

---

## 🔧 Development

### Project Structure

```
soulverse-voxel-desktop/
├── index.html      # Main game file (HTML + CSS + JS)
├── main.js         # Electron main process
├── preload.js      # Electron preload script
├── package.json    # Dependencies and build config
└── README.md       # This file
```

### Technologies

- **Three.js** - 3D rendering
- **Electron** - Desktop app wrapper
- **electron-builder** - Cross-platform packaging

---

## 🌀 Soulverse Integration

The game can sync souls with the main Soulverse system via localStorage. Click "Sync with Soulverse" to import your forged souls.

---

## 📊 PLT System

Each soul has three attributes:
- **Profit** 💰 - Influences resource gathering
- **Love** ❤️ - Influences terrain beauty
- **Tax** ⚖️ - Influences resource efficiency

Balance them to create different soul types!

---

## 🚀 Performance

| Quality | Pixel Ratio | Bloom | FPS (est.) |
|---------|-------------|-------|------------|
| Low | 1.0 | 0.3 | 60+ |
| Medium | Device | 0.6 | 30-60 |
| High | Device | 1.0 | 30-45 |

---

## 📝 License

MIT - PLT Press

---

## 👑 Created for

**Craig Jones (Morpheus)** - Grand Code Pope
The Architect of the Soulverse

---

**Version:** 1.0.0 | **Date:** March 23, 2026
