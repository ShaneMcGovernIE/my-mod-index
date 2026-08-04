# QoL Toggles

Seventeen quality-of-life switches in OPTIONS → **QOL TOGGLES**, each
persisted with your preferences (they stay on across restarts and save
files).

## The switches

1. **POISON SAVE** — a poisoned party member that would faint from
   out-of-battle poison damage survives at 1 HP and the poison subsides:
   *"X's poison has subsided!"*
2. **FULL HEAL CATCH** — every captured Pokémon is fully healed (HP,
   status, and all PP), whether it joins the party or goes to a PC box.
3. **INFINITE REPEL** — no wild encounters while walking through grass,
   surfing, or in caves.  Fishing is unaffected, like the vanilla Repel
   item.
4. **FIELD MOVES ALL** — any Pokémon that can learn a field move
   (level-up or TM/HM) can use it out of battle even without knowing it:
   a Pidgey that never learned FLY can still FLY, a Clefable without
   TELEPORT can still TELEPORT.  Badge gates and context rules still
   apply.
5. **BADGELESS MOVES** — FLY, SURF, CUT, STRENGTH and FLASH work without
   their badges.  Pairs with FIELD MOVES ALL for a no-badge run.
6. **HM ITEM REQUIRED** — the FIELD MOVES ALL extras for HM moves only
   appear once you actually hold the HM item (no CUT on the Cascade
   Badge alone).
7. **UNLIMITED TMs** — TMs teach their move without breaking.
8. **FORGETTABLE HMs** — HM moves can be forgotten when a Pokémon learns
   a new move.
9. **ALWAYS CATCH** — every ball catches, Master Ball style (the ball is
   still consumed).
10. **PERFECT DVS** — caught Pokémon get 15s across the board with stats
    recomputed to match.
11. **EXP x2** — double battle EXP; the "gained N EXP" text shows the
    doubled amount.
12. **CATCH GIVES EXP** — capturing a wild Pokémon pays out the same EXP
    its defeat would, split among the mons that fought.
13. **INSTANT FLEE** — wild battles always escape on the first try.
14. **REMEMBER CURSOR** — the battle FIGHT/BAG/PKMN/RUN cursor stays
    where you left it across turns.
15. **HEAL ON MAP CHANGE** — every map transition fully heals the party:
    HP, status, and all PP.
16. **QUICK S.S. ANNE** — the Vermilion dock sailor prompts for your
    ticket once; after that you walk straight onto the ship.
17. **LAST ITEM (M)** — in battle, press M to use the last item you used
    from the bag: balls throw at the foe, healing opens the party screen
    to pick the mon, targetless battle items work as usual.  M is
    rebindable from the Mods Hotkeys submenu.

## Notes

- POISON SAVE, FULL HEAL CATCH, FIELD MOVES ALL, HM ITEM REQUIRED,
  UNLIMITED TMs, FORGETTABLE HMs and REMEMBER CURSOR ship ON; the rest
  ship OFF.  Each flip is saved immediately to options.lua.
- START on a controller (or P on the keyboard) on any toggle row opens an
  in-depth help popup explaining what that toggle does.
