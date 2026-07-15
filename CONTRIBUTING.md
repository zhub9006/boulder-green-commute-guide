# 🤝 Contributing to Boulder Green Commute Guide

This guide is for Boulder residents, by Boulder residents! Help us make it better.

---

## Ways to Contribute

### 1. Add Your Own Commute Route
Want to share walking/biking analysis for your own route?

1. **Fork** the repository
2. Create a new branch: `your-name-route-name` (e.g., `sarah-nashville-to-globe`)n3. Add your analysis in `routes/[your-name]-[route-slug].md`
4. Add machine-readable data to `route_data/[your-name]-[route-slug].json`
5. Submit a Pull Request with a clear description

### 2. Improve Existing Content
- Fix typos or outdated info
- Add new nearby cafés, shops, or landmarks
- Update neighborhood amenities
- Improve safety notes

### 3. Share Your Experience
- How does YOUR commute compare? (Time, cost, fitness gains)
- What obstacles did you face and how did you overcome them?
- Add a `stories/` section with real commuter testimonials

---

## 📐 Contribution Guidelines

### Format
- Use **Markdown** for all text files
- Use **JSON** for machine-readable data
- Include the following for each route:
  - Origin → Destination coordinates (WGS84)
  - Total distance (km & miles)
  - Segment-level breakdown with OSM street names
  - Travel time estimates for both walking AND biking
  - Bike infrastructure quality ratings
  - Nearby amenities (cafés, shops, transit stops)
  - Seasonal tips & safety notes

### Data Sources
- **Primary:** OpenStreetMap (open source, community-maintained)
- **Supplemental:** City of Boulder GIS, RTD schedules, Google Places
- **Always verify** OSM data against ground truth
- Cite your data sources and verification dates

### File Naming
```
routes/[your-name]-[destination]-[mode].md
route_data/[your-name]-[destination]-[mode].json
stories/[your-name]-commute-story.md
```

### Pull Request Process
1. Fork the repo
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add your feature'`)
4. Push to your branch (`git push origin feature/your-feature`)
5. Open a Pull Request
6. Include a clear description of what you added and why

---

## 🐛 Reporting Issues

- **Outdated routes:** Paths may change — report closures, construction, new bike lanes
- **Data errors:** If OSM data is wrong, fix it! [OpenStreetMap Editor](https://www.openstreetmap.org/edit)
- **General feedback:** Open an issue with the `suggestion` label

---

## 💬 Community

- **Join the conversation:** Post in the repo's GitHub Discussions
- **Slack/Discord:** Check for local Boulder sustainability groups
- **Social:** Use #BoulderGreenCommute on social media

---

## 📋 Code of Conduct

- Be welcoming and inclusive
- Share genuine, verified information
- Respect different commuting choices (not everyone can walk/bike — that's OK!)
- Help others make informed decisions

---

## local Boulder Sustainability Organizations to Check Out

| Org | Focus | Link |
|---|---|---|
| Boulder Transportation Advisory Committee | City policy | [ci.boulder.co.us/HMAS/BTAC](https://www.bouldercolorado.gov/hmas/btac)) |
| PeopleForBikes | National bikes advocacy | [peopleforbikes.org](https://peopleforbikes.org/) |
| Colorado Gotta Get Outdoors | Health & outdoor activity | [hasstimeso.org](https://colorado.gov/gov/greenbook) |
| Eagle Crest | Local Boulder advocacy | — |
| B-cycle | Bike-share program | [bcycle.com/boulder](https://www.bcycle.com/boulder) |
| S-lang | Missoula Shout (Local Open Space Access) | — |

