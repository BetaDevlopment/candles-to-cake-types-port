<p align="center">
  <img src="images/logo.png" alt="Candles to Cake Types" width="560">
</p>

<p align="center">
  <b>Java 1.17 → 26.3 &nbsp;•&nbsp; Bedrock via Geyser &nbsp;•&nbsp; Unofficial port by GalaxyModz</b>
</p>

<p align="center">
  <a href="https://modrinth.com/resourcepack/cake-types"><img src="https://img.shields.io/badge/Original%20pack-Modrinth-1bd96a?style=for-the-badge&logo=modrinth&logoColor=white" alt="Modrinth"></a>
  <img src="https://img.shields.io/badge/Java-1.17%20--%2026.3-orange?style=for-the-badge" alt="Java 1.17 - 26.3">
  <img src="https://img.shields.io/badge/Bedrock-Geyser-blue?style=for-the-badge" alt="Bedrock via Geyser">
</p>

---

## 🎂 What is it?

<img src="images/icon.png" alt="Cake icon" width="96" align="right">

**Candles to Cake Types** is a resource pack by **ARKK & ZAZ** that turns the plain Minecraft cake into **12 different cakes**. You don't need mods or commands, only candles.

This repository is an **unofficial port** of that pack by **GalaxyModz**. It brings the pack to:

- ☕ **Java Edition 1.17 up to 26.3**, from one pack
- 🌉 **Bedrock players on Geyser servers**, so they see the same cakes as Java players, with the same shapes

> [!IMPORTANT]
> **This repo does not contain the original textures.** The original pack is *All Rights Reserved* by ARKK & ZAZ.
> Download it from **[Modrinth](https://modrinth.com/resourcepack/cake-types)** or **[Planet Minecraft](https://www.planetminecraft.com/texture-pack/candles-to-cake-types/)** and run the build script below. Please support the original creators!

## 📸 Showcase

<p align="center">
  <img src="images/showcase.png" alt="All cake types in game">
</p>

## ✨ What does it do?

Put a candle on a cake and it becomes a different kind of cake:

| Candle | Cake | | Candle | Cake |
|---|---|---|---|---|
| *(none)* | Cake without cherries | | 🟫 Brown | Chocolate cake |
| ⬜ White | Cherry cake | | 🟩 Lime | Mint chocolate cake |
| ⬜ Light gray | **Small** cake | | 🟧 Orange | Carrot cake |
| ⬛ Gray | **Two-layer** cake | | 🟨 Yellow | Golden carrot cake |
| 🟦 Light blue | Blue birthday cake 🕯️ | | 🟥 Red | Red velvet cake |
| 🩷 Pink | Pink birthday cake 🕯️ | | ⬛ Black | Cookies & cream cake |

🕯️ The birthday cakes keep their candle. On all the other cakes the candle disappears and only the cake type shows.
Other candle colors look like normal vanilla candle cakes.

## ⚙️ How does it work?

**In game**
1. Place a **whole** cake. You can't add a candle to a cake that has a bite taken out.
2. Right-click it with a candle. The cake changes into the cake type for that color.
3. **Light** the candle with flint and steel and it becomes a normal candle cake again. Blow it out and the cake type comes back.
4. **Eating** a slice drops the candle, as in vanilla.

**Under the hood**
- **Java:** Minecraft has a separate block model for every candle color on a cake. The pack replaces those models with the cake models, so no plugin is needed.
- **Bedrock:** a Bedrock resource pack can't change the shape of vanilla blocks. This port uses **Geyser custom block mappings** instead. Every *unlit* candle cake is sent to Bedrock players as a custom block with its own 3D model (full, small, two-layer, or with a candle). Lit candle cakes stay vanilla, the same as on Java.
- **Multi-version:** `pack.mcmeta` declares both the old (`pack_format` / `supported_formats`) and the new (`min_format` / `max_format`) version fields, so one pack loads from 1.17 to 26.3. On 1.20.2 and newer there's no "made for an older version" warning.

## 📦 Build

You only need **Python 3**. No extra packages are required.

```bash
python build.py path/to/candles-to-cake-types.zip
```

This creates `dist/`:

| File | Use it for |
|---|---|
| `CandlesToCakeTypes_Java_1.17-26.3.zip` | Java players or your Java server resource pack |
| `CandlesToCakeTypes_Server.zip` | Servers with Geyser: Java pack + Geyser pack + block mappings |

## 🌉 Geyser setup

1. Use the Java pack from `Java/` as your server resource pack.
2. Put `Geyser/packs/CandlesToCakeTypes_Geyser.mcpack` in Geyser's `packs` folder.
3. Put `Geyser/custom_mappings/candles_to_cake_types.json` in Geyser's `custom_mappings` folder.
4. Set `enable-custom-content: true` in Geyser's `config.yml`.
5. **Fully restart** the server or proxy. A reload is not enough.

> [!NOTE]
> Bedrock **without** Geyser (single player or Realms) isn't supported. Bedrock doesn't let resource packs give each candle cake its own look, so it only works through Geyser.

## 🔍 Java vs. Bedrock (Geyser)

| | Java | Bedrock via Geyser |
|---|---|---|
| All 12 cake types | ✅ | ✅ |
| Candle hidden on unlit cakes | ✅ | ✅ |
| Small and two-layer cake shapes | ✅ | ✅ |
| Birthday cakes with a burning candle | ✅ | ✅ (light, no flame particles) |

## 🙏 Credits

- **Original pack, textures, logo & idea:** [ARKK](https://modrinth.com/user/ARKK) & [ZAZ](https://modrinth.com/user/ZAZ). [Modrinth](https://modrinth.com/resourcepack/cake-types) · [Planet Minecraft](https://www.planetminecraft.com/texture-pack/candles-to-cake-types/)
- **Bedrock / Geyser port & multi-version update:** **GalaxyModz**
  - 📧 support@galaxymodz.com
  - 💬 Discord: GalaxyModz
  - 🐙 GitHub: [BetaDevlopment](https://github.com/BetaDevlopment)

## 📄 License

The code and configs in this repository (build script, Geyser mappings, Bedrock models) are made by GalaxyModz and released under the [MIT License](LICENSE).
The original pack, its textures, the logo and the icon are **not** covered by this license. They belong to ARKK & ZAZ (All Rights Reserved).

*Not affiliated with Mojang, Microsoft, GeyserMC, or the original creators.*
