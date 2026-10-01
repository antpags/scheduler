# CB Elementary Scheduling v15

**Central Bucks School District — Elementary Specialist Scheduling Tool**

A browser-based scheduling optimizer for 15 elementary schools across 5 specialist subjects (PE, Music, Art, Library, QUEST).

## Features

- **Target 30 sections/specialist** · 1.0 FTE = 30–32 sections · Bins fill to 32 to minimize headcount
- **FFD section-packing algorithm** with travel-aware greedy day-fill
- **55 district-wide specialists** from 336 total sections (⌈336÷32⌉ = 11/subject × 5)
- **Travel time enforced** — A→C uses natural 30-min schedule gap; C→A blocked
- **Full constraint audit** — FTE consistency, daily load ≤7, travel order, section coverage
- **Principal View** — per-school specialist schedule for distribution
- **Auto-generates all 15 school schedules** on optimizer run
- **Grade-level section entry** (K–5) drives dynamic teacher rosters

## Data

- 2026-27 Tentative Elementary Staffing (K–5), screenshot-verified: **336 total sections**
- All 15 CB elementary schools: Barclay, Bridge Valley, Buckingham, Butler, Cold Spring, Doyle, Gayman, Groveland, Jamison, Kutz, Linden, Mill Creek, Pine Run, Titus, Warwick
- Schedule types: A (8:35–3:15) · B (8:50–3:30) · C (9:05–3:45)

## Deployment

Pure static HTML — no server, no build step, no dependencies. Works entirely in the browser. Local storage persists edits between sessions.

```bash
# Deploy to Vercel
npx vercel --prod
```

## Usage

1. Open the app → click **🧮 Run Optimizer (All 15 Schools)**
2. All 15 school schedules generate automatically
3. View **📋 Assignments** → **🗂️ Specialist Cards** → **🏫 Principal View**
4. **🔍 Full Audit** verifies all constraints
5. Click any school in the sidebar to jump to its Principal View
6. Print or export CSV per school

## License

Internal use — Central Bucks School District © 2026
