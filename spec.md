# Project Specification

Project requirements and behavior will be documented here.
# Beam Designer

## Purpose
This evaluates a single simply supported or cantilever beam under point and uniform loads. It calculates reactions, shear, moment, and deflection, displays the results, and checks bending stress and deflection against specified limits. It is an educational design aid, not a complete structural design or a substitute for professional review.

## Inputs
For each load: magnitude, direction, position, and— for a uniform load—its start and end points. Also say whether multiple loads are allowed.
Units for all values, not just span.
How users select a steel or lumber member, and where its material properties come from.
Whether design limits are entered by users or supplied by the app.

## Calculations
- Find support reactions using equilibrium: `ΣFy = 0` and `ΣM = 0`.
- Use standard beam equations for the selected supports and loads to calculate shear `V(x)`, bending moment `M(x)`, and deflection `v(x)`.
- Calculate maximum bending stress: `fb,max = |M|max / S`. Compare it with the selected member's allowable bending stress.
- Compare maximum deflection with `L/360`.
- Show the shear diagram, but do not check shear strength. Report pass/fail for bending and deflection only.

## Outputs
- The beam with its loads
- Separate graphs for shear, bending moment, and deflection, with labeled axes and units
- Support reaction values
- The maximum and minimum value on each graph and where each occurs
- Pass or fail for bending and deflection

## Look and feel
- Use a clean, professional engineering-notebook style.
- Use Georgia as the main serif font, with Cambria and Times New Roman as fallbacks. Use a simple sans-serif for graph labels and controls.
- Use a warm off-white background (`#F6F4EF`), white panels (`#FFFFFF`), charcoal text (`#23272F`), and navy headings (`#23395B`).
- Distinguish the shear, moment, and deflection graphs with teal (`#2A7886`), blue (`#0072B2`), and burnt orange (`#D55E00`).
- Show a faint BYU logo as a background watermark without reducing the readability of text or graphs.
- Open with an example beam loaded.

## Validation
For a 20 ft simply supported W12x26 with a downward 1 kip/ft uniform load over the full span:
- Reactions: 10 kip at each support
- Shear: maximum +10 kip just inside the left end and minimum -10 kip just inside the right end
- Moment: maximum 50.0 kip-ft at midspan and minimum 0 at the supports
- Deflection: maximum 0.609 in at midspan and minimum 0 at the supports

## Out of scope
Shear strength, bearing, connection design, load combinations, continuous beams, and buckling.