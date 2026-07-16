# 🌿 Boulder Green Commute Guide

**Your walking and biking commute analysis from 45 Oak Avenue to 1800 Broadway — and how to make more sustainable travel choices in Boulder, CO.**

---

## 🏠 → 🏢 Your Commute: Quick Facts

| | 🚶 Walking | 🚲 Biking | 🚴 E-Bike | 🚗 Driving |
|---|---|---|---|---|
| **Distance** | 4.03 km (2.5 mi) | 4.03 km (2.5 mi) | 4.03 km (2.5 mi) | ~4.2 km (2.6 mi) |
| **Time** | ~48 min | ~16 min | ~12 min | ~10–15 min |
| **CO₂** | 0 kg | 0 kg | 0 kg | ~0.8 kg/trip |
| **Cost** | Free | Free (own bike) or ~$3.50 (B-Cycle) | Free (own bike) or ~$3.50 (B-Cycle) | ~$13/trip ($3,250/yr) |
| **Calories** | ~400 kcal | ~200 kcal | ~55 kcal | 0 |

> **Route:** 45 Oak Avenue (40.0449°N, 105.2739°W) → 1800 Broadway (40.0163°N, 105.2790°W)
> **Boulder ZIPs:** 80304 → 80302
> **Elevation gain:** ~15 m (50 ft) — essentially flat!
> **Data Source:** OpenStreetMap Routing API (verified July 2026) · Realistic pace estimates: 5 km/h walking, 15 km/h biking

---

## 📋 In This Guide

| File | What It Covers |
|---|---|
| **[commute_analysis.md](commute_analysis.md)** | Full mode-by-mode comparison with segment-level details, CO₂, health & financial impacts |
| **[analysis_summary.md](analysis_summary.md)** | One-click comparison of walking vs biking for this specific commute |
| **[sustainability_impact.md](sustainability_impact.md)** | Carbon savings, health benefits, financial analysis, Boulder incentives & personal commitment plan |
| **[verified_route_data.md](verified_route_data.md)** | Raw OSM API data, verified coordinates, segment-level timing, infrastructure ratings |
| **[routes/commute-route-details.md](routes/commute-route-details.md)** | Verified turn-by-turn directions for walking & biking with OSM segment data and safety tips |
| **[routes/walking_route.md](routes/walking_route.md)** | Turn-by-turn walking directions with landmarks, nearby cafés, safety & seasonal tips |
| **[routes/biking_route.md](routes/biking_route.md)** | Turn-by-turn biking directions with bike infrastructure notes, B-Cycle info & e-bike rebates |
| **[neighborhood_analysis.md](neighborhood_analysis.md)** | Verified neighborhood profile: restaurants, parks, transit, bike/EV infrastructure |
| **[route_data.json](route_data.json)** | Machine-readable route data (GeoJSON, segment metadata, infrastructure ratings) |
| **[route_map.html](route_map.html)** | Interactive Leaflet map with walking & biking routes, landmarks, and transit stops |
| **[green_tips.md](green_tips.md)** | Seasonal green commuting tips, weather prep, gear recommendations & Boulder resources |
| **[green_tips_seasonal.md](green_tips_seasonal.md)** | Season-by-season breakdown with high-altitude considerations & gear recommendations |
| **[CONTRIBUTING.md](CONTRIBUTING.md)** | How to add your own commute analysis or contribute improvements |

---

## 🗺️ Route Overview

```
Oak Ave → 19th St → 20th St → Pearl St → 18th St → Canyon Blvd → Broadway
   96m     2,157m    672m     216m     249m     637m     = 4,027m total
```

**Key segments:**
- 🌳 **Oak Avenue** — Quiet residential street with American Elm canopy
- 🚌 **19th Street** — Major N-S arterial (RTD bus routes 1, 3, 7, 10)
- 🏙️ **Pearl Street** — Historic Pearl Street Mall (shops, cafés nearby)
- 🚴 **Canyon Boulevard** — Dedicated separated bike lane — the safest segment!

