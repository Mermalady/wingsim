# Cosplay Wing Simulator

Design, simulate, and build costume wings with 4-bar linkages.

**Live app:** https://mermalady.github.io/wingsim/

A 2D, browser-based simulator for articulated bird-style costume wings. Adjust the bones, joints and linkages, watch the wing fold and unfold, then export true-scale cut templates for building.

## What it does

- **Simulates a real folding mechanism.** One input (the shoulder swing) drives the whole wing through linked 4-bar loops:
  - the **coracoid** and **clavicle** bars pivot on a backplate and form the humerus;
  - the clavicle bar pins to the **ulna**, which folds the elbow;
  - the **radius** drives the **hand**, which folds the wrist.

  The wing goes from fully open to fully closed.
- **Handle:** a bar that pivots freely at the elbow or at the end of the ulna (wrist). Drag the grip in the view to work the wing by hand.
- **Lift hinge (optional):** both shoulder pivots ride on a lift plate, so the whole wing can be raised above the head.
- **Feathers:**
  - primaries, secondaries with a scalloped trailing edge, and tertials;
  - optional primary coverts (on the radius) and marginal coverts (on the clavicle bar).

  Feather mount holes are placed automatically so they stay clear of every joint bolt and of bars that cross over.
- **Scale check:** show both wings on an adjustable human figure (default 5′8″) to judge span and backplate height.
- **Bird presets:** raptor, corvid, swan and swift proportions. You can also set a target open wingspan and scale everything at once.
- **Inches or centimeters.**

## Using it

1. Open the [live app](https://mermalady.github.io/wingsim/), or download `index.html` and open it in any browser. It works offline and needs no install.
2. Pick a preset, then adjust these panel sections:
   - **Overall size**
   - **Bone dimensions**
   - **Kinematics** (pin positions, wrist pin, radius–ulna spacing)
   - **Fold range**
   - **Handle**
   - **Mounts** (backplate and lift hinge)
   - **Feathers**
   - **Figure**
   
   Use the **View** bar above the drawing to show or hide feathers, the handle, motion paths, the figure, and part and pin labels.
3. Press **Play**, or drag the ringed joints and the handle grip, to check the motion.
4. Go to **Build & export** and set:
   - the width of each bar, or an overall width;
   - widened bases on the clavicle and coracoid bars;
   - pivot and feather hole sizes.
5. Click **Export part templates (SVG)**.

Settings save automatically in your browser. **Undo** (or ⌘/Ctrl+Z) steps back one change at a time; **Reset dimensions** goes back to the preset while keeping your view options.

## Templates

Templates are SVG files at true scale, in millimetres, ready for a laser cutter, CNC router or printing at 100%. Line colours:

| Colour | Meaning |
|---|---|
| Red | Cut |
| Blue dashed | Centreline |
| Black | Engrave / mark |

Cut two of every part, and flip one set for the left wing.

## Build notes

- Put hard stops at the fold-range limits you set. The linkage gets less efficient near full open and full fold.
- For pivots, use shoulder bolts or bolt-and-sleeve joints that match the pivot hole size.
- Each feather pivots on its quill hole, so it swings naturally as the wing folds.

## Project files

| File | Purpose |
|---|---|
| `index.html` | The whole app: HTML, CSS and JavaScript in one file |
| `README.md` | This file |
| `LICENSE` | MIT |

## License

MIT © 2026 Meredith SK
