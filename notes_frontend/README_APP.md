Notes Frontend (Astro)

Features
- Local, client-side authentication (prompt-based) for demo.
- Create, edit, and delete notes.
- Notes list with search and tag-based filtering.
- Tag management via comma-separated input.
- Minimal modern UI with a light theme and color palette:
  - primary: #1e88e5
  - secondary: #1565c0
  - accent: #ffd600

Development
- npm install
- npm run dev  (served at http://localhost:3000)

Implementation Notes
- State is fully client-side using a simple Store abstraction (src/lib/store.ts) persisted to localStorage.
- No backend integration is required for this task; swapping the store to remote APIs can be done later.
- Layout:
  - TopBar: search + auth area.
  - Sidebar: new note + tag filters.
  - Main: split pane with NoteList and NoteEditor.

Environment
- No environment variables are required at this time (container_env: None).
