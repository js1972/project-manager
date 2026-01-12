# Project Manager Gantt SPA

A single-file HTML app for managing projects with an interactive Gantt chart. All data is stored locally in the browser, and you can export a portable HTML file to share plans without a backend.

## Features
- Drag and resize tasks directly on the chart.
- Add milestones, reorder tasks, and color-code them.
- Dependencies with automatic scheduling constraints.
- Inline start/end date editing plus drag/resize.
- Undo/redo for common edits.
- Zoom levels (day/week/month).
- Search filter with compact view.
- Local persistence via `localStorage`.
- Export to a portable HTML file (Share button).
- Export tasks to CSV.

## Usage
1. Open `project_single_file_gantt_spa.html` in a browser.
2. Add tasks or milestones with the buttons in the header.
3. Edit dates directly in the Start/End fields or drag bars to move/resize.
4. Use the dependency dropdown to link tasks, and the zoom controls to change scale.
5. Click **Share** to download a self-contained HTML file you can email.

## Notes
- Dates are normalized to business days (Mon–Fri).
- When a task depends on another, it starts on the next business day after the predecessor ends.
- If you filter tasks, the Gantt view shows only matching tasks.
- Undo/redo stores up to 80 snapshots by default.
