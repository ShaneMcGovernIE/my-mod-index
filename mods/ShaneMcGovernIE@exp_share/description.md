# Exp Share (Gen 1 / Gen 5+ styles)

Party-wide EXP from the OPTIONS menu, in Gen 1 Exp. All style, Gen 5+
style, or BALANCED / AVERAGE presets — with one "EXP is shared amongst
the party" line instead of a gain message per Pokemon. A SINGLE EXP SHARE
row can scope the shared EXP to one party slot instead of the whole bench.

## How it works

1. Open OPTIONS and cycle the new **EXP SHARE** row: **OFF / GEN 1 / GEN 5+ / BALANCED / AVERAGE**.
2. **GEN 1** (Exp. All): the fighters split half the exp; the whole party
   splits the other half — the vanilla Gen 1 split, bug included.
3. **GEN 5+**: the fighters keep the full exp; every alive bench Pokemon
   gets half a fighter's share.
4. **BALANCED** gates the bench on level: a bench Pokemon only gains exp
   while below the active fighter's level. **AVERAGE** uses the party's
   average level instead.
5. **SINGLE EXP SHARE** (right below EXP SHARE) cycles **ALL / 1 / 2 / 3 / 4 / 5 / 6**.
   ALL (the default) shares with the whole bench; a slot number shares
   only with the Pokemon in that party slot. A slot past your party size
   shares nothing at all.
6. Fighters keep their own "X gained N EXP. Points!" lines, then one
   "EXP is shared amongst the party" line, and every level-up, stat box
   and move learning still shows for each Pokemon that gained exp.
7. **OFF** restores vanilla behavior, including the vanilla Exp. All
   item's per-Pokemon messages.

Fainted Pokemon get no exp (Gen 5+ rules). The setting persists per save.

## Install

1. Download `exp_share-0.1.5.zip` from the
   [releases page](https://github.com/ShaneMcGovernIE/exp_share/releases).
2. In the launcher: MODS → **Import mod .zip**.

With `"github": "ShaneMcGovernIE/exp_share"` set, the launcher's
**Update** and **Versions** buttons handle new releases from there.
