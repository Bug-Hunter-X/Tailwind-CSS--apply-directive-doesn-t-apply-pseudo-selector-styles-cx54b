# Tailwind CSS @apply Directive Issue with Pseudo-Selectors

This repository demonstrates a bug where Tailwind CSS's `@apply` directive fails to apply styles when a pseudo-selector (like `:hover` or `:focus`) is included in the utility class.  The issue is that only the base styles are applied, leaving the interactive styles missing.

## Reproduction

1. Clone this repository.
2. Open `bug.css` to see the buggy implementation.
3. Open `index.html` (if provided) to see the visual effect of the bug.
4. Open `bugSolution.css` to see a working solution.

## Solution

The solution involves avoiding the use of `@apply` with classes containing pseudo-selectors and instead directly applying the styles in your component styles.  This ensures all styles (including pseudo-selector styles) are applied correctly.