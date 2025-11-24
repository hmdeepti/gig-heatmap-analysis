# gig-heatmap-analysis
Gig Heat Map Analysis (DailyGo)

This project visualizes worker density, gig activity and no-show hotspots
using Kepler.gl. The goal was to help the operations team understand where
worker supply was strong, where events were concentrated, and which areas
tended to have higher no-shows.

What we visualized
------------------
1. Worker Density Heat Map
   Helps identify areas where most workers are active. This was useful for
   planning events and understanding supply availability.

2. Gig Locations
   Gigs are displayed as individual points. Larger events appear clearly,
   making it easier for the ops team to see workload distribution.

3. No-Show Hotspots
   Using a simple cluster view, we identify locations where worker no-shows
   occurred more often. This helped event managers plan backup staffing.

4. Time Controls
   The notebook supports time filtering to check activity by hour/shift.

How to use
----------
1. Install requirements
2. Open `notebooks/heatmap_kepler.ipynb`
3. Run the last cell to launch Kepler visualization
4. Export HTML from Kepler (File → Export → HTML)

Files
-----
- workers_geo.csv: Worker locations from app check-ins
- gigs_geo.csv: Event locations and worker counts
- no_show_history.csv: No-show data with shift info
