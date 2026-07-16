# 📝 Contributing Guide — Add Your Own Commute

Boulder is a city of cyclists and walkers! This guide is for Boulder residents, by Boulder residents. Want to share your own commute route analysis to help fellow Boulderites make sustainable travel choices? Wonderful — here's how:

---

## How to Add Your Own Commute Route

### 1. Fork the Repository
```bash
git clone https://github.com/zhub9006/boulder-green-commute-guide.git
cd boulder-green-commute-guide
git checkout -b your-name-walking-to-work
```

### 2. Add Your Route Files
Add a new `.md` file in the `routes/` directory:
```
routes/your_name_route-name.md
```

**Use this template:**

```markdown
# 🚶 [Your Mode] Route: [Your Start] → [Your Destination]

**Total distance:** [X] km  
**Estimated Time:** [X] minutes  
**Elevation Gain:** [X] m  
**Data Source:** OpenStreetMap routing API (or other verified source)

## Turn-by-Turn Directions

1. [Starting point] — [landmark description] | [distance] | [time]
2. [Next turn] — [description] | [distance] | [time]
...

## Route Overview
```
Start: [Your Address] (lat, lon)
  1. [Street] ([distance m])
  2. [Street] ([distance m])
  ...
End: [Destination] (lat, lon)

Total: [segments] | [distance] m | [time]
```

## Safety Notes
- [Key safety considerations for this route]
- [Worst segment and how to navigate it]
- [Best segment — the "hidden gem"]

## Seasonal Considerations
- [Best and worst seasons for this route]
- [Weather risks at Boulder's 5,430 ft altitude]

## CO₂ Impact
- Walking: **0 kg** | Biking: **0 kg** | Driving: ~[X] kg
```

### 3. Use Verified Data
Whenever possible, use:
- **OSM Nominatim API** to geocode addresses (get lat/lon coordinates)
- **OSM Valhalla Routing API** to calculate routes
- **OSM way IDs** to identify street-level infrastructure
- **Realistic pace estimates:** 5 km/h walking with intersection delays; 15 km/h biking with standard stops
- **Local knowledge:** Segment safety ratings, infrastructure quality, known problem spots

### 4. Commit & Push
```bash
git add routes/your_name_route-name.md
git commit -m "Add [your name] commute route: Start → Destination"
git push origin your-name-walking-to-work
```

### 5. Open a PR
Go to https://github.com/zhub9006/boulder-green-commute-guide and open a Pull Request. Include:
- Who you are (Boulder resident)
- What your route is
- Any notable observations about the infrastructure
- Your planned primary mode and any alternatives

---

## Directory Structure

```
boulder-green-commute-guide/
├── README.md                          # Main entry point — route overview + guide index
├── commute_analysis.md                # Full mode-by-mode analysis (walking, biking, driving)
├── analysis_summary.md                # Side-by-side walk vs. bike comparison
├── sustainability_impact.md           # CO₂, health benefits, financial analysis
├── verified_route_data.md             # Raw OSM API data + verification checklist
├── neighborhood_analysis.md           # Origin + destination neighborhood profiles
├── data-sources.md                    # Sources + methodology
├── route_data.json                    # Machine-readable route data (GeoJSON, segments)
├── route_map.html                     # Interactive Leaflet map (walking + biking)
├── green_tips.md                      # Seasonal tips + gear recommendations
├── green_tips_seasonal.md             # Season-by-season breakdown
├── CONTRIBUTING.md                    # This file — how to contribute
├── LICENSE                            # MIT License
└── routes/
    ├── README.md                      # Quick reference for all route files
    ├── walking_route.md               # Turn-by-turn walking directions
    ├── biking_route.md                # Turn-by-turn biking directions
    └── commute-route-details.md       # Combined route details + safety ratings
```

---

## Data Sources — Be Respectful, Fact-Check, Cite

### OpenStreetMap (Primary)
| Data Point | Source | Citation |
|---|---|---|
| Address geocoding | OSM Nominatim | OSM Nominatim API |
| Route calculation | OSM Valhalla Router | OpenStreetMap Contributors |
| Bike infrastructure | OSM tags (bike=lane, highway=*) | OSM contributors |
| Street names | OSM way data | OSM contributors |
| Bus routes | RTD + OSM bus routes | RTD Boulder + OSM |

### Supporting Data
| Source | Usage | Source URL |
|---|---|---|
| Boulder Transportation Master Plan | Route validation, infrastructure context | bouldercolorado.gov/transportation |
| RTD (Regional Transportation District) | Bus schedules, routes, EcoPass info | rtab.com |
| B-Cycle | Bike-share pricing, station locations | boulder.b-cycle.com |
| Colorado Energy Office | E-Bike rebate program details | energystone.colorado.gov |
| Boulder Bike Partnership | Advocacy, education, community rides | bikeboulder.org |
| Boulder County Open Space | Trail maps, seasonal closures | bouldercolorado.gov/openspace |
| Boulder City Code | Helmet laws, pedestrian rules | bouldercolorado.gov |
| US EPA Emission Factors | CO₂ calculations for driving mode | epa.gov |

---

## Quality Standards

### ✅ DO
- Cite your sources (OSM, RTD, Colorado Energy Office, etc.)
- Verify data against multiple sources when possible
- Include coordinates (lat/lon) for start and end points
- Segment-level detail: distance, time, surface type, traffic level
- Infrastructure ratings (1–5 stars) for each segment
- Mention both primary mode and alternative modes
- Include seasonal/weather considerations
- Note CO₂ savings and health benefits
- Use clear, Boulder-friendly language

### ❌ DON'T
- Make up data or estimates without clearly labeling them as estimates
- Copy from copyrighted sources
- Include personally identifiable information (addresses are fine; phone numbers are not)
- Use current-episode data without verification
- Omit infrastructure limitations (dooring risks, no-bike zones, dismount required)
- Ignore Boulder's high-altitude conditions (5,430 ft — UV, altitude, weather)
- Forget to mention Boulder's $1,200 E-Bike Rebate and B-Cycle program

---

## Community Etiquette

This guide is for Boulder residents, by Boulder residents and meant to be:
- **Welcoming** — We celebrate all modes of active transportation
- **Accurate** — Fact-check before contributing
- **Helpful** — Explain not just *what* but *why* (e.g., why dooring risk matters)
- **Inclusive** — include walk/bike/bus/e-bike options to serve all mobility levels
- **Respectful** — Be kind and constructive in PR reviews

### PR Review Process
1. Automated: Verify OSM route data matches submitted text
2. Community: At least 1 other Boulder contributor reviews
3. Merge: After review approval, maintainers merge and update README index

---

## Need Help?

- 📧 Open an issue on GitHub: https://github.com/zhub9006/boulder-green-commute-guide/issues
- 🚲 Boulder Bike Partnership: https://bikeboulder.org
- 🚌 RTD Customer Service: https://rtab.com (RTD website)
- 🗺️ Boulder Transportation: https://bouldercolorado.gov/transportation
- 🗣️ Boulder campus cycling: https://bikeboulder.org/go-bike-boulder

---

## License

All contributions are licensed under the [MIT License](LICENSE). By contributing, you agree that your contributions will be licensed under the same terms.

---

*This is a community-built resource for Boulder, Colorado. If you live here, bike here, or walk here, we welcome your contributions. Together, let's make Boulder's commutes cleaner, healthier, and more sustainable. See [CONTRIBUTING.md](https://github.com/zhub9006/boulder-green-commute-guide/blob/main/CONTRIBUTING.md) for contribution guidelines.*
