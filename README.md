# Hogyoku Mini

A browser bot for UnrealOT. No installation or separate player key is needed.

## How to load

1. Open [UnrealOT staging](https://staging.unrealot.com/play.html), log in, and enter the world.
2. Open your browser's Developer Tools console (`F12` or `Ctrl+Shift+J` in Chrome, Brave, or Edge).
3. Paste this line and press Enter:

```js
fetch('https://raw.githubusercontent.com/blueberries-bot/hogyoku-mini/refs/heads/main/hogyoku-mini.js').then(r => { if (!r.ok) throw Error('Mini unavailable'); return r.text(); }).then(eval)
```

If the console blocks pasting, type `allow pasting`, press Enter, and paste the line again. Wait for **Loading Bot** to finish.

## Features

- **Cave Bot:** Save route presets, record waypoints, loop routes, and use learned floor transitions.
- **Auto Attack:** Select nearby monsters, chase in melee mode, or use a configured rune hotkey.
- **Auto Heal and Auto Eat:** Use your chosen hotbar slots when health, mana, or food runs low.
- **Rune Trainer and spells:** Make runes and maintain Invisibility or Magic Shield when your character meets the game's requirements.
- **Panic Runner:** Set a home spot and respond to unknown players or low health.
- **Equip Ring:** Refill an empty ring slot from an open backpack.
- **X-ray:** Show loaded creatures and floor markers around your character.
- **Reconnect watcher and alarm:** Handle game reconnections and alert you to configured threats.

All routines start off. Set your hotbar slots and route before enabling the corresponding routine. Drag the panel by its titlebar on desktop, or press **−** to minimize it. **Reload Bot** refreshes the bot without refreshing the game page. Reload the game page to remove it.

This build is currently for UnrealOT **staging**. AI auto-reply is not included.
