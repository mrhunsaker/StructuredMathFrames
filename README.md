# Structured Math Frames (UEB, Nemeth, and Print)

3D-printable tactile math frames, number/operation tiles, storage carriers, and worksheet generator scripts designed for blind and visually impaired students—supporting **Unified English Braille (UEB)**, **Nemeth Braille**, and **large/standard print**.

> **Project Overview:** [TVI Resources — Structured Math Frames for UEB, Nemeth, and Print](https://tviresources.github.io/blog/structured-math-frames/)

---

## Why This Project Exists

Sighted students rely on graph paper or lined columns as an immediate visual guide to align digits vertically during multi-digit arithmetic. Students using a Perkins braillewriter, however, must simultaneously manage mathematical reasoning and tactile layout—keeping place-value columns aligned while composing braille.

Multi-digit multiplication compounds this cognitive load: multiplying by tens or hundreds digits requires placing trailing zeros on partial products before summing, which can easily interrupt problem-solving and introduce alignment errors. **Structured Math Frames** provide a physical, graph-paper-like scaffold so learners can focus on math concepts and computation rather than layout mechanics.

---

## Key Benefits

- **Lower formatting burden:** Offloads vertical column alignment to physical structure so students focus on math.
- **Concrete place-value support:** Dedicated columns for ones, tens, hundreds, and thousands (plus specialized layouts such as time-keeping) make place value tactile and intuitive.
- **Independent practice & self-checking:** Tactile boundaries help students align numbers accurately and verify their own work.
- **Multi-notation flexibility:** Available in **UEB**, **Nemeth**, and **print** versions to match each student's curriculum and visual/tactile needs.

---

## Included Components & Features

- **Operation-Specific Frames:**
  - **Addition & Subtraction:** Place-value columns, operation sign slot, and a horizontal divider separating problem rows from the answer line.
  - **Multiplication:** Place-value columns, operation sign slot, extra rows for intermediate partial products, and a final answer line to support trailing zeros/place alignment.
  - **Division:** Tactile long-division layout with space for the divisor, dividend, partial quotients, and final answer.
  - **Additional / Specialized Layouts:** Such as a time-keeping frame (`TimeKeepingFrame`).
- **Tiles & Storage:**
  - Number tiles (`0–9`), operation tiles (`+`, `-`, `×`, `÷`, etc.), and blank filler tiles.
  - A small lidded carrier / storage bay for keeping frames and tiles organized.
- **Notation Variants (`exported_stls/`):**
  - `*_UEB.stl` — Unified English Braille
  - `*_Nemeth.stl` — Nemeth Braille
  - `*_print.stl` — Print-friendly versions
  - Designed for optional two-color filament swaps to increase visual/tactile contrast.
- **Custom Worksheet Generator Scripts:**
  - Scripts to generate custom worksheets (varying sizes, number ranges, and UEB/Nemeth/print options) via PowerShell on Windows or Bash/Zsh on macOS and Linux.
- **Parametric OpenSCAD Source (`structured_math.scad`):**
  - Editable source file configured for the OpenSCAD Customizer panel.

---

## Getting Started

### 1. Quick Print (Pre-Generated STL Files)

1. Download or clone the repository (`https://github.com/mrhunsaker/StructuredMathFrames`).
2. Navigate to the `exported_stls` folder and pick the files matching your target notation:
   - `*_UEB.stl`
   - `*_Nemeth.stl`
   - `*_print.stl`
3. Slice and print in your preferred slicer (e.g., BambuStudio, OrcaSlicer, PrusaSlicer).

#### 3D Printing Notes
- **Braille orientation & touch:** Orienting/printing with braille raised appropriately to the side helps dots read cleanly without feeling overly sharp to the touch.
- **Filament & slicer settings:** Tested on a Bambu P1S in BambuStudio using default print parameters with budget PLA (such as Generic PLA, Filastruder PLA, or Elegoo PLA). Start with default settings and tune for your specific printer and filament.

### 2. Generate Custom Worksheets

1. Run the provided **PowerShell** script on Windows, or the **Bash / Zsh** script on macOS or Linux.
2. Follow the prompts to configure worksheet size, number ranges, and notation options (UEB, Nemeth, or print).

---

## Customizing with OpenSCAD

To adjust dimensions, column spacing, tile tolerances, or braille depth:

1. Install [OpenSCAD](https://openscad.org/) and open `structured_math.scad`.
2. Open the **Customizer** panel on the right side of the OpenSCAD window.
3. Adjust parameters (dimensions, spacing, braille depth, etc.).
4. Press **F6** to render and **F7** to export the updated `.stl` file.
5. Slice and print the exported STL.

---

## Classroom Tips

- **Introduce one operation at a time:** Build comfort with addition alignment before moving to subtraction, multiplication, or division.
- **Pair with verbal narration:** Have students name place-value columns (`ones`, `tens`, `hundreds`) aloud as they place tiles.
- **Use for verification:** Have students rebuild paper-and-pencil or braillewriter solutions on the frame to check alignment and catch errors.
- **Fade scaffolding gradually:** Transition fluent students to graph paper or unlined/blank media as independence grows.

---

## Contributing & Feedback

Contributions, custom variations, lesson plans, and classroom guides are welcome:

- **Issues & Pull Requests:** [mrhunsaker/StructuredMathFrames](https://github.com/mrhunsaker/StructuredMathFrames)
- **Blog & Notes:** [TVI Resources](https://tviresources.github.io/blog/structured-math-frames/)

---

## Author

Created by **Michael Ryan Hunsaker, M.Ed., Ph.D.** — Behavioral neuroscientist and Teacher of Students with Visual Impairments (TVI). More resources at [TVI Resources](https://tviresources.github.io/).
