# Hogyoku Mini for UnrealOT

This repository hosts the browser bundle for Hogyoku Mini. The bot runs inside the UnrealOT web client and requires an active game character. No separate player key is needed.

The current release is a **staging candidate**. Open [staging UnrealOT](https://staging.unrealot.com/play.html), log in, enter the world, then paste this into the browser's Developer Tools console:

```js
fetch('https://raw.githubusercontent.com/blueberries-bot/hogyoku-mini/refs/heads/main/hogyoku-mini.js').then(r => { if (!r.ok) throw Error('Mini unavailable'); return r.text(); }).then(eval)
```

The bundle asks the game server for a short-lived account authorization and renews it while running. All automation starts off. The owner can disable access through the server; editing this JavaScript does not grant server permissions. Delivered browser code can be inspected or copied, and minification is not a security boundary.

This candidate includes panic/PZ travel, cave waypoints and floor links, monster targeting, healing and supplies, rune and spell routines, ring equipment, X-ray awareness, and reconnect handling. AI auto-reply is deferred. Some gameplay paths still need acceptance on staging.

Reload the browser page to remove Mini. The panel's **Reload Bot** button fetches this GitHub file again after authorization. LIVE UnrealOT does not serve this candidate yet.
