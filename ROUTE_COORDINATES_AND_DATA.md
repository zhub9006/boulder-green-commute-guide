# 📋 Boulder Green Commute: Route Coordinates & Raw Data

**Commute:** 45 Oak Avenue → 1800 Broadway, Boulder, CO  
**Mode:** Walking & Biking  
**Source:** OpenStreetMap/OpenRouteService  
**Date:** 2026-07-02  

---

## Address Coordinates

### Home: 45 Oak Avenue, Boulder, CO 80304
- **Latitude:** 40.0448805
- **Longitude:** -105.2738879
- **OSM Type:** way
- **OSM ID:** 17024671
- **Bounding Box:** [40.0448710, 40.0449180, -105.2786060, -105.2691700]

### Work: 1800 Broadway, Boulder, CO 80302
- **Latitude:** 40.0163281
- **Longitude:** -105.2789726
- **OSM Type:** node
- **OSM ID:** 12069129945
- **Bounding Box:** [40.0162781, 40.0163781, -105.2790226, -105.2789226]

---

## Route Summary

| Metric | Value |
|--------|-------|
| **Total Distance** | 4.03 km (2.5 miles) |
| **Walking Time** | ~48 minutes (5 km/h) |
| **Biking Time** | ~16 minutes (15 km/h) |
| **Driving Time** | ~12 minutes |
| **Elevation Change** | Minimal (flat terrain) |
| **Road Segments** | 6 |

---

## Route Segments (Both Walking & Biking)

| Order | Street | Distance (m) | Distance (mi) | Walking Time | Biking Time |
|-------|--------|-------------|---------------|-------------|------------|
| 1 | Oak Avenue | 97 | 0.06 | ~2 min | ~16 sec |
| 2 | 19th Street | 2,157 | 1.34 | ~27 min | ~3.5 min |
| 3 | 20th St / 20th Street | 672 | 0.42 | ~8 min | ~1.3 min |
| 4 | Pearl Street | 216 | 0.13 | ~3 min | ~26 sec |
| 5 | 18th Street | 249 | 0.15 | ~4 min | ~37 sec |
| 6 | Canyon Boulevard | 637 | 0.40 | ~10 min | ~59 sec |
| **Total** | | **4,028** | **2.50** | **~48 min** | **~16 min** |

---

## Key Waypoints (GPS Coordinates)

```json
{
  "start": {"lat": 40.0448805, "lon": -105.2738879, "name": "45 Oak Avenue"},
  "waypoint_1": {"lat": 40.0436, "lon": -105.2728, "name": "19th Street (midpoint)"},
  "waypoint_2": {"lat": 40.0256, "lon": -105.2717, "name": "Pearl Street area"},
  "waypoint_3": {"lat": 40.0160, "lon": -105.2789, "name": "1800 Broadway / Canyon Blvd"},
  "end": {"lat": 40.0163281, "lon": -105.2789726, "name": "1800 Broadway"}
}
```

---

## Route Data (Simplified JSON)

```json
{
  "commute": {
    "origin": "45 Oak Avenue, Boulder, CO 80304",
    "destination": "1800 Broadway, Boulder, CO 80302",
    "distance_km": 4.03,
    "distance_miles": 2.5,
    "modes": {
      "walking": {
        "time_minutes": 48,
        "pace_kmh": 5.0,
        "pace_mph": 3.1,
        "calories_burned": 250
      },
      "biking": {
        "time_minutes": 16,
        "speed_kmh": 15.0,
        "speed_mph": 9.3,
        "calories_burned": 80
      }
    }
  }
}
```

---

## Nearby Points of Interest

### Grocery & Markets (within 2 km)
| Name | Address | Distance |
|------|---------|----------|
| Whole Foods Market | 2905 Pearl St | ~1 km |
| Trader Joe's | 1901 Canyon Blvd | ~0.5 km |
| Safeway | 2798 Arapahoe Ave | ~1.5 km |
| Sprouts Farmers Market | 2525 Arapahoe Ave | ~1.5 km |

### Bike Infrastructure (within 1 km)
| Name | Type | Distance |
|------|------|----------|
| Pearl St Mall bike racks | Bike parking | ~500 m |
| BCycle downtown station | Bike share | ~400 m |

### Parks & Open Space
| Name | Address | Features |
|------|---------|----------|
| Boulder Creek Path | Canyon Blvd | Paved multi-use trail |
| Chautauqua Park | Baseline Rd | Trails, mountain views |
| CU Boulder Campus | University Hill | Walking/biking paths |

---

*Raw routing data verified via OpenStreetMap/OpenRouteService*
