<p align="center">
  <img src="images/logo.png" alt="Candles to Cake Types" width="560">
</p>

<p align="center">
  <b>Java 1.17 → 26.3 &nbsp;•&nbsp; Bedrock via Geyser &nbsp;•&nbsp; Unofficial port by GalaxyModz</b>
</p>

<p align="center">
  <a href="../../releases/latest"><img src="https://img.shields.io/badge/Download-Latest%20release-2ea44f?style=for-the-badge&logo=github" alt="Download"></a>
  <a href="https://modrinth.com/resourcepack/cake-types"><img src="https://img.shields.io/badge/Original%20pack-Modrinth-1bd96a?style=for-the-badge&logo=modrinth&logoColor=white" alt="Modrinth"></a>
  <img src="https://img.shields.io/badge/Bedrock-Geyser-blue?style=for-the-badge" alt="Bedrock via Geyser">
</p>

---

## 🎂 What is it?

<img src="images/icon.png" alt="Cake icon" width="96" align="right">

**Candles to Cake Types** is a resource pack by **ARKK & ZAZ** that turns the plain Minecraft cake into **12 different cakes**. You don't need mods or commands, only candles.

This is an **unofficial port** by **GalaxyModz** that brings the pack to:

- 🌉 **Bedrock players on Geyser servers**, so they see the same cakes as Java players, with the same shapes
- ☕ **Java Edition 1.17 up to 26.3**, from one pack

## 📸 Showcase

<p align="center">
  <img src="images/showcase.png" alt="All cake types in game">
</p>

## ✨ What does it do?

Put a candle on a cake and it becomes a different kind of cake. There are **12 cakes** in total:

<table>
<tr>
<td align="center"><img src="images/cakes/no_candle.png" width="120"><br><b>Cake with no Cherries</b><br><sub>no candle</sub></td>
<td align="center"><img src="images/cakes/white.png" width="120"><br><b>Cake with Cherries</b><br><sub>⬜ white candle</sub></td>
<td align="center"><img src="images/cakes/light_gray.png" width="120"><br><b>Small Cake</b><br><sub>⬜ light gray candle</sub></td>
<td align="center"><img src="images/cakes/gray.png" width="120"><br><b>Double Cake</b><br><sub>⬛ gray candle</sub></td>
</tr>
<tr>
<td align="center"><img src="images/cakes/brown.png" width="120"><br><b>Chocolate Cake</b><br><sub>🟫 brown candle</sub></td>
<td align="center"><img src="images/cakes/lime.png" width="120"><br><b>Mint Chocolate Cake</b><br><sub>🟩 lime candle</sub></td>
<td align="center"><img src="images/cakes/orange.png" width="120"><br><b>Carrot Cake</b><br><sub>🟧 orange candle</sub></td>
<td align="center"><img src="images/cakes/yellow.png" width="120"><br><b>Golden Carrot Cake</b><br><sub>🟨 yellow candle</sub></td>
</tr>
<tr>
<td align="center"><img src="images/cakes/light_blue.png" width="120"><br><b>Blue Birthday Cake</b><br><sub>🟦 light blue candle</sub></td>
<td align="center"><img src="images/cakes/pink.png" width="120"><br><b>Pink Birthday Cake</b><br><sub>🩷 pink candle</sub></td>
<td align="center"><img src="images/cakes/red.png" width="120"><br><b>Red Velvet Cake</b><br><sub>🟥 red candle</sub></td>
<td align="center"><img src="images/cakes/black.png" width="120"><br><b>Cookies and Cream Cake</b><br><sub>⬛ black candle</sub></td>
</tr>
</table>

### 🍰 All cakes in detail

| Cake | Candle | Shape | Look | Candle visible? | Bedrock (Geyser) |
|---|---|---|---|---|---|
| **Cake with no Cherries** | *none* | Full cake | Plain white frosting with a swirl, no cherries | - | ✅ |
| **Cake with Cherries** | White | Full cake | White frosting with red cherries, classic sponge | No | ✅ |
| **Small Cake** | Light gray | **Small** (half width, lower) | Mini cake with one cherry on top | No | ✅ real small shape |
| **Double Cake** | Gray | **Two layers** | Big cake with a small cherry cake stacked on top | No | ✅ real two-layer shape |
| **Chocolate Cake** | Brown | Full cake | Chocolate frosting with a swirl, chocolate sponge | No | ✅ |
| **Mint Chocolate Cake** | Lime | Full cake | Chocolate top with mint pieces, mint drip down the sides | No | ✅ |
| **Carrot Cake** | Orange | Full cake | Cream top with a carrot, layered orange sponge | No | ✅ |
| **Golden Carrot Cake** | Yellow | Full cake | Cream top with a golden carrot, layered golden sponge | No | ✅ |
| **Blue Birthday Cake** | Light blue | Full cake | Blue frosting ring and colorful sprinkles | **Yes** | ✅ (unlit) |
| **Pink Birthday Cake** | Pink | Full cake | Pink frosting ring and colorful sprinkles | **Yes** | ✅ (unlit) |
| **Red Velvet Cake** | Red | Full cake | Cream top with a red ring, red velvet sponge | No | ✅ |
| **Cookies and Cream Cake** | Black | Full cake | White top with cookie pieces, cookies & cream sponge | No | ✅ |

