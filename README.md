[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/yOwut1-r)
[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=21363755&assignment_repo_type=AssignmentRepo)
# 07
Neurosynth Frontend

## AJAX Demo Frontend

This repository now includes a small, static AJAX frontend at `index.html` that talks to Tren's backend (default: `https://mil.psy.ntu.edu.tw:5000`). The page uses Bootstrap (CDN) and optional Tailwind utilities for a compact, pretty UI.

Usage

* Serve this folder with a static server (do not open the file via `file://`):

```bash
python3 -m http.server 8000
# then open http://localhost:8000 in your browser
```

* The UI allows you to edit the Base URL and Path (defaults to `/terms`) and fetch the endpoint. JSON responses are pretty-printed.

Notes

* The backend must allow CORS from the origin serving this page. If you get a network/CORS error, check the server's CORS configuration.
* The frontend is intentionally dependency-free (CDNs only) so you can deploy to GitHub Pages or any static host quickly.

Deployment

* GitHub Pages: push to GitHub and enable Pages for the `main` branch (root). The page will be available at `https://<username>.github.io/<repo>`.
* Alternate hosts: Netlify, Vercel, Surge are all viable for static hosting.

Next steps

* Add an interactive JSON tree viewer.
* Add a small samples list of common endpoints.
