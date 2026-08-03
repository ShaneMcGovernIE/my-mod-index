# Mods Hotkeys

Scans every enabled mod's Lua sources for the hotkeys they listen for —
wrapped `keypressed` checks (`key == "q"`), wrapped `gamepadpressed`
checks (`button == "leftshoulder"`), held pad combos (`held.back and
held.leftshoulder`), GB-button combos (`wasPressed("select") and
wasPressed("a")`) and configurable GB-button triggers (DexNav's
`DEXNAV_BUTTONS`) — and lists each one in **OPTIONS → MODS HOTKEYS**.

No opt-in needed: the detection is static, so it works with any mod.

## Rebinding

- **A** on a row arms a capture: press your new combo — any mix of
  keyboard keys and pad buttons, up to 4 pieces — and release to set.
  `SELECT×A`, `TAB×LB`, `T×Y` all work.
- **SELECT** resets one row, **START** resets everything.
- Rebinds persist in options.lua, so they survive NEW GAME, CONTINUE
  and quitting.

When your new trigger fires, the mod's *original* trigger is re-emitted
through the input chain — the source mod is never modified, and the
original trigger keeps working as an extra way in.

Engine hotkeys (F1/F2/F10, the 2/3/4/5 display cycles, -/= zoom) can't be
bound, so a combo can never quicksave or cycle colours by surprise.

## Install

1. Download `mods_hotkeys-0.1.5.zip` from the
   [releases page](https://github.com/ShaneMcGovernIE/mods_hotkeys/releases).
2. In the launcher: MODS → **Import mod .zip**.

With `"github": "ShaneMcGovernIE/mods_hotkeys"` set, the launcher's **Update**
and **Versions** buttons handle new releases from there.
