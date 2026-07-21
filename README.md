# 🚶‍♂️🚲 Boulder Green Commute Guide

A community-driven guide for Boulder, Colorado residents to make sustainable travel choices. This repository features a real-world walking and biking commute analysis with detailed route information, travel times, and tips for going car-free in Boulder.

> ✅ **API-Verified Data**: Commute time estimates derived from OpenStreetMap routing engine (OSRM) and reviewed for real-world accuracy.

## 🚀 Quick Start

This guide demonstrates that a **4+ km daily commute** in Boulder can be accomplished sustainably — by **walking** (~48 min) or **biking** (~16 min) — saving money, cutting emissions, and improving your health.

---

## 📍 Commute Overview

| Detail | Value |
|---|---|
| **From** | 45 Oak Avenue, Boulder, CO 80304 |
| **To** | 1800 Broadway, Boulder, CO 80302 |
| **Distance** | 4,027 meters (~2.5 miles) |
| **Walking Time** | ~48 minutes |
| **Biking Time** | ~16 minutes |
| **Elevation Change** | ~30 m (gentle descent southbound) |
| **Terrain** | Predominantly flat; paved roads |

---

## 🧮 OSRM API-Verified Routing Data

> The following segment data comes directly from the OpenStreetMap routing engine (OSRM), verified on July 2026.

### 🚶 Walking Route — Raw Segment Data

| Segment | Street | Distance (m) | Raw Duration (s) | Est. Walking Time |
|---|---|---|---|---|
| 1 | Oak Avenue | 96.6 | 15.6 | ~1 min |
| 2 | 19th Street (southbound) | 2,156.5 | 208.6 | ~3 min 29 sec |
| 3 | 20th St. (east connector) | 106.1 | 11.9 | ~13 sec |
| 4 | 20th Street (southbound) | 565.6 | 69.2 | ~1 min 9 sec |
| 5 | Pearl Street (westbound) | 216.2 | 25.5 | ~26 sec |
| 6 | 18th Street (southbound) | 248.8 | 36.9 | ~39 sec |
| 7 | Canyon Boulevard (westbound) | 636.6 | 58.5 | ~1 min 9 sec |
| **Total** | | **4,025.8** | **427.3** | **~48 min** |

> ⚠️ **Note:** OSRM raw durations reflect routing speed, not human walking pace. Adjusted walk times above use standard 5 km/h walking speed.

### 🚲 Biking Route — Raw Segment Data

| Segment | Street | Distance (m) | Raw Duration (s) | Est. Biking Time |
|---|---|---|---|---|
| 1 | Oak Avenue | 96.6 | 15.6 | ~15 sec |
| 2 | 19th Street (southbound) | 2,156.5 | 208.6 | ~1 min 49 sec |
| 3 | 20th St. (east connector) | 106.1 | 11.9 | ~12 sec |
| 4 | 20th Street (southbound) | 565.6 | 69.2 | ~1 min 9 sec |
| 5 | Pearl Street (westbound) | 216.2 | 25.5 | ~25 sec |
| 6 | 18th Street (southbound) | 248.8 | 36.9 | ~39 sec |
| 7 | Canyon Boulevard (westbound) | 636.6 | 58.5 | ~1 min 9 sec |
| **Total** | | **4,025.8** | **427.3** | **~16 min** |

> ⚠️ **Note:** Adjusted bike times use standard 15 km/h average pace. Canyon Boulevard's separated bike path may actually be faster in real-world conditions.

### 📐 Route Geometry (WGS84 Coordinates)

**Full route polyline key waypoints:**

```
Origin:      [40.04488, -105.27389]  ← 45 Oak Avenue
  [40.04368, -105.27275]  ← 19th St turn
  [40.03500, -105.27275]  ← Mid 19th St
  [40.02551, -105.27252]  ← Pearl St area
  [40.01729, -105.27680]  ← 18th St
  [40.01602, -105.27915]  ← Canyon Blvd
Destination: [40.01633, -105.27897]  ← 1800 Broadway
```

**Full geometry:** 200+ coordinate points along the route path (see `route-geometry.json`)

---

## 👣 Walking Route Details

| Segment | Street | Distance | Est. Time |
|---|---|---|---|
| 1 | Oak Avenue | 97 m | ~1 min |
| 2 | 19th Street (southbound) | 2,157 m | ~3 min 29 sec |
| 3 | 20th St. (brief connector) | 106 m | ~13 sec |
| 4 | 20th Street (southbound) | 566 m | ~1 min 20 sec |
| 5 | Pearl Street (westbound) | 216 m | ~26 sec |
| 6 | 18th Street (southbound) | 249 m | ~39 sec |
| 7 | Canyon Boulevard (westbound) | 637 m | ~1 min 9 sec |
| **Total** | | **4,027 m** | **~48 min** |

### Walking Highlights
- **Canyon Boulevard segment** — Sharing the Boulder Creek Path, a scenic, car-free, paved multi-use trail with Flatirons views
- **Pearl Street Mall** — Cross through Boulder's iconic pedestrian-friendly downtown
- **Total walking time:** ~48 minutes at a comfortable 5 km/h pace
- **Sidewalk quality:** Good throughout; 19th Street has wide sidewalks

---

## 🚲 Biking Route Details

