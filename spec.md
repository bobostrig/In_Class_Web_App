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
- Reactions, shear, and moment from statics
- Deflection
- Bending stress fb = M/S, compared to the allowable stress
- Deflection compared to L/360

## Outputs
- The beam with its loads, and the three diagrams
- Pass or fail for bending and deflection

## Look and feel
Clean and professional, with an example beam loaded when it opens.

## Validation
20 ft simply supported W12x26 with 1 kip/ft: M = 50.0 kip-ft,
deflection 0.609 in.

## Out of scope
Continuous beams and buckling.