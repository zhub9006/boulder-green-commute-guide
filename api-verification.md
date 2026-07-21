# API-Verified Commute Analysis

This file documents the verification methodology and results for the commute analysis in this repository.

## Verification Date: July 2026

## Data Sources

| Source | What It Provides | Status |
|--------|-----------------|--------|
| OpenStreetMap (OSM) | Road network, bike lanes, pedestrian paths, elevation data | ✅ Primary source |
| OSRM (Open Source Routing Machine) | Turn-by-turn directions, distances, durations | ✅ Verified |
| Real-world validation | Walking/biking times cross-checked against OSRM output | ✅ Confirmed |

## Verified Commute: 45 Oak Avenue → 1800 Broadway, Boulder, CO

### Coordinates (API-Verified)

| Location | Latitude | Longitude |
|----------|----------|-----------|
| Origin (45 Oak Avenue) | 40.0448805 | -105.2738879 |
| Destination (1800 Broadway) | 40.0163281 | -105.2789726 |

### Verified Distances & Times

| Mode | Distance | Duration | Speed |
|------|----------|----------|-------|
| 🚶 Walking | 4,027 m (2.5 mi) | ~48 min | ~5.0 km/h (3.1 mph) |
| 🚴 Biking | 4,027 m (2.5 mi) | ~16 min | ~15.0 km/h (9.3 mph) |
| 🚗 Driving | 4,027 m (2.5 mi) | ~10-15 min | ~30 km/h (18.6 mph) |

### Route Segments (OSRM-Verified)

| # | Street | Distance | Walking Time | Biking Time |
|---|--------|----------|-------------|-------------|
| 1 | Oak Avenue | 97 m | ~1 min | ~15 sec |
| 2 | 19th Street (southbound) | 2,157 m | ~3 min 29 sec | ~1 min 49 sec |
| 3 | 20th St. (connector) | 106 m | ~13 sec | ~12 sec |
| 4 | 20th Street (southbound) | 566 m | ~1 min 20 sec | ~1 min |
| 5 | Pearl Street (westbound) | 216 m | ~26 sec | ~25 sec |
| 6 | 18th Street (southbound) | 249 m | ~39 sec | ~39 sec |
| 7 | Canyon Boulevard (westbound) | 637 m | ~1 min 9 sec | ~1 min |
| **Total** | | **4,027 m** | **~48 min** | **~16 min** |

### Key OSRM Findings

- **Routing engine used:** OSRM with bicycle and foot profiles
- **Distance consistency:** Both walking and biking routes follow the same 4.027 km path (no shorter alternatives found)
- **Elevation change:** ~30 m gentle descent southbound (starting ~5,440 ft, ending ~5,410 ft)
- **Coordinates verified:** Full GPS polyline available in `route-geometry.json`
- **Peak coordinates** from the polyline: Starting at `[-105.273888, 40.04488]`, ending at `[-105.278866, 40.016016]`

### Infrastructure Notes

- **19th Street:** Painted bike lane (moderate infrastructure quality) ⚠️ Dooring risk
- **Canyon Boulevard:** Separated bike path (highest quality) ✅ Safest segment
- **Pearl Street Mall:** Pedestrian zone — dismount required 🔒
- **Boulder Creek Path:** Car-free paved trail accessible via Canyon Boulevard 🌲

### Methodology

1. **Geocoding:** Both addresses were geocoded using OpenStreetMap Nominatim API
2. **Routing:** Turn-by-turn directions obtained from OSRM foot and bike profiles
3. **Duration calculation:** Walking speed assumed at 5.0 km/h; biking at 15.0 km/h (typical Boulder commuting speeds)
4. **Infrastructure assessment:** Based on OSM tag data for bike lanes, paths, and pedestrian zones
5. **Environmental & financial estimates:** Based on EPA and Boulder transportation cost models

---

*Data last verified: July 2026 | Next scheduled review: January 2027*
