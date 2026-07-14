# Contributing to Boulder Green Commute Guide

This guide is a community resource for making sustainable commuting choices in Boulder, Colorado. Everyone is welcome to contribute!

## 🎯 How to Help

### Report Route Changes
OpenStreetMap is a living map. If you notice:
- 🚧 Construction or road closures affecting walk/bike routes
- 🚲 New bike lanes or infrastructure added
- ⚠️ Safety hazards or missing sidewalks
- 🌳 Tree removal or new plantings affecting shade

**Please:**
1. Verify the change on OpenStreetMap first
2. Create a GitHub issue describing the change
3. Include coordinates (lat/long) and a description

### Add Local Commute Routes

Want to share another Boulder commute route?

1. Fork this repository
2. Create a new file in `routes/` named `commuter_name_route.md`
3. Follow the template in the routing files
4. Submit a pull request

Include:
- Start and end points (use OSM addresses)
- Segment-by-segment directions
- Infrastructure notes (bike lanes, sidewalks, Canyon Blvd access)
- Nearby amenities (food, coffee, transit stops)
- Seasonal notes and weather tips

### Fix or Update Amenity Data

Our amenity data comes from OpenStreetMap (July 2025 verification). Businesses open/close, so:

1. Check OpenStreetMap for the current listing
2. If updated on OSM, update `neighborhood_analysis.md` and `route_data.json`
3. Submit a PR with the updated details

### Translate

We welcome translations! Boulder is an international community:
- Create a file `i18n/README.{lang}.md` (e.g., `i18n/README.es.md`)
- Translate the README and key sections
- Add a note about your language in the README

### Suggest New Features

Found a gap in this guide? File an issue with:
- **Feature requested:** Brief description
- **Boulder relevance:** Why this matters for local commuters
- **Data needed:** What information would fill the gap

## 🏷️ Code Style

- All markdown files use **Heading 2 (`##`)** for sections and **Heading 3 (`###`)** for subsections
- Route files use table format with consistent columns: Direction | Distance | Time | Notes
- JSON files follow the `route_data.json` schema — see the existing file for the template
- Link all URLs that are repeated: [B-Cycle Boulder](https://www.b-cycle.com/cities/b-cycle-boulder/boulder-co), [colorado.gov/ebike](https://colorado.gov/ebike), [bikeboulder.org](https://bikeboulder.org)

## 📋 Pull Request Process

1. **Fork** the repo
2. **Create** a feature branch (`git checkout -b feature/your-feature`)
3. **Add** your content or updates
4. **Test:** Ensure all links work and all tables render properly
5. **Commit** with a clear message (e.g., "Add Pearl Street winter walking tips")
6. **Open** a Pull Request with:
   - A clear description of changes
   - Links to related issues if applicable
   - Verification that OSM data is current

Thank you for helping Boulder residents commute greener! 🌿🚶🚴