**Good to know**
- 🕯️ The **birthday cakes** keep their candle on top. On all other cakes the candle disappears and only the cake type shows.
- 🔥 **Lit candles:** lighting the candle turns any cake back into a normal candle cake. Blow it out and the cake type comes back.
- 🎨 **Other colors** (cyan, purple, magenta, blue, green) look like normal vanilla candle cakes.
- 🍽️ **Eating** works as normal: you get a slice and the candle drops.

## ⚙️ How does it work?

**In game**
1. Place a **whole** cake. You can't add a candle to a cake that has a bite taken out.
2. Right-click it with a candle. The cake changes into the cake type for that color.
3. **Light** the candle with flint and steel and it becomes a normal candle cake again. Blow it out and the cake type comes back.
4. **Eating** a slice drops the candle, as in vanilla.

**Under the hood**
- **Java:** Minecraft has a separate block model for every candle color on a cake. The pack replaces those models with the cake models, so no plugin is needed.
- **Bedrock:** a Bedrock resource pack can't change the shape of vanilla blocks. This port uses **Geyser custom block mappings** instead. Every *unlit* candle cake is sent to Bedrock players as a custom block with its own 3D model (full, small, two-layer, or with a candle). Lit candle cakes stay vanilla.
- **Multi-version:** the Java pack declares both the old and the new version fields in `pack.mcmeta`, so one pack loads from 1.17 to 26.3.
- **No cache clearing:** every release has a new version number but the same pack ID, so Bedrock players get updates automatically.

## 📥 Download

Get the files from the **[latest release](../../releases/latest)**:

| File | What it is | Where it goes |
|---|---|---|
| `CandlesToCakeTypes_Geyser.mcpack` | Bedrock resource pack | Geyser's `packs` folder |
| `candles_to_cake_types.json` | Geyser block mappings | Geyser's `custom_mappings` folder |
| `CandlesToCakeTypes_Java_1.17-26.3.zip` | Java resource pack | Your server resource pack, or your `resourcepacks` folder |

## 🌉 Server setup (Geyser)

1. Set the **Java pack** as your server resource pack, in `server.properties` or with your resource pack plugin.
2. Put `CandlesToCakeTypes_Geyser.mcpack` in Geyser's **`packs`** folder.
   - Spigot/Paper: `plugins/Geyser-Spigot/packs/`
   - Velocity/BungeeCord: the Geyser folder on your proxy
3. Put `candles_to_cake_types.json` in Geyser's **`custom_mappings`** folder (in the same Geyser folder).
4. In Geyser's `config.yml`, make sure this is on:
   ```yaml
   enable-custom-content: true
   ```
   On newer Geyser versions this setting is under `gameplay:`.
5. **Fully restart** the server or proxy. A reload is not enough.

**Updating:** replace the `.mcpack` and the `.json` with the new ones and restart. You don't need to clear any cache.

> [!NOTE]
> Bedrock **without** Geyser (single player or Realms) isn't supported. Bedrock doesn't let a resource pack give each candle cake its own look, so it only works through Geyser.

## 🔍 Java vs. Bedrock (Geyser)

| | Java | Bedrock via Geyser |
|---|---|---|
| All 12 cake types | ✅ | ✅ |
| Candle hidden on unlit cakes | ✅ | ✅ |
| Small and two-layer cake shapes | ✅ | ✅ |
| Birthday cakes (unlit) | ✅ | ✅ |
| Birthday cakes with a burning candle | ✅ | ⚠️ normal cake with a burning candle |

## ❓ Troubleshooting

| Problem | Fix |
|---|---|
| Bedrock players see normal candle cakes | Check `enable-custom-content: true`, check the `.json` is in `custom_mappings`, and fully restart |
| Cakes are invisible | The `.mcpack` and `.json` come from different releases. Use both from the same release |
| Purple and black textures | The `.mcpack` is missing from `packs`, or the player declined the resource pack |
| Two versions of the pack load | Remove old `.mcpack` files from the `packs` folder |

## 🙏 Credits

- **Original pack, textures, logo & idea:** [ARKK](https://modrinth.com/user/ARKK) & [ZAZ](https://modrinth.com/user/ZAZ). [Modrinth](https://modrinth.com/resourcepack/cake-types) · [Planet Minecraft](https://www.planetminecraft.com/texture-pack/candles-to-cake-types/)
- **Bedrock / Geyser port & multi-version update:** **GalaxyModz**
  - 📧 support@galaxymodz.com
  - 💬 Discord: GalaxyModz
  - 🐙 GitHub: [BetaDevlopment](https://github.com/BetaDevlopment)

Please support the original creators on [Modrinth](https://modrinth.com/resourcepack/cake-types)!

## 📄 License

The textures, logo, icon and original pack belong to **ARKK & ZAZ**.
The Geyser mappings and Bedrock cake models were made by GalaxyModz. See [LICENSE](LICENSE).

*Not affiliated with Mojang, Microsoft, GeyserMC, or the original creators.*
