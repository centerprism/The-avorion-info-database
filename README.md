# Avorion — Industrial Database

Interactive reference for factories, mines, farms, materials and utility stations for the game Avorion.

This repository includes a single self-contained HTML reference file:

- `avorion_factory_station_database.html` — interactive browser reference (JavaScript + styles bundled inline).

How to view the HTML page

1) Preview locally (recommended):

```bash
# clone the repo
git clone https://github.com/centerprism/The-avorion-info-database.git
cd The-avorion-info-database

# start a simple static server (Python 3)
python3 -m http.server 8000

# open in your browser:
# http://localhost:8000/avorion_factory_station_database.html
```

2) Open the file directly in your browser

You can also open `avorion_factory_station_database.html` directly from your filesystem by double-clicking it, but some browsers may restrict certain JavaScript features when using the `file://` protocol. Using a simple local HTTP server as shown above avoids those issues.

3) (Optional) Serve via GitHub Pages

To make the page publicly available at a GitHub Pages URL, one of these options works:

- In the repository Settings → Pages, set the Source to the default branch and the root folder. After saving, the page will be available at `https://centerprism.github.io/The-avorion-info-database/avorion_factory_station_database.html`.

- Or move the HTML file into a `docs/` folder on the default branch and set Pages source to the `docs` folder. That also serves the file at `https://centerprism.github.io/The-avorion-info-database/avorion_factory_station_database.html`.

Notes

- The HTML file is self-contained and should work offline.
- If you want the file to be the repository homepage on Pages, rename it to `index.html` or add a copy to `docs/index.html`.

If you'd like, I can:
- Add a copy of the HTML to `docs/index.html` so Pages works without manual settings change, or
- Automatically create a small index README that embeds a link or screenshot, or
- Enable a GitHub Actions workflow that publishes Pages (requires repository settings/permissions).

