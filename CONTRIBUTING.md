# 🤝 Contributing to the Boulder Green Commute Guide

This guide is for Boulder residents, by Boulder residents. Help us make it better!

---

## How to Add Your Own Commute Route

### Step 1: Geocode Your Addresses
1. Go to [OpenStreetMap](https://www.openstreetmap.org) or use a geocoding service
2. Find the coordinates (latitude, longitude) of your home and workplace

### Step 2: Analyze Your Route
1. Walk or bike the route and note the segments
2. Record street names, distances, and any notable features
3. Note bike infrastructure quality (bike lane, shared path, separated lane)
4. Identify transit stops and bike-share stations along the way

### Step 3: Document Your Findings
1. Create a new file (e.g., `routes/route_xxx.md`) following our format
2. Include:
   - Full addresses and coordinates
   - Segment-by-segment directions with distances and times
   - Transit options and bike-share availability
   - Seasonal notes and safety considerations
   - Cafés, parks, and landmarks worth knowing

### Step 4: Open a Pull Request
1. Fork this repository
2. Create a new branch (`git checkout -b add-route-xxx`)
3. Commit your changes
4. Open a Pull Request with a clear description

--n
---

## Suggested Format for New Route Files

```markdown
# [Mode] Route: [Origin] → [Destination]

**Distance:** X km (X mi) | **Estimated Time:** ~X min | **Terrain:** [description]

## Turn-by-Turn Directions
1. [Street Name] (X m) — ~X min — [brief description]
2. [Street Name] (X m) — ~X min — [brief description]
...

## Key Landmarks
| Landmark | Location | Description |
|---|---|---|
... | ... | ... |

## Safety Notes
- [any hazards, lights, crossings]

## Fitness & Health
- [calories burned, elevation, altitude notes]
```

---

## Reporting Issues or Incorrect Data

1. **Check OpenStreetMap:** Many of our route details come from OSM. If you notice discrepancies, please update OSM directly:
   - [Edit on OpenStreetMap](https://www.openstreetmap.org/edit)
2. **File a GitHub Issue:** For data corrections or missing information
3. **Verify locally:** Always double-check routes — construction and changes happen!

---

## Code of Conduct

- Be welcoming and inclusive — all Boulder residents and visitors are welcome
- Respect the environment — our mission is sustainability
- Leave trails better than you find them
- Share your knowledge — the best routes come from local experience

---

## Want More?

- **Add neighborhood analysis** — Create `neighborhoods/xxx.md`
- **Add sustainability data** — Create `impacts/xxx.md`
- **Add business listings** — Create `businesses/xxx.md`
- **Add data visualizations** — Create `plots/xxx.py` to generate charts from `route_data.json`

---

## Questions?

Open a GitHub Issue and we'll get back to you. We're all volunteers building a better Boulder!

---

*Let's make Boulder the greenest commuting city in Colorado.* 🌱🚲🚶
