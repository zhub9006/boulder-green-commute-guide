# 📊 Data Sources & Methodology

## Data Sources

- **OpenStreetMap (OSM)** — Primary data source for road network, segments, and routing
- **OSM Routing API** — Used to calculate walking and biking directions between locations
- **OSM Geocoding** — Used to convert addresses to geographic coordinates

## Methodology

1. **Geocoding:** Addresses were converted to lat/lon coordinates using OSM geocoding
2. **Routing:** The OSM routing engine calculated optimal paths for both walking and biking modes
3. **Segment Analysis:** Each route was broken down into named street segments with distance and duration
4. **Comparison:** Routes were compared for distance, time, and sustainability impact

## Notes

- Walking and biking routes in Boulder often share the same road infrastructure
- The OSM routing engine may optimize similarly for both modes on shared roads
- Real-world walking times may be longer due to pedestrian-specific routing, signals, and sidewalks
- Real-world biking times may be shorter due to dedicated bike lanes and higher permissible speeds

## Acknowledgments

- OpenStreetMap contributors for maintaining the map data
- The Boulder community for building a walkable, bikeable city
- Boulder Valley School District, University of Colorado, and City of Boulder for supporting sustainable transportation
