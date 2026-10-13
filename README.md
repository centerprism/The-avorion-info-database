# Avorion — Industrial Database

Interactive reference for factories, mines, farms, materials and utility stations for the game Avorion.

This repository's single canonical data/view is the self-contained HTML file:

- `avorion_factory_station_database.html` — interactive browser reference (JavaScript + styles bundled inline). The database and UI are included in that file.

What this README adds

This README explains how to use the database from the repository's main file, how to view it in a browser, and how to embed or extract the data for other projects.

Quick start — preview locally (recommended)

1) Clone the repo:

```bash
git clone https://github.com/centerprism/The-avorion-info-database.git
cd The-avorion-info-database
```

2) Start a simple static server and open the page:

```bash
# Python 3
python3 -m http.server 8000
# then open in your browser:
# http://localhost:8000/avorion_factory_station_database.html
```

Open the file directly

You can also open `avorion_factory_station_database.html` directly from your filesystem (double-click). Note: some browsers restrict JavaScript features when using the file:// protocol, so use a local server if you see problems.

Serve via GitHub Pages

To make the page publicly available with GitHub Pages, either:

- In the repository Settings → Pages, set the Source to the default branch and the root folder. After saving, the page will be available at `https://centerprism.github.io/The-avorion-info-database/avorion_factory_station_database.html` (or the repository root if you rename/copy the file to `index.html`).

- Or move/copy `avorion_factory_station_database.html` into a `docs/` folder on the default branch and set Pages source to the `docs` folder; it will then be served at `https://centerprism.github.io/The-avorion-info-database/`.

Embedding the database in other pages

If you want to include the interactive reference in another website, you can embed the HTML file using an iframe. Example:

```html
<iframe src="/centerprism/The-avorion-info-database/main/avorion_factory_station_database.html" style="width:100%;height:800px;border:0"></iframe>
```

(Adjust the `src` path to point to a hosted copy — e.g., your GitHub Pages URL or a local server URL.)

Programmatic access & data extraction

The repository's primary data is bundled inside `avorion_factory_station_database.html` as part of the page's JavaScript. If you need machine-readable access (JSON, CSV, or a small API) you have a few options:

- Open the HTML file in a text editor and locate the embedded data structures — you can copy / convert them to JSON.
- I can extract the embedded data and add a new file (e.g. `data/avorion_db.json`) to this repository so other tools can consume it directly.
- Alternatively, I can add a small script (Node/Python) that reads the HTML and outputs a JSON file as part of the repo.

If you want me to add a JSON export or a `docs/index.html` copy for GitHub Pages, tell me which option you prefer and I'll update the repo.

Notes

- The HTML file is self-contained and should work offline when opened correctly.
- If you want the HTML to be the repository homepage on Pages, rename it to `index.html` or place a copy at `docs/index.html`.

Questions / next steps

I updated this README to explain how to use the database from the repository's main HTML file. I can now:

- Add `docs/index.html` (copy of the main file) so Pages serves the UI as the repo homepage, or
- Extract the embedded database into `data/avorion_db.json`, or
- Add a small extraction script (Node or Python) that produces a JSON file from the HTML.

Which would you like me to do next?
