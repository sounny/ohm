# Ohm's Law Calculator

An interactive single-page tool for exploring the relationships between voltage (V), current (I), resistance (R), and power (P). Enter any two values to instantly compute the remaining quantities, see the formulas that were used, and watch the accompanying SVG circuit diagram update in real time.

## Features

- **Responsive layout** that keeps the calculator and circuit diagram side-by-side on larger screens and stacks them on small displays.
- **Declarative calculation engine** that chooses the correct Ohm's and Joule's Law relationships based on the last two values you edited.
- **Live SVG updates** so the circuit illustration always reflects the latest computed values.
- **Inline hints and styling cues** that distinguish between user-provided and auto-calculated inputs.

## Getting Started

1. Open `index.html` in any modern web browser.
2. Provide values for any two of the four electrical properties.
3. Review the computed results, highlighted formulas, and updated circuit diagram.

No build step or external dependencies are required; everything runs entirely in the browser.

## Project Structure

- `index.html` – Contains the HTML, CSS, and JavaScript for the calculator UI and logic.
- `README.md` – Project overview, usage instructions, and architectural notes (this file).
- `AGENTS.md` – Working-memory notes for autonomous agents collaborating on the project.

## Development Notes

- Calculations are centralized in `CALCULATION_RULES` within the script, making it straightforward to extend the tool with additional derived quantities.
- The helper functions at the bottom of `index.html` keep DOM updates organized and well-commented for easier maintenance.
