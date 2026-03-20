## 2025-03-20 - Standard Search UX and Accessibility
**Learning:** Modern search inputs benefit significantly from smooth transitions (using `opacity` instead of `display: none`) and standard keyboard interactions. Supporting the `Escape` key to clear content first, then blur, is a crucial UX pattern that power users expect.
**Action:** When implementing or refining search components, ensure smooth visual state transitions and include `Escape` key handlers for clearing/blurring.
