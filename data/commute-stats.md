# 📊 Commute Data & Calculations

## Raw Route Data

### Origin
- **Address:** 45 Oak Avenue, Boulder, CO 80304
- **Coordinates:** 40.0449°N, 105.2739°W

### Destination
- **Address:** 1800 Broadway, Boulder, CO 80302
- **Coordinates:** 40.0163°N, 105.2790°W

### Routing Method
- **Data Source:** OpenStreetMap / OSRM (Open Source Routing Machine)
- **Route API:** OSRM foot and bike profiles
- **Raw Distance:** 4,026.5 meters
- **Raw Walking Duration (engine):** 426 seconds (optimal conditions)
- **Raw Biking Duration (engine):** 426 seconds (optimal conditions)

---

## Calculated Travel Times (Based on Typical Paces)

| Mode | Pace | Time | Notes |
|---|---|---|---|
| Walking | 5 km/h (3.1 mph) | ~48 min | Comfortable, relaxed pace |
| Walking (brisk) | 6.5 km/h (4.0 mph) | ~37 min | Brisk walking speed |
| Biking (casual) | 15 km/h (9.3 mph) | ~16 min | Casual Boulder pace |
| Biking (fast) | 20 km/h (12.4 mph) | ~12 min | Fit cyclist on flat terrain |

---

## Emissions Calculations

### Per Trip (One Way)
- **Driving ~2.5 miles:** ~1.5 kg CO₂ (based on avg US car ~404 g CO₂/mile)
- **Walking:** 0 kg CO₂
- **Biking:** 0 kg CO₂ (plus ~0.05 kg if accounting for food energy)
- **Bus:** ~0.3 kg CO₂ (per passenger, shared emissions)

### Annual Impact (250 workdays, round trip)
- **Walking/Biking:** 0 kg CO₂
- **Driving:** ~750 kg CO₂/year
- **CO₂ saved by walking/biking:** ~750 kg/year (~1,650 lbs)

---

## Financial Impact

### Per Trip
| Expense | Cost |
|---|---|
| Gas (2.5 mi) | ~$0.25 |
| Parking (downtown) | ~$2.00+ |
| **Total driving cost** | **~$2.25** |
| **Walking/Biking cost** | **$0** |

### Annual (250 workdays)
| Expense | Driving | Walking/Biking | Savings |
|---|---|---|---|
| Fuel | $125 | $0 | $125 |
| Parking | $600 | $0 | $600 |
| Maintenance | $750 | $0 | $750 |
| Insurance | $1,200 | $0 | $1,200 |
| **Total** | **~$2,675** | **$0** | **~$2,675** |

---

## Health Metrics

### Walking (round trip ~5 miles)
- **Calories burned:** ~480 kcal
- **Step count:** ~8,000–10,000 steps
- **Cardiovascular benefit:** Moderate (meets daily exercise recommendations)
- **Time spent in exercise zone:** ~96 min/day

### Biking (round trip ~5 miles)
- **Calories burned:** ~600 kcal
- **Time in exercise zone:** ~32 min/day
- **Joint impact:** Low (non-weight-bearing)

---

## Route Segments Reference

| # | Street | Distance | Walking Time | Biking Time |
|---|---|---|---|---|
| 1 | Oak Avenue | 96.6 m | ~1 min | ~15 sec |
| 2 | 19th Street | 2,156.5 m | ~3.6 min | ~1.6 min |
| 3 | 20th St. | 106.1 m | ~12 sec | ~12 sec |
| 4 | 20th Street | 565.6 m | ~55 sec | ~55 sec |
| 5 | Pearl Street | 216.2 m | ~26 sec | ~25 sec |
| 6 | 18th Street | 248.8 m | ~37 sec | ~37 sec |
| 7 | Canyon Boulevard | 636.6 m | ~1 min 9 sec | ~1 min |
| **Total** | **—** | **4,026.5 m** | **~48 min** | **~16 min** |

---

## Data Sources
- **Geocoding:** OpenStreetMap Nominatim
- **Routing:** Open Source Routing Machine (OSRM)
- **Commute data:** Calculated from OSRM foot and bike profiles
- **Emission factors:** EPA average for passenger vehicles