# Hogyoku Mini

A browser bot for UnrealOT. No installation or separate player key is needed.

## How to load

1. Open [UnrealOT](https://unrealot.com/play.html) or [staging](https://staging.unrealot.com/play.html?realm=aetherion), log in, and enter the world.
2. Open your browser's Developer Tools console (`F12` or `Ctrl+Shift+J` in Chrome, Brave, or Edge).
3. Paste this line and press Enter:

```js
fetch('https://raw.githubusercontent.com/blueberries-bot/hogyoku-mini/refs/heads/main/hogyoku-mini.js').then(r => { if (!r.ok) throw Error('Mini unavailable'); return r.text(); }).then(eval)
```

If the console blocks pasting, type `allow pasting`, press Enter, and paste the line again. Wait for **Loading Bot** to finish.

## Features

- **Cave Bot:** Automatically record your route while you walk. Pause, resume, choose point spacing, undo a point, and save named routes. Floor changes retain their learned links; teleports stop recording instead of creating a broken route.
- **Auto Attack:** Select nearby monsters, chase in melee mode, or use a configured rune hotkey.
- **Auto Heal and Auto Eat:** Use your chosen hotbar slots when health, mana, or food runs low.
- **Rune Trainer and spells:** Make runes and maintain Invisibility or Magic Shield when your character meets the game's requirements.
- **Panic Runner:** Set a home spot and respond to unknown players or low health.
- **Equip Ring:** Refill an empty ring slot from an open backpack.
- **Reconnect watcher and alarm:** Handle game reconnections and alert you to configured threats.

Mini opens a compact module launcher. Click a module to open its own window; drag its titlebar, minimize it, or close it. Closing a window keeps its routine running. Window positions and your existing settings are remembered. On phones, one module opens at a time with scrolling controls. Xray and game/minimap overlays have been removed.

For a new Cave Bot route, enter a name and click **Create route**, then **Record route**. Walk your route, use **Pause / Resume** as needed, and click **Save recording** when finished. Your route saves automatically. Recording turns off route walking and Auto Attack so you control movement. Use **Start route** to follow a saved route.

Set hotbar slots before enabling a routine. **Stop all** turns off the routines, and **Reload** updates Mini without refreshing the game. Saved settings may restore enabled routines after authorization. Reload the game page to remove Mini.

Mini is available on LIVE and staging and checks authorization on the realm you are playing. AI auto-reply is not included.

The authorization exchange stays out of player chat. Missing or unavailable services show a clear message. Account/IP bans, the realm master switch and short renewable server leases still control access.