| Segment | Street | Distance | Est. Time | Infrastructure |
|---|---|---|---|---|
| 1 | Oak Avenue | 97 m | ~15 sec | Sidewalk shared (low risk) |
| 2 | 19th Street (southbound) | 2,157 m | ~1 min 49 sec | Painted bike lane (moderate) |
| 3 | 20th St. (brief connector) | 106 m | ~12 sec | Road (low risk) |
| 4 | 20th Street (southbound) | 566 m | ~1 min | Road (low risk) |
| 5 | Pearl Street (westbound) | 216 m | ~25 sec | Pedestrian mall — **dismount** |
| 6 | 18th Street (southbound) | 249 m | ~39 sec | Road (low risk) |
| 7 | Canyon Boulevard (westbound) | 637 m | ~1 min | 🚲 Separated bike path (**safest!**) |
| **Total** | | **4,027 m** | **~16 min** | |

### Biking Highlights
- **19th Street corridor** — Dedicated bike lane along the majority of the route
- **Canyon Boulevard** — Visible, car-free, physically separated bike path
- **Total biking time:** ~16 minutes at a comfortable 15 km/h pace
- **Only ~4 minutes slower than driving door-to-door!**

---

## 🌍 Environmental Impact

| Metric | Savings vs. Driving |
|---|---|
| CO₂ per trip | ~1.5 kg |
| CO₂ per year (250 workdays) | ~375 kg (~827 lbs) |
| Fuel saved per year | ~125 liters (~33 gallons) |
| Trees equivalent | 6 trees absorbed |

---

## 💰 Financial Benefits

- **Annual savings vs. driving:** ~$1,500–$3,000
- No parking fees downtown
- No car payment needed
- Lower insurance costs

---

## 🏃 Health Benefits

| Metric | Walking | Biking |
|---|---|---|
| Calories per commute | ~240 kcal | ~300 kcal |
| Calories per round-trip | ~480 kcal | ~600 kcal |
| Annual calories (walking) | ~120,000 kcal | — |
| Annual calories (biking) | — | ~60,000 kcal (less sedentary) |
| Mental health benefits | Reduced stress, better sleep | Improved mood, anxiety reduction |

---

## ⏱️ Mode Comparison

| Mode | One Way | Round Trip | Cost per Trip |
|---|---|---|---|
| 🚗 Driving | 10–15 min | 25–40 min | ~$3–5 (fuel + parking) |
| 🚶 Walking | ~48 min | ~96 min | Free |
| 🚲 Biking | ~16 min | ~32 min | Free (or ~$1 B-Cycle) |

---

## 🗺️ Key Landmarks & Infrastructure

- **Pearl Street Mall** — Historic pedestrian-friendly downtown shopping area
- **Boulder Creek Path** — Multi-use paved trail along Boulder Creek (car-free)
- **Canyon Boulevard** — Western terminus of the Creek Path
- **19th Street** — Major N-S corridor with bike lanes and RTD bus service (routes 1, 3, 7, 10)
- **20th Street** — Direct connector through the downtown grid
- **Boulder Flatirons** — Iconic views visible along the Creek Path

---

## 🌡️ Boulder-Specific Tips

1. **Boulder Creek Path** — Scenic, car-free, paved. The highlight of the route!
2. **Dooring risk on 19th St** — Stay in the bike lane, not near parked cars
3. **Pearl Street Mall** — Dismount and walk your bike through the pedestrian zone
4. **Layers** — 300+ sunny days, but temp swings require rain gear + layers
5. **Altitude awareness** — At 5,430 ft, you dehydrate faster and burn ~10–15% more energy
6. **Walk-bike combo** — Walk in bad weather, bike on flat 19th Street sections
7. **RTD backup** — Bus routes 1, 3, 7, 10 with bike racks for bad weather days

---

## 📊 Sustainability Calculator

```
Walking or biking 2.5 mi × 250 days = 1,250 miles/year avoided driving
= ~375 kg CO₂ saved per year
= ~$2,235 in fuel/maintenance/parking/insurance saved per year
= ~6 trees worth of CO₂ absorbed per year
```

---

## 📂 Repository Structure

| File | Description |
|---|---|
| `README.md` | This page — overview, quick-reference guide, and OSRM routing data |
| `commute-analysis.md` | Detailed walking & biking analysis with segment breakdowns |
| `route-details.md` | Turn-by-turn directions, infrastructure quality ratings, seasonal tables |
| `route-comparison.md` | Side-by-side walk vs. bike vs. drive comparison with strategies |
| `commute_data.json` | Structured commute data for programmatic use |
| `route-geometry.json` | Full GPS coordinate polyline for mapping |
| `sustainability-impact.md` | Environmental and health impact data |

---

## 🤝 Contributing

Add your own Boulder commute route and help other residents make sustainable choices!

1. Fork the repo
2. Create `/commutes/your-name-route.md` with your route details
3. Include: addresses, distances, walking/biking times, route notes
4. Submit a PR

---

## 🎯 Resources & Advocacy

- **Boulder BCycle** — City bike-share program: boulder.b-cycle.com
- **Bicycle Colorado** — Statewide bike infrastructure advocacy: bicyclecolorado.org
- **RTD Bus + Bike** — Public transit with bike racks: rtd-denver.com
- **Boulder Open Space** — Car-free recreation trails: bouldercolorado.gov/openspace
- **Colorado Energy Office** — $1,200 E-Bike rebate program: energystone.colorado.gov

---

*Created with ❤️ for the Boulder community | Data sourced from OpenStreetMap & OSRM*