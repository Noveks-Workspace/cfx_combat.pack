# 🛡️ Noveks Combat Logging Script

**Version:** 1.2.1 
**Developer:** Novek  
**Discord:** [Join Support Discord](https://discord.gg/8q8BnmgXq2)  
**Tebex Store:** [Buy Here](https://noveks-workspace.tebex.io/package/6505498)  

---

## 📄 Overview

The **Noveks Combat Logging Script** ensures fair play by logging all player disconnects, especially during combat. Notifications are sent to a Discord channel, and players or admins are alerted in-game. This script helps you maintain transparency and control over combat logging incidents.

---

## 🔧 **Features:**

- 🛡️ **Discord Logging:**  
  Logs every disconnect to a specified Discord channel, providing detailed insights.

- ⏳ **Customizable Settings:**  
  Control text appearance, logging behavior, and alert durations through an easy-to-edit config.

- 📣 **In-Game Notifications:**  
  Display customizable alerts when players leave during combat, enhancing server awareness.

- 🚀 **Optimized Performance:**  
  Lightweight with minimal resource usage, ensuring smooth server operation.

---

## 📑 **Requirements:**

- **ESX 1.2** or **ESX Legacy**  

---

## 🛠️ **Installation:**

1. **Download the Script:**  
   Place the script files into your server’s **`resources`** folder.

2. **Add to `server.cfg`:**  
   ```lua
   ensure Noveks_CombatLog
   ```

3. **Configure the Script:**  
   Edit the `config.lua` file with your preferred settings and webhook URL.

---

## 📝 **Configuration Example:**

Customize the script by editing the `config.lua` file:

```lua
Noveks_CFG = {}

-- ================================================
-- Discord Logging
Noveks_CFG.DiscordWebhook = "YOUR_DISCORD_WEBHOOK_URL"  -- Replace this with your Discord webhook URL

-- ================================================
-- Drawing Time Settings (in milliseconds)
Noveks_CFG.DrawingTime = 20 * 1000                      -- Duration: 20 seconds (20,000 ms)

-- ================================================
-- Text Color Settings (RGB)
Noveks_CFG.TextColor = {r = 255, g = 255, b = 255}      -- Default text color (White)
Noveks_CFG.AlertTextColor = {r = 255, g = 0, b = 0}     -- Alert text color (Red)

-- ================================================
-- Logging Settings
Noveks_CFG.LogSystem = true                             -- Enable or disable the logging system
Noveks_CFG.UseSteam = true                              -- Enable Steam integration (true/false)
Noveks_CFG.LogBotName = "Combatlog"                     -- Bot name for Discord logs

-- ================================================
-- Auto Disable Drawing Settings
Noveks_CFG.AutoDisableDrawing = true                    -- Automatically disable drawing after a set time
Noveks_CFG.AutoDisableDrawingTime = 15 * 1000           -- Duration: 15 seconds (15,000 ms)
```

---

## 📢 **How It Works:**

1. **Player Disconnect Detection:**  
   When a player leaves during combat, the script captures the event.

2. **Discord Logging:**  
   The disconnect event is logged to your specified Discord channel, providing details like player name and Steam ID (if enabled).

3. **In-Game Alerts:**  
   Custom messages alert admins or players in-game when someone disconnects unexpectedly, helping maintain transparency.

---

## 💬 **Support:**

Need assistance or have questions? Join our **Support Discord**:  
[Noveks Support Discord](https://discord.gg/8q8BnmgXq2)

---

### 📑 **License:**

This script is **not open-source**. Redistribution, resale, or unauthorized modification is strictly prohibited.
