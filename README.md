# Playing with Fabrics

Small experiments in simulating cloth in the browser. Each folder is one standalone page with no build step and no dependencies.

## Madras

`madras/index.html`: a woven madras plaid, drawn thread by thread on a 2D canvas.

Every vertical warp and horizontal weft thread is its own physics line rendered as a plain weave. Hover to part the threads, click to pluck them, and they spring back with tension and damping while a faint breeze keeps the cloth swaying at rest. Threads near the stitched pleat seams are stiffer.

The pattern lives in two arrays at the top of the script: `WEFT` (horizontal bands, top to bottom, as height and colour) and `WARP` (vertical stripes across one repeat). Edit those to weave a different cloth.

## Running

Open any `index.html` directly, or serve the folder:

```bash
python3 -m http.server 8000
```
