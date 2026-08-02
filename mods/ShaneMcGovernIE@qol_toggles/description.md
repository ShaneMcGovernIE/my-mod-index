# QoL Toggles

Four quality-of-life switches in OPTIONS → **USEFUL TOGGLES**, each
persisted with your preferences (they stay on across restarts and save
files).

## The switches

1. **POISON SAVE** — a poisoned party member at 1 HP no longer faints
   from out-of-battle poison damage; the poison subsides with *"X's
   poison has subsided!"*
2. **FULL HEAL CATCH** — every captured Pokémon is fully healed (HP,
   status, and all PP), whether it joins the party or goes to a PC box.
3. **INFINITE REPEL** — no wild encounters while walking through grass,
   surfing, or in caves.  Fishing is unaffected, like the vanilla Repel
   item.
4. **FIELD MOVES ALL** — any Pokémon that can learn a field move
   (level-up or TM/HM) can use it out of battle even without knowing it:
   a Pidgey that never learned FLY can still FLY, a Clefable without
   TELEPORT can still TELEPORT.  Badge gates and context rules still
   apply — no FLY without the Thunder Badge, no SURF without the Soul
   Badge, DIG only on its cave tilesets.

## Notes

- Toggles default to OFF; each flip is saved immediately to
  options.lua, so toggles set from the title screen survive starting or
  continuing a game.
- FIELD MOVES ALL never touches battle: it only adds the out-of-battle
  party-menu options.
