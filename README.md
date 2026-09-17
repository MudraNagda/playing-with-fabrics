# Playing with Fabrics

Small experiments in simulating cloth in the browser. Each folder is one standalone page with no build step and no dependencies.

## Madras

`madras/index.html`: a woven madras plaid, drawn thread by thread on a 2D canvas.

Every vertical warp and horizontal weft thread is its own physics line rendered as a plain weave. Hover to part the threads, click to pluck them, and they spring back with tension and damping while a faint breeze keeps the cloth swaying at rest. Threads near the stitched pleat seams are stiffer.

**Design your own.** The panel at the bottom is the sett: the sequence of colours and thread counts that a weaver winds onto the warp beam. The same sett runs across and down, which is what makes a madras check.

- Tap a stripe, then tap a skein to dye it.
- Drag a stripe's right edge to change its thread count. Shift + arrow keys do the same from the keyboard.
- `+ stripe` duplicates the selected stripe; `remove` deletes it.
- `Share link` copies a URL with the whole sett encoded in it, so nothing is stored anywhere.

Presets in the top right give you a starting point: the original Chennai swatch, an indigo check, and a red and navy "bleeding madras".

## Running

Open any `index.html` directly, or serve the folder:

```bash
python3 -m http.server 8000
```
