# 🌿 Boulder Green Commute Guide

> A community resource helping Boulder, Colorado residents make sustainable travel choices — one step and one pedal at a time.

---

## 🚶 Walking & 🚴 Biking Commute Analysis

This guide presents a detailed analysis of walking and biking commute options for a route in Boulder, CO — **45 Oak Avenue (home) → 1800 Broadway (office)** — using verified live OpenStreetMap routing data.

### 📍 Verified Locations

| | Address | Coordinates |
|---|---------|-------------|
| 🏠 **Home** | 45 Oak Avenue, Boulder, CO 80304 | `40.0448805°N, 105.2738879°W` |
| 🏢 **Office** | 1800 Broadway, Boulder, CO 80302 | `40.0163281°N, 105.2789726°W` |

### ⏱️ At a Glance

| Metric | 🚶 Walking | 🚴 Biking |
|--------|-----------|----------|
| **Distance** | **4.03 km / 2.5 mi** | **4.03 km / 2.5 mi** |
| **Realistic One-Way Time** | **~48–50 minutes** | **~12–15 minutes** |
| **Average Speed** | 5 km/h (3.1 mph) | 16–19 km/h (10–12 mph) |
| **Calories Burned** | ~280–340 kcal/trip | ~120–180 kcal/trip |
| **CO₂ Saved vs. Car** | ~0.9 kg/trip | ~0.9 kg/trip |
| **Annual CO₂ Save (260 rt)** | **~234 kg** | **~234 kg** |
| **Cost** | ✅ Free | ✅ Free |
| **Weather Dependent** | Yes — bundle up in winter! | Yes — layers, fenders, lights |

---

## 🗺️ Route Overview

Both walking and biking routes share the same scenic corridor through central Boulder — **Oak Ave → 19th St → 20th St → Pearl St → 18th St → Canyon Blvd** — passing near CU Boulder campus and downtown.

| # | Street | Distance | Walk Time | Bike Time |
|---|--------|----------|-----------|-----------|
| 1 | Oak Avenue | 97 m | ~12 s | ~14 s |
| 2 | 19th Street | 2,157 m | ~4 min | ~1 min 20 s |
| 3 | 20th St. | 106 m | ~13 s | ~15 s |
| 4 | 20th Street | 566 m | ~7 min | ~2 min |
| 5 | Pearl Street | 216 m | ~28 s | ~17 s |
| 6 | 18th Street | 249 m | ~31 s | ~18 s |
| 7 | Canyon Boulevard | 637 m | ~1 min | ~28 s |
| | **TOTAL** | **4,027 m** | **~48–50 min** | **~12–15 min** |

---

## 🌱 Why Green Commuting Matters

- 🌍 **Reducing emissions** — A single 4 km car trip produces ~0.9 kg of CO₂
- 💪 **Improving health** — Walking 30+ min/day reduces heart disease risk by up to 30%
- 💰 **Saving money** — Walking/biking cost $0/mile vs. $0.65/mile driving
- 🚗 **Reducing congestion** — Fewer cars, better traffic for everyone
- 🏔️ **Supporting Boulder's green ethos** — 300+ miles of bike paths, 45,000+ acres of open space

---

## 🗂️ Repository Files & Resources

| File | Description |
|------|-------------|
| [`routes/commute-analysis.md`](routes/commute-analysis.md) | 📝 Detailed walk & bike commute analysis |
| [`routes/verified-commute-analysis-45-oak-to-1800-broadway-aug2026.md`](routes/verified-commute-analysis-45-oak-to-1800-broadway-aug2026.md) | ✅ Live OSM-verified commute analysis |
| [`routes/route.geojson`](routes/route.geojson) | 🗺️ Route geometry (GeoJSON) for mapping tools |
| [`route-map.html`](route-map.html) | 🌐 Interactive HTML route map |
| [`route_details_45_octave_to_1800_broadway.md`](route_details_45_octave_to_1800_broadway.md) | 📋 Turn-by-turn walking & biking directions |
| [`neighborhood/neighborhood-context.md`](neighborhood/neighborhood-context.md) | 🏘️ Neighborhood amenities throughout the corridor |
| [`sustainability/sustainability-impact.md`](sustainability/sustainability-impact.md) | 🌿 Full impact & sustainability analysis |

---

## 🚴 Boulder Biking & Walking Resources

- [Boulder B-Cycle](https://bouldercolorado.gov/bcycle) — Bike share program, 44 stations
- [Boulder Connectivity Map](https://bouldercolorado.gov/streets/connectivity) — Official bike network
- [RTD Bike & Ride](https://www.rtd-denver.com/riding/bike-and-ride) — Combine biking with public transit
- [CU B-cycle](https://www.cubicycle.org/) — University bike-share, convenient stations on this route
- [OpenStreetMap — Boulder](https://www.openstreetmap.org/#map=15/40.0163/-105.2790) — Explore the route live!

---

## 🔍 Route on OpenStreetMap

- 🏠 **Home (45 Oak Ave):** [View on OSM](https://www.openstreetmap.org/#map=15/40.0449/-105.2739)
- 🏢 **Office (1800 Broadway):** [View on OSM](https://www.openstreetmap.org/#map=15/40.0163/-105.2790)
- 🗺️ **Both points & route:** [OSRM Directions](https://map.project-osrm.org/?zoom=13&alternatives=1&annotations=true&instructions=true&operand=foot&osmId=&osmType=N&output=json&routeType=shortest&summary=true&waypoints=40.0448805%2C-105.2738879%3B40.0163281%2C-105.2789726)

---

## 🤝 Contributing

This is a community guide! **Help us make it better for all Boulder residents.**

### How to Add Your Own Commute Analysis
1. Geocode 📍 your home and work addresses using [Nominatim](https://nominatim.openstreetmap.org/)
2. Run a commute analysis with the [OSRM live demo](https://map.project-osrm.org/)
3. Add your route as a `.md` file under `/routes`
4. Include a GeoJSON `.geojson` file of your route geometry if available
5. Submit a pull request! 🎉

---

## 📊 Data Sources

| Component | Source |
|-----------|--------|
| Geocoding | Nominatim (OpenStreetMap) |
| Route & Direction Engine | OSRM (Open Source Routing Machine) |
| Coordinate-led Route Polyline | OSRM; 70 verified coordinate points in `route.geojson` |
| Carbon Emission Factors | U.S. EPA GHG Emission Factors Hub (2024) |
| Calorie Estimates | Compendium of Physical Activities (Ainsworth et al., 2011) |
| Infrastructure Planning | City of Boulder Mobility & Connectivity Plan 2024 |

---

## 💬 Get Involved

- 🔍 Open an [Issue](https://github.com/zhub9006/boulder-green-commute-guide/issues) to suggest improvements
- 📧 Share this guide with neighbors, coworkers, and CU Boulder friends
- 🚲 Advocate for more protected bike lanes in Boulder!
- 🌍 Start a similar repo in your city — open-source sustainability!

---

*Made with ❤️ for a greener Boulder. Data verified September 2026. Data © OpenStreetMap contributors, ODbL 1.0.*
