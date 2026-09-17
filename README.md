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

**Zoom** with the − / + control in the top left, the + and − keys, or ctrl + scroll, from 60% to 400%. Zooming in shows the individual threads of the weave.

**Wrap me** in the top right lifts the whole cloth off the screen. It zooms out a touch, its left edge gathers into a rope and leads the cloth around the screen like the snake game (south, east, north, then west along the top), and it folds itself back and forth onto a card, like a scarf folded on a shelf. The card shows the thread count and the sett, with a Share button (the system share sheet where there is one, otherwise the link is copied) and Save image, which downloads the card as a PNG. "Back to the loom" returns you to the editor.

Presets in the top right of the panel give you a starting point: the original Chennai swatch, an indigo check, and a red and navy "bleeding madras".

## Running

Open any `index.html` directly, or serve the folder:

```bash
python3 -m http.server 8000
```
