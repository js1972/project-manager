# Project Manager Gantt SPA

A single-file HTML app for managing projects with an interactive Gantt chart. All data is stored locally in the browser, and you can export a portable HTML file to share plans without a backend.

## Features
- Drag and resize tasks directly on the chart.
- Add milestones, reorder tasks, and color-code them.
- Dependencies with automatic scheduling constraints.
- Search filter with compact view.
- Local persistence via `localStorage`.
- Export to a portable HTML file (Share button).

## Usage
1. Open `project_single_file_gantt_spa.html` in a browser.
2. Add tasks or milestones with the buttons in the header.
3. Drag bars to move or resize; use the dependency dropdown to link tasks.
4. Click **Share** to download a self-contained HTML file you can email.

## Notes
- Dates are normalized to business days (Mon–Fri).
- When a task depends on another, it starts on the next business day after the predecessor ends.
- If you filter tasks, the Gantt view shows only matching tasks.
