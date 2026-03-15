# SOILE Tourism Data Model

The SOILE platform organizes tourism information into structured offline packages that can be downloaded by tourists and accessed without internet connectivity.

The data model is designed to support remote regions where network access is limited or intermittent.

---

## Core Data Entities

### Route

A tourism route represents a predefined path or travel experience.

Attributes:

• route_id  
• route_name  
• region  
• difficulty_level  
• estimated_duration  
• distance_km  
• route_geometry (GPS track)

Routes contain multiple Points of Interest and navigation waypoints.

---

### Waypoint

Waypoints define navigation points along the route.

Attributes:

• waypoint_id  
• latitude  
• longitude  
• altitude  
• sequence_index  
• waypoint_type

Waypoint types may include:

• navigation point  
• viewpoint  
• safety checkpoint  
• rest location

---

### Point of Interest (POI)

Points of interest provide contextual information along the route.

Attributes:

• poi_id  
• name  
• category  
• description  
• media_assets  
• coordinates

Categories may include:

• natural landmark  
• cultural site  
• historical location  
• environmental feature

---

### Safety Zone

Safety zones define areas where special monitoring or alerts may be triggered.

Attributes:

• zone_id  
• zone_type  
• geographic_boundary  
• safety_instructions  
• monitoring_enabled

---

## Offline Route Package

Tourism data is distributed as downloadable route packages.

Each package may contain:

• route metadata  
• navigation tracks  
• waypoint lists  
• POI descriptions  
• maps and tiles  
• safety instructions  
• multimedia content

Packages are cached locally on the tourist device.

---

## Synchronization Model

SOILE operates in an offline-first mode.

Data synchronization occurs when connectivity becomes available.

Possible updates include:

• route corrections  
• safety alerts  
• tourism content updates  
• infrastructure notifications

---

## Edge Integration

When edge intelligence nodes are present along a route, the data model may interact with local services.

Examples:

• environmental monitoring data  
• safety event alerts  
• local sensor information

Edge nodes may enrich route data without requiring constant cloud connectivity.
