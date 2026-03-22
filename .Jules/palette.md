## 2025-03-21 - Interactive Code Blocks for Better Developer Experience
**Learning:** Developers frequently interact with code snippets in documentation. Making the `code` block itself interactive and "clickable to copy" (with proper ARIA roles and keyboard support) reduces the precision required to trigger the copy action and improves the overall tactile feel of the interface.
**Action:** Always consider making code snippets focusable and clickable for copying, and provide clear visual cues (hover states, focus indicators) to signal interactivity.

## 2025-03-24 - Optimizing Search Inputs for Mobile and Accessibility
**Learning:** For search inputs, using `type="search"` along with `enterkeyhint="search"` provides a significantly better mobile experience by customizing the keyboard layout and action key. Additionally, adding `aria-keyshortcuts` informs assistive technology of available shortcuts, and `spellcheck="false"` reduces visual noise in search queries.
**Action:** For all search-like inputs, ensure semantic `type="search"`, set appropriate `enterkeyhint`, disable spellcheck if the input is for short queries, and communicate keyboard shortcuts via `aria-keyshortcuts`.
