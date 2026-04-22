## 2026-04-22 - OS-Aware Keyboard Shortcut Discoverability
**Learning:** Users on different operating systems expect different modifier keys (⌘ on Mac, Ctrl on Windows/Linux). Hardcoding "Ctrl" or "/" in the UI leads to confusion for Mac users. Dynamically updating shortcut hints and ARIA labels based on the user's platform significantly improves discoverability and makes the application feel like a native experience.
**Action:** Always detect the user's platform and programmatically update shortcut hints (e.g., labels, titles, and visual text) to use the correct modifier symbol (⌘ vs Ctrl).
