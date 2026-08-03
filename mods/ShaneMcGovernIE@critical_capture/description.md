# Critical Capture

Gen 5's critical capture for Gen 1: a thrown ball can whistle, pause and
shudder in mid-air, then shake once with far better odds. The chance scales
with your Pokedex completion, rescaled from the modern 600+ dex to Gen 1's
151 species.

- OPTIONS > CRIT CAPTURE cycles OFF / GEN 5 / GEN 6 (GEN 5 is the default).
- GEN 5 / GEN 6 use Bulbapedia's model: `c = floor(a * multiplier / 6)`, with
  `a` as the exact Gen 1 catch probability scaled to 0-255.
- Multiplier tiers rescaled to the 151-species dex in quarter steps.
- A critical capture shakes the ball exactly once; a normal throw is
  byte-for-byte vanilla. Master Balls never roll critical.

## Install

1. Download `critical_capture-<version>.zip` from the
   [releases page](https://github.com/ShaneMcGovernIE/critical_capture/releases).
2. In the launcher: MODS → **Import mod .zip**.

With `"github": "ShaneMcGovernIE/critical_capture"` set, the launcher's
**Update** and **Versions** buttons handle new releases from there.
