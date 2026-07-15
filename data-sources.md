# Data Sources & Methodology

This guide was built using verified OpenStreetMap data and live routing analysis. Here's how we ensure accuracy.

---

## Primary Data Sources

### OpenStreetMap (OSM)
- **Routing Engine:** OSRM (Open Source Routing Machine) — the same engine powering many commercial map services
- **Data License:** ODbL 1.0 (Open Database License)
- **Last Verified:** July 2025
- **Coverage:** All streets, bike lanes, sidewalks, transit stops, and amenities within the route corridor were verified against live OSM data

### Coordinate Data
- **45 Oak Avenue:** 40.0449°N, 105.2739°W (verified via OSM geocoding)
- **1800 Broadway:** 40.0163°N, 105.2790°W (verified via OSM geocoding)
- **ZIP Codes:** 80304 (origin) → 80302 (destination)

---

## Pace Estimates Methodology

The OSM routing engine returns raw durations tuned for vehicular traffic, which are unrealistic for walking and biking. Our methodology:

| Mode | Raw OSM Duration | Our Adjusted Estimate | Basis |
|---|---|---|---|
| Walking | ~426s (7.1 min) | **~48 min** | 5 km/h comfortable pace incl. intersections |
| Biking | ~426s (7.1 min) | **~16 min** | 15 km/h average pace in urban settings |

### Adjustment Factors
- **Walking:** 5 km/h = 83 m/min, includes intersection delays, search time, and fatigue recovery
- **Biking:** 15 km/h = 250 m/min, includes intersection delays and cautious approach at busy segments
- **Elevation:** ~15 m gain over 4 km — essentially flat; no hill factor applied

---

## CO₂ Estimates

| Source | Value | Notes |
|---|---|---|
| Walking/Biking | 0 kg | Zero emissions |
| Driving (avg car) | ~0.8 kg/trip | EPA average: 404 g CO₂/mile for 2.5 mi → ~1,010 g; adjusted for urban driving conditions |
| Driving (SUV) | ~1.2 kg/trip | Higher for heavier vehicles |
| Bus (RTD) | ~0.3 kg/trip | Average bus emissions per passenger-mile |

## Boulder-Specific Context

- **Transportation emissions:** ~35% of Boulder's GHG (City of Boulder, 2023)
- **Active commute rate:** ~15–20% (Boulder Transportation Master Plan)
- **State comparison:** 3× Colorado average (~5–6%)
- **E-Bike rebate:** $1,200 through Colorado's HB 1281 program
- **B-Cycle:** Denver-Boulder metro bike-share with stations near this route

---

## Toolchain

1. **Geocoding:** OpenStreetMap Nominatim — converts addresses to lat/lon
2. **Routing:** OSRM (foot/bike profiles) — calculates turn-by-turn with distances
3. **Neighborhood Analysis:** OSM Overpass API — amenities, buildings, transit within 1km radius
4. **Reverse Geocoding:** OSM Nominatim — converts coordinates back to addresses for verification
5. **GitHub Publishing:** Automated deployment to public repo for community access

---

## Known Limitations

- OSM data may not reflect real-time conditions (construction, closures)
- Pace estimates are averages; actual times vary by fitness level, weather, and time of day
- Business hours for nearby cafés/shops may have changed since last verification
- Bike lane quality is classified by OSM tags and may have been updated since our analysis

---

*This guide is maintained by volunteers. If you notice outdated information, please open an issue or pull request!*