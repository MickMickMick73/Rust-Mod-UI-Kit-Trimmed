# Rust-Mod-UI-Kit-Trimmed

Drop-in **alpha-trimmed** replacements for [`MickMickMick73/Rust-Mod-UI-Kit`](https://github.com/MickMickMick73/Rust-Mod-UI-Kit).

Same **filenames**, same **folders**, same **canvas sizes** — copy over the originals.

## What was wrong

Transparent pixels still carried colour (white / yellow / fringe RGB). In Oxide CUI that shows as a yellow or dirty halo. Some icons also had leftover specks from the matte (gear shard, lock triangle, map/skull hairlines, rifle round).

## What we did

- Zero RGB on fully transparent pixels (stops the yellow matte)
- Harden fringe alpha
- Delete tiny disconnected junk islands
- Did **not** change seamless `textures/`

See `TRIM-REPORT.md` for the per-file list.

## Swap

Copy `sprites/` from this repo over the matching paths in the original pack.
