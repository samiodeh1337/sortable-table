# Changelog

## 2.0.17 (2026-07-17)

### Bug Fixes

- Flush pending drop cleanup so a fast second drag (or a cancel) no longer races the ~200ms drop-snap animation timeout, which could leave the previous row hidden or corrupt drag state
- Skip the post-shift transform frame when the drag has already ended

### Chores

- Bump `styled-components`, `typescript-eslint`, and `vite` devDependencies

## 1.0.0 (2025-03-14)

### Features

- Drag-and-drop reordering for both rows and columns
- Smooth 60fps animations using direct DOM transforms
- Auto-scroll when dragging near container edges
- Drag range constraints (`columnDragRange`, `rowDragRange`)
- Custom placeholder rendering via `renderPlaceholder`
- `DragHandle` component for restricting drag to a grip element
- Virtual scrolling support (compatible with `@tanstack/react-virtual`)
- Full `className` and `style` prop support on every component
- Event delegation — single listener regardless of row count
- TypeScript support with full type definitions
