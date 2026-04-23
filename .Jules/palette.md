## 2026-04-22 - OS-Aware Keyboard Shortcut Discoverability
**Learning:** Users on different operating systems expect different modifier keys (⌘ on Mac, Ctrl on Windows/Linux). Hardcoding "Ctrl" or "/" in the UI leads to confusion for Mac users. Dynamically updating shortcut hints and ARIA labels based on the user's platform significantly improves discoverability and makes the application feel like a native experience.
**Action:** Always detect the user's platform and programmatically update shortcut hints (e.g., labels, titles, and visual text) to use the correct modifier symbol (⌘ vs Ctrl).

## 2026-04-23 - Multi-word Search and Individual Highlighting
**Learning:** Single-string search is often too restrictive for users trying to find specific content. Implementing order-independent multi-word search allows users to combine multiple keywords (e.g., "pnpm ux") to filter results more effectively. Pairing this with individual word highlighting provides immediate visual confirmation of why each result matched the query, making the search interface feel more "intelligent" and helpful.
**Action:** Always split search queries into individual words and use an "AND" matching strategy (every word must match) combined with a grouped regex for granular highlighting.
