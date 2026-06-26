<div align="center">

# ⚡ SwiftMobile

### A Mobile-First Minecraft Java Performance Modpack

[![Fabric](https://img.shields.io/badge/mod%20loader-Fabric-dbd0b4?style=flat-square)](https://fabricmc.net)
[![Minecraft](https://img.shields.io/badge/Minecraft-1.20.1%20%7C%201.21.1%20%7C%201.21.4-62b36f?style=flat-square)](https://minecraft.net)
[![Based on FO](https://img.shields.io/badge/based%20on-Fabulously%20Optimized-blue?style=flat-square)](https://github.com/Fabulously-Optimized/fabulously-optimized)

> **SwiftMobile** is a Fabric modpack engineered specifically for Android mobile launchers.
> Built on top of [Fabulously Optimized](https://github.com/Fabulously-Optimized/fabulously-optimized),
> it layers in mobile-specific performance boosts to push stable, high FPS on phones and tablets
> — even on low-end hardware.

</div>

---

## 📱 Compatible Launchers

| Launcher | Status |
|---|---|
| **Zalith Launcher 2** | ✅ Fully supported |
| **Zalith Launcher** | ✅ Fully supported |
| **PojavLauncher** | ✅ Fully supported |
| **Modrinth App** (desktop) | ✅ Supported |
| **MultiMC / Prism Launcher** | ✅ Supported |

**Install method:** Download the `.mrpack` from [Releases](../../releases), then import it in your launcher.

---

## ⚡ What Makes SwiftMobile Different

SwiftMobile keeps every optimization from Fabulously Optimized **plus** adds a second layer of
mobile-targeted tweaks that vanilla FO doesn't include:

### Mobile-Exclusive Additions

| Mod | Benefit |
|---|---|
| **Noisium** | 20–30 % faster chunk generation — massive on mobile where CPU is the bottleneck |
| **C2ME** (Concurrent Chunk Management Engine) | Parallel chunk loading across all CPU cores |
| **Exordium** | Renders HUD/GUI elements at a reduced tick rate, freeing GPU for the 3D scene |
| **BadOptimizations** | Micro-optimizations targeting things other mods miss |
| **Clumps** | Merges XP orbs into single entities — huge FPS recovery in mob farms |

### Inherited from Fabulously Optimized

- **Sodium** — fastest open-source renderer available for Fabric  
- **Lithium** — server-side logic and physics optimizations  
- **FerriteCore** — aggressive memory footprint reduction  
- **ModernFix** — dynamic resource loading, faster world join  
- **ImmediatelyFast** — UI and entity rendering speed-ups  
- **EntityCulling** — async path-tracing to skip off-screen entity rendering  
- **MoreCulling** — additional geometry culling passes  
- **Dynamic FPS** — drops render rate when the game is backgrounded  
- **Enhanced Block Entities** — faster chest/sign/banner rendering  
- And ~30 more — see [INCLUDED-MODS.md](INCLUDED-MODS.md)

---

## 📦 Supported Versions

| Minecraft | Status |
|---|---|
| 1.21.4 | ✅ Active (recommended) |
| 1.21.1 | ✅ Active |
| 1.20.1 | ✅ Active (LTS) |
| 1.19.x / 1.18.x / 1.17.x / 1.16.x | 🔒 Legacy (no new mods) |
| 26.x (Bedrock-version-numbered) | 🔒 Legacy |

---

## 🛠 Building from Source

The CI auto-builds on every push to `main`. You can also build locally:

```bash
# 1. Install packwiz
# https://packwiz.infra.link/installation/

# 2. Export for a version
cd Packwiz/1.21.4
packwiz update --all
packwiz refresh
packwiz modrinth export -o ../../SwiftMobile-1.21.4.mrpack
```

---

## 🙏 Credits

- **[robotkoer](https://github.com/robotkoer)** and the Fabulously Optimized team —  
  original modpack this is based on
- **Zen** — SwiftMobile mobile-specific additions and maintenance
- All the mod authors whose work makes this possible

---

<div align="center">
<sub>SwiftMobile is not affiliated with Mojang Studios.</sub>
</div>
