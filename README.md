# LaLaLeads – Dashboard Analytics CRM

Static, client‑side dashboard to analyze CRM exports (CSV) with Chart.js and PapaParse.  
Works on GitHub Pages — no backend required.

## 🚀 Quick start (GitHub Pages)

1. Create a new public repository (e.g. `lalaleads-dashboard`).
2. Upload these files:
   - `index.html`
   - `sample-data.csv`
   - `README.md`
3. Enable **GitHub Pages** in your repo settings:
   - Settings → Pages → **Source**: `Deploy from a branch`
   - **Branch**: `main` (or `master`) → `/ (root)` → **Save**.
4. Open the Pages URL (shown by GitHub) to use the app.

## 🧪 Demo data
Click **“charger les données de démo”** to load `sample-data.csv` and explore the dashboard without uploading anything.

## 📦 Local run
Just open `index.html` in your browser (Chrome/Edge/Firefox).

## 📝 CSV columns expected
- `Campagne`
- `Phase du cycle de vie` (e.g., `RDV confirmé`, `callback`, `Prospect à traiter`)
- `Nom de l'entreprise`
- `Last used Aircall tags` (optional; used for “pitch” → RDV conversion)

> The app is resilient to missing values and extra columns.

## ✨ Notes
- Uses **Chart.js 3.x**. Horizontal bars are implemented with `type: "bar"` and `indexAxis: "y"`.
- Report/PPT exports are stubbed with alerts; you can wire them to a real exporter later.
