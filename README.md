# Smart India Hackathon Workshop
# Date:29/10/2026
## Reference Number:26012214
## Name: DARREN JENKIN P 

## Problem Title
SIH 26033: Multiple intermediaries reduce farmers earnings and increase consumer prices.

## Problem Creater's Organization
Ministry of Consumer Affairs, Food & Public Distribution

## Theme
Agriculture, FoodTech & Rural Development

## Problem Description
Expected Solution: Create a digital marketplace that:

• Connects farmers/FPOs directly with consumers and bulk buyers.
• Provides logistics support.
• Uses AI for demand forecasting and route optimization.

Benefits:

• Better prices for farmers.
• Lower prices for consumers.
• Reduced supply chain inefficiencies.

## Proposed Solution
1. Detailed explanation of the proposed solution

FloodSafe has four connected workspaces: a public alert feed, a resident report form, an operations map for authorized staff, and a shelter and route directory. Public feeds provide rainfall or warning context; trained staff can add verified field updates; residents can report water on roads, blocked drains or urgent needs with a location and optional photo.  

2. How it addresses the problem

The system groups reports by place and time, highlights areas with multiple recent signals, and allows an authorized operator to publish a neighborhood advisory. Each advisory includes what changed, when it was updated, what residents should do, and where to get help. Route and shelter status can be updated manually during the prototype, preserving human review where local conditions change quickly.

3. Innovation and proposed workflow
FloodSafe focuses on making local information actionable and auditable. Instead of treating every incoming report as confirmed, it separates raw observations, verified updates and official warnings. The interface shows the source and time for each item, helping users judge whether information is current.
 
Distinctive elements:
 1.Neighborhood-level alert cards that explain the change and a recommended action.  
 2.A triage queue that prioritizes reports by recency, location, severity and verification status.  
 3.A shelter directory with accessibility notes, contact details and last-confirmed status.  
 4.Route advisories that can be updated or withdrawn by authorized staff.  
 5.Low-bandwidth pages and SMS-ready alert text for users with limited connectivity.  
 
FloodSafe response workflow:

<img width="1800" height="900" alt="FloodSafe_Workflow" src="https://github.com/user-attachments/assets/033b0891-085f-4a2a-88de-76b7ac507a43" />
 
Example user journey:

Resident: receives a locality alert, checks the timestamp and recommended action, then opens the nearest confirmed shelter details.  
Ward operator: reviews a new waterlogging report, checks nearby reports and official inputs, marks it verified or unverified, and publishes an advisory if needed. 
Responder: reviews priority locations and shelter status, then updates the operational view as conditions change.

## Technical Approach
1. Technologies to be used

Frontend: responsive web app (HTML, CSS and JavaScript or React). Backend: Python with FastAPI or Django REST. Database: PostgreSQL with PostGIS for location queries. SQLite can support an offline demo. Map display: OpenStreetMap-based tiles subject to file service terms. Notifications: in-app first, with SMS-gateway integration only if available and approved. Authentication: role-based access for operator and administrator functions.

2. Methodology and process

 1.Define roles: resident, ward operator, responder and administrator.  
 2.Create sample neighborhoods, shelters, hazard reports and alert records.  
 3.Build report intake with coordinates, time, category, description and optional image.  
 4.Add operator review controls for verification, duplicate linking and status changes.  
 5.Display a map and list view with filters for time, category and verification state.  
 6.Publish an alert template with locality, source, issue time, action and expiry/review time.  
 7.Add shelter details and manually maintained route status for the demo.  
 8.Test permissions, stale-data handling, low-bandwidth behavior and accessibility.  
 
Proposed system architecture

<img width="1500" height="1500" alt="FloodSafe_System_Architecture" src="https://github.com/user-attachments/assets/29c1e75a-dc44-47d9-80da-30666a6b053b" />


## Feasibility and Viability
1. Analysis of the feasibility of the idea

A hackathon prototype can be built with open-source web and database tools and a small, simulated dataset. The first demonstration can use manually entered warnings and reports, so it does not depend on access to live government systems. A map, report queue, alert composer and shelter directory are enough to demonstrate the main workflow.

2. Potential challenges and risks

 1.Reports may be inaccurate, duplicated or deliberately misleading.  
 2.Network or power outages may prevent timely updates.  
 3.A route or shelter can become unsafe after it was last checked.  
 4.Location and contact information can expose residents to privacy risks.  
 5.Official data feeds, SMS services and mapping services may have access or usage limits.  
 6.Users may interpret an estimated risk indicator as an official warning.
 
3. Strategies for overcoming these challenges

Keep official alerts visually distinct from community reports. Show source and last-updated time; expire stale statuses and request re-confirmation. Require authorized review before publishing operational guidance. Minimize collection of personal information, restrict access to sensitive reports and define retention rules. Provide a phone/SMS fallback plan and printable shelter information. Test the workflow with local responders before any real deployment.

## Impact and Benefits
1. Potential impact on the target audience

Residents could receive clearer locality-specific information. Ward teams may gain a common queue for incoming observations, while responders can see the latest verified shelter and route information in one view. The benefits depend on reliable data, connectivity, training and coordination with the responsible authorities; the prototype alone cannot establish real-world impact.

2. Benefits of the solution

Track time from report submission to review, share of reports with a resolved status, alert delivery success, age of shelter and route updates, and task completion in user walkthroughs. Compare results against a defined baseline and include feedback from residents with different accessibility and connectivity needs.

## Research and References
1. Details / Links of the reference and research work

The following primary resources can inform a later implementation. Confirm the applicable local authority, data availability, permissions and current guidance before deployment.  
India Meteorological Department — official weather forecasts and warnings: https://mausam.imd.gov.in  
Central Water Commission — flood forecasting services and information: https://cwc.gov.in  
National Disaster Management Authority — disaster management guidance: https://ndma.gov.in  
OpenStreetMap — map data and usage guidance: https://www.openstreetmap.org  
PostGIS — spatial database documentation: https://postgis.net/documentation/  
Smart India Hackathon — official program information and challenge content: https://www.sih.gov.in
