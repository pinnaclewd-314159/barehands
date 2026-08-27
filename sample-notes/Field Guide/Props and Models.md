# Props and Models

The `media/` folder is the **airlock**: the only place the board will ever stage a file from. That's a safety feature: your AI can show what you deliberately put there, and nothing else on your disk.

## The folders are the render law

- `media/misc/`: images. Stage as framed glass cards.
- `media/fx/`: transparent props. Render NAKED (no frame, no chrome), a floating object. Transparent PNGs float; alpha WebM videos loop silently (a fireball you can throw).
- `media/models/`: 3D models (.glb / .gltf / .stl / .3mf). GLB/glTF and 3MF render REAL: full textures (or, for 3MF, whatever color it carries) plus environment lighting. STL carries no color or texture data at all — that's just how the format works — so it always renders as the hologram wire, wherever you put it.
- `media/holo/`: the same model files, but anything in here renders as the **hologram**: a translucent blue-glass wireframe with a scan beam. Same file, different folder, different reality.

Drop a file in, press **R** (or tap the ring → Props), and it's on the shelf.

## Where to get models

GLB/glTF and 3MF work for full-color models. Free sources with proper licenses: Sketchfab (filter by downloadable + license), Poly Haven, or generate your own with AI tools that export GLB. A model made of separate named parts gets the full **explode** treatment; single fused meshes stage fine but can't be pulled apart.

3D-printer files (STL, and 3MF with its color intact) drop straight into `media/models/` too — handy for previewing a print before you send it to the printer.
