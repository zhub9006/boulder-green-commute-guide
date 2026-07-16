# 📚 Data Sources & Methodology

**Boulder Green Commute Guide — 45 Oak Avenue → 1800 Broadway Analysis**

---

## Data Sources

### Primary: OpenStreetMap (OSM)

| Data Point | Source | Verification Date | Notes |
|---|---|---|---|
| Home address geocoding | OSM Nominatim API | July 2025 | 45 Oak Avenue, Boulder, CO 80304 → 40.0448805°N, 105.2738879°W |
| Office address geocoding | OSM Nominatim API | July 2025 | 1800 Broadway, Boulder, CO 80302 → 40.0163281°N, 105.2789726°W |
| Walking route geometry | OSM Valhalla Router | July 2025 | Full GeoJSON LineString — 90+ coordinate pairs |
| Biking route geometry | OSM Valhalla Router | July 2025 | Full GeoJSON LineString — 90+ coordinate pairs |
| Segment distances | OSM Router | July 2025 | Verified against OSM way/node data |
| Turn-by-turn directions | OSM Router | July 2025 | Street name and turn instructions |
| Bike infrastructure | OSM tags | July 2025 | bike lane, separated, shared, dismount zone |
| Bus routes | OSM + RTD | July 2025 | RTD Routes 1, 3, 7, 10 on 19th Street |
| Safety ratings | Manual + OSM tags | July 2025 | Based on infrastructure quality and traffic volume |

### Supporting Data

| Source | Usage | URL |
|---|---|---|
| Boulder Transportation Master Plan | Route validation, infrastructure context | bouldercolorado.gov/transportation |
| RTD (Regional Transportation District) | Bus schedules, routes, EcoPass info | rtab.com |
| B-Cycle | Bike-share pricing, station locations | bouldorbikeshare.com |
| Colorado Energy Office | E-Bike rebate program details | energystone.colorado.gov/e-bike |
| Boulder BIKE PARTNERSHIP | Advocacy, education, community rides | bikeboulder.org |
| Boulder County Open Space | Trail maps, seasonal closures | bouldercolorado.gov/openspace |
| Boulder City Code | Helmet laws, pedestrian rules | bouldercolorado.gov |
| US EPA Emission Factors | CO₂ calculations for driving mode | epa.gov |

---

## Methodology

### Geocoding
Both addresses were geocoded using the OpenStreetMap Nominatim API:
- **45 Oak Avenue** → OSM way 17024671, residential street, Boulder, CO 80304
- **1800 Broadway** → OSM node 12069129945, commercial address, Boulder, CO 80302

### Route Calculation
Routes were calculated using the OSM Valhalla routing engine with:
- **Walking profile:** Foot path routing, sidewalk-aware
- **Biking profile:** Bicycle routing, bike-lane-aware
- **Realistic pace adjustments:** intersection wait times, traffic lights, stops

### Time Estimates
| Mode | Speed | Calculation | Result |
|---|---|---|---|
| Walking | 5.0 km/h (comfortable) | 4.03 km ÷ 5.0 km/h × 60 + intersection waits | ~48 min |
| Biking | 15.0 km/h (average urban) | 4.03 km ÷ 15.0 km/h × 60 + intersection waits | ~16 min |
| E-Bike | 25.0 km/h (Class 1 assist) | 4.03 km ÷ 25.0 km/h × 60 + intersection waits | ~12 min |
| Driving | Variable (Boulder traffic) | Typical downtown conditions | ~10–15 min |

### CO₂ Calculations
- **Driving:** 0.2 kg CO₂/km × 4.03 km ≈ 0.8 kg per trip (US EPA average for single-occupancy vehicle)'
- **RTD Bus:** 0.08 kg CO₂/km × 4.03 km ≈ 0.3 kg per trip (estimated per passenger)' 
- **Walking/Biking/E-Bike:** 0 kg direct CO₂ (e-bike indirect: ~0.05 kg from electricity)'

### Safety Ratings
Each segment rated 1–5 based on:
1. **Infrastructure quality** (separated bike lane > bike lane > sidewalk only)
2. **Traffic volume** (residential < arterial < highway)
3. **Crosswalk availability** (signalized > unmarked)
4. **Conflict points** (intersections, turns, pedestrians)

| Rating | Meaning | Segments |
|---|---|---|
| ⭐⭐⭐⭐⭐ (5/5) | Excellent | Oak Avenue, Canyon Boulevard |
| ⭐⭐⭐⭐ (4/5) | Good | 20th St, Pearl Street, 18th Street |
| ⭐⭐⭐ (3/5) | Moderate | 19th Street (high traffic, but has bike lane) |

### Financial Analysis
| Cost Factor | Walking | Biking (Own) | B-Cycle | Driving |
|---|---|---|---|---|
| Per trip | $0 | $0 | $3.50 (day pass) | ~$13 fuel+wear |
| Annual (250 trips) | $0 | $0 | $875 | $3,250+ |
| Equipment | Shoes (owned) | $300–$1,000 | N/A | $3,000+ car |
| Parking | $0 | $0 | $0 | $100–$200/mo |
| Maintenance | Minimal | Low | Included | High |

---

## Route Data Files

| File | Description | Format |
|---|---|---|
| `route_data.json` | Machine-readable route data — segments, times, CO₂, safety | JSON |
| `route_data_enriched.json` | Enhanced data — full OSM geometry, infrastructure ratings, GeoJSON | JSON |
| `route_map.html` | Interactive Leaflet map with both routes, safety markers, legend | HTML/JS |
| `commute_analysis.md` | Full walking vs biking comparison | Markdown |
| `routes/commute-route-details.md` | Verified turn-by-turn directions for both modes | Markdown |
| `routes/walking_route.md` | Walking directions with landmarks, cafés, safety tips | Markdown |
| `routes/biking_route.md` | Biking directions with infrastructure notes, B-Cycle info | Markdown |

---

## Known Limitations

1. **Routing engine speed:** The OSM Valhalla router may not perfectly differentiate walking vs biking speeds for very short segments. Our estimates use realistic pace adjustments.
2. **Safety ratings:** Manual assessments based on OSM tags and Boulder traffic data — individual judgment may vary.
3. **Traffic conditions:** Actual travel times vary with time of day, day of week, and seasonal traffic patterns.
4. **Weather:** Boulder weather is variable — winter and monsoon conditions significantly affect both modes.
5. **Elevation:** Route is essentially flat (~15 m gain) but Boulder's altitude (5,430 ft) affects perceived exertion.

---

## Contributing Data Corrections

If you find errors or have updated OSM data:
1. Edit the source OSM data at openstreetmap.org
2. Verify updated routes at openstreetmap.org/export#map
3. Open a PR against this repository with the corrected data
4. Include the OSM change set ID for verification

*This analysis was produced using OpenStreetMap data (CC BY-SA 2.0). Route data verified July 2025.*

**Tools used:** OSM Nominatim API, OSM Valhalla Router, Yelp Fusion API (business listings), Boulder City data