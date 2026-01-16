# Project Manager Gantt SPA

A single-file HTML app for managing projects with an interactive Gantt chart. All data is stored locally in the browser, and you can export a portable HTML file to share plans without a backend.

## Features
- Drag and resize tasks directly on the chart.
- Add milestones, reorder tasks, and color-code them.
- Dependencies with automatic scheduling constraints.
- Dependency linking via drag handles.
- Critical path highlighting with a toggle.
- Inline start/end date editing plus drag/resize.
- Task status and % complete with progress overlays.
- Assignee field for tasks.
- Undo/redo for common edits.
- Zoom levels (day/week/month).
- Search filter with compact view.
- Project and task notes in a drawer.
- Local persistence via `localStorage`.
- Export to a portable HTML file (Share button).
- Export tasks to CSV (includes `assignee`, `status`, `progress`, `projectTitle`, `projectNotes`, and per-task `notes`).
- Import tasks from CSV (overwrites after confirmation).

## Usage
1. Open `project_single_file_gantt_spa.html` in a browser.
2. Add tasks or milestones with the buttons in the header.
3. Edit dates directly in the Start/End fields or drag bars to move/resize.
4. Use the dependency dropdown or drag the dot on a task bar to link tasks, and the zoom controls to change scale.
5. Toggle **Critical Path** to highlight the longest dependency chain.
6. Open **Notes** to edit project notes, or use the task note button to add task notes.
7. Click **Share** to download a self-contained HTML file you can email.
8. Use the menu to import or export CSV task data.

## Notes
- Dates are normalized to business days (Mon–Fri).
- When a task depends on another, it starts on the next business day after the predecessor ends.
- If you filter tasks, the Gantt view shows only matching tasks.
- Undo/redo stores up to 80 snapshots by default.
