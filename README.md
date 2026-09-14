# Portfolio site

## Publish to GitHub Pages
1. Create a repo (e.g. `yourusername.github.io`, or any repo name if you'll use a project page).
2. Push these files keeping the folder structure exactly as-is:
   ```
   index.html
   assets/models/Steering_Wheel.glb
   assets/models/eNav.glb
   assets/models/PCB1.glb
   resume.pdf   <- add your resume here, filename must match the link in index.html
   ```
3. In the repo settings, enable GitHub Pages (Settings → Pages → Deploy from branch → main / root).

## Still needs your input (marked `TODO` in index.html)
- Real name/description for `PCB1` project
- Contact email, LinkedIn, GitHub links (currently placeholders)
- Experience bullet detail (dates, scope) — send your resume and I'll fill these in precisely
- `resume.pdf` file itself isn't included — drop it in the root folder

## 3D viewers
- Models were converted from your STEP files to `.glb` (web-friendly) using `cascadio`.
- Viewer code uses three.js (loaded from CDN via import map) with `OrbitControls`:
  drag to rotate, scroll to zoom, right-click drag to pan.
- Models lazy-load only when their viewer scrolls into view, so page load stays fast.
