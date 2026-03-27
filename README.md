coverage-map
Interactive coverage map for Service Partners showing technician and electrician locations, service radius, and pricing.

EVPassport Coverage Map
This repository hosts a lightweight, browser-based coverage map used to visualize Service Partner resources (Technicians and Electricians), their coverage radius, and whether a specific job address is within coverage.

The map is hosted using GitHub Pages and reads data directly from data.csv in this repository.

How to use the map
Open the live map (GitHub Pages).
Use the filters at the top:
Service Partner
State
Role (Technician / Electrician)
Enter a Job address and press Enter (or click Check coverage).
Review:
Eligible resources inside radius (sorted by nearest)
If none are eligible, the nearest outside-radius resources (capped at 250 miles)
Updating coverage data
All map data is stored in data.csv.

Process
Open data.csv in GitHub.
Click Edit (pencil icon).
Add or update rows.
Commit changes to main.
Refresh the live map page to load the latest data.
Required fields (minimum)
partner
role (Technician or Electrician)
lat
lon
active (TRUE/FALSE)
Recommended fields
state (2-letter code, e.g., TX)
name
service_radius_miles
price
notes
Exporting results
Current export approach:

Run a job search
Copy the results list from the sidebar into email/notes
Planned enhancement (optional next step):

Add an Export CSV button to download eligible results for the searched job address.
