# Data Sources & Methodology

## Geocoding

| Location | Address | Latitude | Longitude | Source |
|----------|---------|----------|-----------|--------|
| Home | 45 Oak Avenue, Boulder, CO 80304 | 40.0448805 | -105.2738879 | OpenStreetMap (Nominatim) |
| Work | 1800 Broadway, Boulder, CO 80302 | 40.0163281 | -105.2789726 | OpenStreetMap (Nominatim) |

## Route Data

- **Routing Engine**: OSRM (Open Source Routing Machine)
- **Walking Mode**: Foot routing with pedestrian-optimized paths
- **Biking Mode**: Bicycle routing with bike-friendly road selection
- **Data Source**: OpenStreetMap (live, community-maintained)

## Neighborhood Analysis

- **Tool**: OSM Neighborhood Analysis (custom)
- **Categories Analyzed**: Walkability, Groceries, Restaurants, Healthcare, Education, Public Transport, Parks, Sports, Entertainment, Shopping, Services
- **Search Radius**: 1000m from each point
- **Metrics**: Count, average distance, minimum distance for each category

## Commute Analysis

- **Tool**: OSM Commute Analysis Engine
- **Modes Compared**: Foot, Bicycle
- **Parameters**: Distance, Duration, Route Segments, Turn-by-Turn Directions
- **Elevation**: Simple elevation profile from OpenStreetMap contour data

## CO₂ Calculations

- **Average car emissions**: ~0.2 kg CO₂ per km (source: EPA)
- **Round trip**: 4 km × 2 = 8 km daily
- **Annual (250 workdays)**: 8 km × 250 = 2000 km → ~400 kg CO₂
- **One-way savings**: ~0.8 kg CO₂ per trip (4 km avoided)

## How to Replicate

Researchers and fellow Boulder residents can replicate this analysis:

1. **Geocode your addresses**: Use OpenStreetMap Nominatim API or geocode.address
2. **Calculate routes**: Use OSRM (http://router.project-osrm.org) or similar
3. **Analyze neighborhoods**: Use OSM Overpass API queries for amenities
4. **Compare CO₂**: Use EPA emission factors or similar databases

## Tools & APIs Used

| Tool | Purpose | URL |
|------|---------|-----|
| OpenStreetMap | Base map data | https://www.openstreetmap.org |
| Nominatim | Geocoding | https://nominatim.openstreetmap.org |
| OSRM | Routing engine | http://project-osrm.org |
| Overpass API | OSM data query | https://overpass-turbo.eu |

---

*All data is from OpenStreetMap and is available under the ODbL license. Always verify current conditions independently.*
