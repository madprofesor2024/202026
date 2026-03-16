## 2025-03-13 - [Color Contrast in Success States]
**Learning:** Success states (e.g., green backgrounds) must maintain a 4.5:1 contrast ratio for normal text. White text on light green often fails.
**Action:** Use dark green backgrounds (e.g., Tailwind's `emerald-900` / `#065f46`) for success states when using white text.

## 2025-03-16 - [Stable Layout for Success States]
**Learning:** Changing button text length (e.g., "Copy" to "Copied!") can cause layout shifts if the button doesn't have a stable `min-width`.
**Action:** Define a stable `min-width` on buttons that change text content to prevent jumping.

## 2025-03-16 - [Tactile Feedback]
**Learning:** Adding a small scale down effect on `:active` state makes buttons feel more "clickable" and responsive.
**Action:** Use `transform: scale(0.96)` for `:active` states on buttons.
