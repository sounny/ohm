# Agent Working Memory

This file is a living log for autonomous agents collaborating on the Ohm's Law calculator. Append new entries rather than rewriting history so future sessions can see the full lineage of changes.

## Session Log — v1
- Established this working-memory file to capture reasoning for future contributors.
- Refactored the calculator script to use a declarative `CALCULATION_RULES` map, reducing branching complexity.
- Added inline documentation that explains how the calculator chooses formulas and formats results.
- Authored a project README summarizing purpose, usage, and structure.

## Implementation Notes
- Calculation rules are keyed by combining the relevant variable symbols (e.g., `IR`, `PV`). When adding new relationships, keep keys alphabetized to match the sorter in `calculateAndDisplay`.
- Helper utilities (`getInputValues`, `updateUI`, `updateStylesAndDiagram`, `formatNumber`) are intentionally small and single-purpose. Favor extending them over reintroducing ad-hoc DOM updates.

## Guidance for Future Agents
- When you make changes, append a new section under "Session Log" with a short summary of what changed and why.
- Preserve the declarative rule structure in the script; it keeps maintenance approachable and reduces regression risk.
- If you introduce build tooling or additional assets, update the README and note the change here so future agents know the expected workflow.

## Session Log — v2
- Added a new "Learning Coach" panel that provides a guided, step-by-step walkthrough of each calculation so users can understand the reasoning, not just the result.
- Extended the calculator logic with a teaching narrative builder that summarizes known values, shows each formula substitution, and includes a quick power sanity check.
- Kept the existing declarative rule system intact while enhancing the UI to make the tool more instructional for learners.
