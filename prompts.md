# Prompt Log

- Asked to set up the project folder layout for a single-file web app. Created the requested root-level project files, numbered folders, folder READMEs, and layout guidance in `AGENTS.md`. Worked: the requested structure is in place; no app behavior was built.
- Clarified that the numbered directories should not contain README files. Removed the four READMEs and added empty `.gitkeep` markers so the directories remain in Git. Worked: `00_planning`, `01_data`, `02_validation`, and `03_output` are folders without README files.
- Asked why the folders contain `.gitkeep` files. Explained that Git does not track empty directories, so these placeholders make the folders persist in the repository. No project structure changes were made.
- Asked for a high-level summary and whole-spec review. Read `spec.md`; no code or app behavior was built and the spec itself was not changed.
- Asked for suggestions on the Purpose section. Provided draft wording and scope guidance; did not change the spec.
- Asked for feedback on Inputs. Noted which input definitions are still underspecified and suggested categories to clarify; did not change the spec.
- Asked for feedback on the remaining spec sections. Reviewed calculations, outputs, look and feel, validation, and out-of-scope coverage; did not change the spec.
- Asked what changes to make to the other sections. Proposed requirement-focused wording and scope clarifications; did not change the spec.
- Asked for recommendations for the Calculations section. Suggested clarifying assumptions, material-specific criteria, deflection basis, reported extrema, and checks not performed; did not change the spec.
- Asked why the suggested steel/lumber and load details matter. Explained they determine calculation inputs and pass/fail criteria, while distinguishing essential scope decisions from implementation-level detail; did not change the spec.
- Said the spec should not be so complex. Recommended a simpler educational-app scope and a short calculations statement; did not change the spec.
- Asked for suggestions for a simple calculations version. Recommended limiting checks to basic beam response, bending, and deflection with clear exclusions; did not change the spec.
- Requested formulas for all supported load cases in Calculations and selected the general case. Added load/reaction, shear, moment, deflection, stress, and deflection-limit equations for multiple point loads and partial/full uniform loads on both support types.
- Said the expanded formulas were too complex and long. Simplified the Calculations section to equilibrium, standard beam equations, bending stress, and the deflection limit.
- Asked for feedback on Outputs after simplifying Calculations. Recommended showing reactions, labeled diagrams, and the two check results with their limits; did not change the spec.
- Clarified that each result should have its own graph. Updated Outputs to specify separate shear, bending-moment, and deflection graphs.
- Approved the proposed simple Calculations wording and asked to apply it. Updated only the Calculations section in `spec.md`; no code or app behavior was built.
- Asked for suggestions for the Outputs section. Recommended beam/load view, reactions, labeled diagrams, and concise bending/deflection results; did not change the spec.
