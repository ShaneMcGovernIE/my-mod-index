# my-mod-index

A personal mod index for the [Gen 1 recomp engine](https://github.com/DramaticShape/pokemon-gen1-recomp-project),
modeled on the [official community index](https://github.com/bryanthaboi/gen1recomp-mod-index).
One folder per mod, holding metadata only — the mods live in their own
repositories; this index says where they are and what they need.

- **Consume it in the launcher:** MODS → **Find mods** → paste
  `ShaneMcGovernIE/my-mod-index` (or the Pages URL). The feed is
  published to Pages on every push and refreshed nightly.
- **Feed:** `data/index.json` on
  [GitHub Pages](https://shanemcgovernie.github.io/my-mod-index/data/index.json).

## Layout

```
mods/
  <Author>@<mod id>/
    meta.json          required — the entry itself
    description.md     required — long form, markdown
    thumbnail.png      optional — or thumbnail.jpg, 2 MB max
```

The id half is the mod's `manifest.json` `id`. Nothing else may live in
the folder. Entries validate against
[`schema/mod.schema.json`](schema/mod.schema.json).

## Adding a mod

1. Copy `examples/YourName@example_mod/` to `mods/<Author>@<id>/`.
2. Fill in `meta.json` (mostly a copy of the mod's manifest) and
   `description.md`.
3. Check it: `node scripts/validate.mjs`.
4. Push — the workflow builds `site/data/index.json` and deploys Pages.

Version bumps need no pull request: `--releases` re-reads each repo's
GitHub Releases nightly (same asset-picking rule as the launcher's
`ModUpdate.lua`), so tagging a release in your mod repo updates this
index within a day.

## Working on it

```sh
node scripts/validate.mjs                 # every entry (offline, instant)
node scripts/validate.mjs mods/You@my_mod # one entry
node scripts/build-index.mjs              # write site/data/index.json
node scripts/build-index.mjs --releases   # …and re-read GitHub Releases
```

No dependencies — a plain `node` is the whole toolchain.

## Credit

Validation and build scripts adapted from
[bryanthaboi/gen1recomp-mod-index](https://github.com/bryanthaboi/gen1recomp-mod-index).
Listing is not vetting: read a mod's source before you enable it.
