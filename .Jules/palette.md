## 2026-04-22 - OS-Aware Keyboard Shortcut Discoverability
**Learning:** Users on different operating systems expect different modifier keys (⌘ on Mac, Ctrl on Windows/Linux). Hardcoding "Ctrl" or "/" in the UI leads to confusion for Mac users. Dynamically updating shortcut hints and ARIA labels based on the user's platform significantly improves discoverability and makes the application feel like a native experience.
**Action:** Always detect the user's platform and programmatically update shortcut hints (e.g., labels, titles, and visual text) to use the correct modifier symbol (⌘ vs Ctrl).

## 2026-04-23 - Multi-word Search and Individual Highlighting
**Learning:** Single-string search is often too restrictive for users trying to find specific content. Implementing order-independent multi-word search allows users to combine multiple keywords (e.g., "pnpm ux") to filter results more effectively. Pairing this with individual word highlighting provides immediate visual confirmation of why each result matched the query, making the search interface feel more "intelligent" and helpful.
**Action:** Always split search queries into individual words and use an "AND" matching strategy (every word must match) combined with a grouped regex for granular highlighting.

## 2026-04-24 - Coordinated Search Error Feedback
**Learning:** In search interfaces, an empty state is more than just "no results." Synchronizing the color of the search icon and the focus ring (e.g., to red #dc2626) when no matches are found provides immediate, high-contrast visual feedback that the current query is invalid within the context. This coordinated feedback loop makes the interface feel more responsive and reduces the cognitive load for users identifying a failed search.
**Action:** Toggle a coordinated `.error` state on search components (icon and input focus ring) when matches are zero to provide clear, high-contrast feedback.

## 2026-04-25 - Intelligent Enter Navigation for Search
**Learning:** Enhancing search inputs to handle the 'Enter' key by programmatically triggering the primary action of the first visible result (e.g., copying a command or resetting the search) significantly streamlines the transition from query to action. This is especially impactful for keyboard-only users, as it reduces the number of Tab presses required to act on a filtered list.
**Action:** Always map the 'Enter' key in search inputs to the first available result's action to provide a faster, more intuitive user flow.
