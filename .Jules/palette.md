## 2025-03-21 - Interactive Code Blocks for Better Developer Experience
**Learning:** Developers frequently interact with code snippets in documentation. Making the `code` block itself interactive and "clickable to copy" (with proper ARIA roles and keyboard support) reduces the precision required to trigger the copy action and improves the overall tactile feel of the interface.
**Action:** Always consider making code snippets focusable and clickable for copying, and provide clear visual cues (hover states, focus indicators) to signal interactivity.

## 2025-03-24 - Optimizing Search Inputs for Mobile and Accessibility
**Learning:** For search inputs, using `type="search"` along with `enterkeyhint="search"` provides a significantly better mobile experience by customizing the keyboard layout and action key. Additionally, adding `aria-keyshortcuts` informs assistive technology of available shortcuts, and `spellcheck="false"` reduces visual noise in search queries.
**Action:** For all search-like inputs, ensure semantic `type="search"`, set appropriate `enterkeyhint`, disable spellcheck if the input is for short queries, and communicate keyboard shortcuts via `aria-keyshortcuts`.

## 2025-03-25 - Search UX: Accessible Clear Buttons and Universal Shortcuts
**Learning:** Using `opacity: 0` to hide a "Clear search" button is insufficient for accessibility as it remains in the tab order. Using `visibility: hidden` correctly removes it from the accessibility tree and prevents focus when inactive, while still allowing for smooth CSS transitions. Additionally, supporting universal shortcuts like `Ctrl+K`/`Cmd+K` provides a familiar and efficient experience for power users.
**Action:** When hiding interactive elements visually, use `visibility: hidden` to also hide them from assistive technology and the keyboard tab order. Implement `Ctrl+K`/`Cmd+K` as a standard secondary shortcut for search inputs.