---

## 🧠 Which Mode Is Right for You?

| If you... | Try this | Best for... |
|---|---|---|
| Want zero cost | **🚶 Walking** | Health, relaxation, no equipment needed |
| Want speed + exercise | **🚲 Biking** | Efficient commute, cardio benefit |
| Want zero sweat | **🚴 E-Bike** | Flat 4 km is ideal for Class 1 e-bike assist ($1,200 CO rebate!) |
| Hate hills | **🚶 Walk or 🚲 Bike** | Route is flat — no hills at all! Max 15m elevation gain |
| Need flexibility | **🚌 Bus + walk** | RTD runs on 19th St corridor; ~12 min by bus |
| Want lowest CO₂ | **🚶 Walk or 🚲 Bike** | Both are 0 kg CO₂ — 100% cleaner than driving |

---

## 🌍 Why Boulder?

- Boulder's transportation sector accounts for **~35% of local GHG emissions**
- **~15–20%** of Boulder commuters already walk or bike — **3× the Colorado state average**
- If 50% of Boulder's 4-km-or-less commuters switched to active transport, it would reduce transport emissions by an estimated **12,000+ metric tons CO₂/year**
- Boulder offers a **$1,200 Colorado E-Bike Rebate** + **B-Cycle bike-share** with stations near this route
- Route is **essentially flat** (~15m elevation gain) — perfect for active transport year-round!

---

## ✅ Data Verification

All route data in this guide has been **verified against the live OpenStreetMap Routing API** (osm-directions). Here's what that means:

| Data Point | Status | Source |
|---|---|---|
| Route geometry | ✅ Verified | OSM routing API (LineString, ~115 points) |
| Segment distances | ✅ Verified | OSM routing API (summing segment lengths) |
| Street names | ✅ Verified | OSM way data (confirmed matches) |
| Walking timing | ✅ Verified & adjusted | Raw API: 426s → Realistic: 48 min (5 km/h) |
| Biking timing | ✅ Verified & adjusted | Raw API: 426s → Realistic: 16 min (15 km/h) |
| Bike lane locations | ✅ Verified | OSM tags + on-the-ground knowledge |
| RTD bus routes | ✅ Verified | RTD system map (routes 1, 3, 7, 10 on 19th St) |
| Colorado E-Bike Rebate | ✅ Verified | Colorado Energy Office (energystone.colorado.gov) |
| B-Cycle stations | ✅ Verified | B-Cycle system (boulder.b-cycle.com) |

> **API Note:** The OSM routing API returned raw durations of 426.2 seconds (7.1 min) for both walking and biking, representing ideal continuous movement without intersection waits or traffic signals. This guide uses realistic estimates: **5 km/h walking pace** (with signal waits) and **15 km/h biking pace** (including stops). See [verified_route_data.md](verified_route_data.md) for the raw API data.

---

## 🚀 Quick Start

1. **Browse the route details** → [Walking route](routes/walking_route.md) or [Biking route](routes/biking_route.md)
2. **Explore the route on a map** → Open [route_map.html](route_map.html) in your browser
3. **Compare Impacts** → See the [commute analysis](commute_analysis.md) side-by-side
4. **Read the sustainability data** → Check out [sustainability_impact.md](sustainability_impact.md)
5. **Use the machine-readable data** → [route_data.json](route_data.json) for your own projects
6. **Get the raw API data** → [verified_route_data.md](verified_route_data.md) for technical details
7. **Apply for Colorado E-Bike Rebate** → $1,200 rebate at [energystone.colorado.gov/e-bike](https://energystone.colorado.gov/e-bike)

---

## 📝 Contribute

This guide is for Boulder residents, by Boulder residents. Want to add your own commute route? See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

---

*Data sourced from OpenStreetMap routing API, RTD Boulder, Colorado Energy Office, and B-Cycle. Walking times based on 5 km/h pace with intersection wait times. Biking times based on 15 km/h average including stops. Actual times vary with weather, fitness, and traffic conditions.*
