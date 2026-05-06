# AGENTS.md

## Cursor Cloud specific instructions

This is a single-file web application (`index.html`) — a Bartender Shift Tracker & Earnings Dashboard. There are no dependencies, no build tools, no package managers, and no backend.

### Running the app

Serve the app with any static HTTP server:

```bash
python3 -m http.server 8080 --directory /workspace
```

Then open `http://localhost:8080/index.html` in a browser.

### Key notes

- The entire application is in `index.html` (~2,963 lines of HTML + CSS + vanilla JS).
- There is no build step, no linting configuration, no test framework, and no CI/CD.
- All state is in-memory. The "Save Shift" button triggers `window.alert()` with JSON — there is no persistence layer.
- No external libraries or CDN resources are loaded; the app is fully self-contained.
