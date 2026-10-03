# IPU East Campus Navigator

A browser-based shortest-route finder prototype for GGSIPU East Delhi Campus, Surajmal Vihar.

## Features
- Choose a starting point and destination.
- Search for the library, canteen, EDC Chowk, Chill Zone, lecture halls, classroom blocks, schools, auditorium, sports complex and hostel area.
- Find and display a shortest route and estimated graph cost.
- Interactive schematic map; click markers or location cards to choose a destination.
- Works in a modern browser without installing dependencies.

## Run
Open `index.html` in Chrome, Edge, Firefox or Safari.

## Publish
Upload all three files to the repository root, then configure GitHub Pages: Settings → Pages → Deploy from a branch → `main` → `/(root)` → Save.

## Graph and algorithm
Locations are vertices and assumed walkable connections are undirected weighted edges. Dijkstra's algorithm finds the minimum-total-cost route for non-negative edge weights. This simple implementation scans all vertices to select the next minimum-distance vertex, so time complexity is O(V² + E); space complexity is O(V + E). A min-heap can improve time to O((V + E) log V).

## Accuracy limitation
This is a student-project prototype, not an official surveyed campus map. The university's public website confirms the East Delhi Campus at Surajmal Vihar and identifies its schools, but exact locations of student-named places (such as Chill Zone and EDC Chowk), individual classrooms and pedestrian connections have not been verified. Map positions and costs are illustrative; verify routes with campus signage before relying on them.
