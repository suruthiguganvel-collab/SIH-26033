# Smart India Hackathon Workshop
# Date:29/10/2026
## Reference Number:26019481
## Name: SURUTHI G S

## Problem Title
SIH 26033: Multiple intermediaries reduce farmers earnings and increase consumer prices.
AI-Assisted Direct Farm-to-Buyer Marketplace With Shared Logistics
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
   
   FarmBridge SmartTrade is a digital marketplace concept that connects farmers and Farmer Producer Organisations (FPOs) directly with households, retailers, restaurants and bulk buyers. Farmers can list available produce, quantity, expected harvest date, quality grade and pickup location. Buyers can compare listings, place orders and choose retail or bulk quantities. The platform shows a transparent price breakdown, including the farmer's listed price, any platform charge and estimated delivery cost.
Its key differentiator is a Group Basket and Shared Logistics feature. Nearby buyers can combine compatible orders, while nearby farmers can coordinate available produce and collection windows. This can help consolidate deliveries and reduce avoidable transport costs. An AI-assisted demand module estimates likely demand from historical orders and seasonal patterns, while route planning groups deliveries by location and time. These recommendations support decision-making; users can review and override them.

2. How it addresses the problem
   
Direct listings give farmers and FPOs a digital route to reach buyers without depending entirely on several intermediaries. Transparent prices help buyers compare options and understand charges. Group orders and pooled transport may reduce per-order logistics costs. Demand forecasts can help farmers and buyers plan quantities and reduce mismatches between supply and demand. Order status, delivery updates and buyer feedback improve traceability and trust.

3. Innovation and uniqueness of the solution
Unlike a simple listing-only marketplace, FarmBridge combines four connected functions:
Group purchasing for compatible buyer orders.
Pooled pickup and delivery planning.
Explainable demand estimates using available order history and seasonality.
Transparent price and delivery breakdowns.
The platform also supports farmer/FPO profiles, quality and harvest details, order status and feedback. The innovation claim should be checked against existing platforms and refined after team research; do not claim that no similar system exists.

<img width="1500" height="430" alt="WhatsApp Image 2026-10-30 at 2 16 10 PM" src="https://github.com/user-attachments/assets/810907be-e072-4f21-9ef3-a28c6854a68c" />

<img width="1536" height="1024" alt="sih" src="https://github.com/user-attachments/assets/d1b86b57-3631-40c5-a3ce-40361ffe6e8b" />


## Technical Approach
1. Technologies to be used
   
Frontend: HTML, CSS and JavaScript for a responsive interface.
Backend: Python with Django or Flask to manage listings, orders, users and APIs.
Database: SQLite for a small prototype; PostgreSQL for a larger deployment.
Demand forecasting: Begin with simple baseline methods using historical order counts and seasonal patterns. Evaluate machine-learning models only if enough suitable data is available.
Route planning: Use map/distance data and a routing service, or demonstrate a simple distance-based batching prototype. Check service terms and costs before integration.
Visualisation: Charts for demand trends, order status and price breakdowns.
Development tools: Git for version control and a test dataset with sample farmers, products and orders.

2. Methodology and process for implementation <b>(Flow Charts/Images/ working prototype)</b>

Define user roles: Farmer/FPO, buyer and administrator.
Create produce listings: Include produce name, quantity, price, quality grade, harvest date and pickup area.
Build search and orders: Let buyers filter listings and place sample orders.
Show transparent pricing: Display product price, estimated transport charge and total before order confirmation.
Add Group Basket: Identify compatible orders by delivery area, date and product constraints.
Add demand estimates: Use sample order history to show a basic forecast, clearly labelled as an estimate.
Add route batching: Group delivery points and display a proposed sequence with manual override.
Test the prototype: Check account roles, invalid inputs, order calculations, grouping logic and usability

<img width="1200" height="800" alt="sih 1" src="https://github.com/user-attachments/assets/ab58b702-7734-4a18-96a3-dc400321aabe" />

## Feasibility and Viability
1. Feasibility analysis

The core marketplace can be prototyped with common web technologies and a small database. A team can demonstrate the workflow using sample data without connecting to real payment or logistics providers. Demand forecasting can begin with historical sample orders and seasonal averages. Route batching can begin with approximate distances or a routing service if access is available. Starting with one crop category and a limited local area keeps the initial scope manageable.

2. Potential challenges and risks

Inconsistent product quality, grading and quantity descriptions.
Farmers or buyers may have limited connectivity or digital experience.
Forecasts may be inaccurate when order history is limited or seasons change.
Delivery delays, cancellations and perishable produce can affect trust.
Map, messaging, payment or logistics integrations may have costs or access constraints.
Personal, location and transaction data require appropriate protection.

3. Strategies for overcoming challenges

Use clear listing fields, optional photos and agreed quality labels. Design a mobile-friendly interface with simple language and minimal steps. Mark early forecasts as estimates and show the data period used. Allow manual confirmation of delivery batches and provide order-status updates. Begin with demo payments or a payment simulation rather than handling real payment credentials. Collect only necessary user data, restrict access and test the workflow with representative users.

## Impact and Benefits
1. Potential impact on the target audience

  The primary users are farmers, FPOs, household consumers, retailers, restaurants and bulk buyers. Farmers may gain additional ways to reach buyers; consumers can compare listings and charges; logistics partners can receive more consolidated delivery plans. Administrators can monitor listings, order progress and common service issues. Impact should be evaluated through a small pilot rather than assumed.
2. Benefits 

Economic: Transparent price information and direct buyer access may improve market choices for farmers and buyers.
Operational: Grouped orders and shared transport may lower duplicated trips and delivery effort.
Social: Digital access can help FPOs and small producers reach more customers.
Environmental: Better delivery consolidation may reduce unnecessary travel, depending on actual routes and vehicle use.
Food management: Demand visibility may help users plan quantities and reduce avoidable surplus; this requires validation with real data.
Success measures to test
Track the number of active listings, order completion rate, average delivery cost per order, time from listing to sale, forecast error, cancellation rate and farmer/buyer satisfaction. Compare pilot results with a defined baseline before claiming improvements.

## Research and References
1. Details / Links of the reference and research work
Smart India Hackathon — https://www.sih.gov.in/
Ministry of Agriculture & Farmers Welfare, Government of India — https://agriwelfare.gov.in/
e-NAM (National Agriculture Market) — https://www.enam.gov.in/
OpenStreetMap — https://www.openstreetmap.org/
Django documentation — https://docs.djangoproject.com/
scikit-learn documentation — https://scikit-learn.org/
Food and Agriculture Organization (FAO) — https://www.fao.org/
