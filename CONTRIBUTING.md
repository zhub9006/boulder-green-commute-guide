# Contributing to Boulder Green Commute Guide 🌿

We welcome contributions from the Boulder community! Here's how you can help make this a better resource for sustainable commuting in Boulder.

---

## How to Contribute

### 1. Fork & Clone
```bash
git clone https://github.com/zhub9006/boulder-green-commute-guide.git
cd boulder-green-commute-guide
```

### 2. Create a Branch
```bash
git checkout -b your-feature-name
```

### 3. Make Your Changes
- **Add a new route**: Create a new file in `routes/` with turn-by-turn directions
- **Update amenities**: Add new cafes, B-Cycle stations, or parks to `neighborhood_analysis.md`
- **Add commute data**: Use the OSM MCP tools to analyze a new commute route
- **Fix errors**: Typos, outdated info, missing data

### 4. Commit & Push
```bash
git add .
git commit -m "Add: brief description of your changes"
git push origin your-feature-name
```

### 5. Open a Pull Request
Describe your changes and why they help the Boulder community.

---

## Data Sources

All route and amenities data should be verified from OpenStreetMap (verified within the last 3 months). Key tools:

- **Geocoding**: Convert addresses to coordinates
- **Route directions**: Get turn-by-turn directions for walking and biking
- **Nearby places**: Search for amenities (cafes, bike stations, parks, etc.)
- **Neighborhood analysis**: Generate comprehensive area profiles

---

## Adding a New Commute Route

To add analysis for a different Boulder commute:

1. Geocode both origin and destination addresses
2. Run route directions for both `foot` and `bike` modes
3. Run `analyze_commute` for both modes
4. Search for nearby amenities using the home coordinates
5. Create a new file in `routes/` with the analysis
6. Update `route_data.json` with the new commute data
7. Add the new route to the README

---

## Community Standards

- **Be inclusive**: All modes of transportation are welcome
- **Be accurate**: Only include verified, up-to-date information
- **Be helpful**: Focus on practical, actionable advice
- **Be sustainable**: Prioritize green transportation options

---

## Questions?

Open an issue or reach out to the repository maintainer. Together, let's make Boulder the greenest commute city in Colorado! 🚶‍♂️🚴‍♀️🌲
