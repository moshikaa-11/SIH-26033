# Smart India Hackathon Workshop
# Date:30.10.26
## Reference Number:26000027
## Name:Moshikaa Suresh

## Problem Title
SIH 26033:Multiple intermediaries reduce farmers earnings and increase consumer prices.

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
HarvestLoop is a digital marketplace that connects farmers and Farmer Producer Organisations (FPOs) with households, apartment communities, restaurants, hostels and bulk buyers.
Its core innovation is a “Harvest Circle”: a group of nearby buyers whose orders are combined into one economical delivery trip.

Farmers list available produce, expected harvest dates, quantities and their minimum acceptable earnings after deductions. Buyers specify quantities, acceptable quality grades and delivery windows.

The platform matches these requirements and calculates the complete delivery cost. An order group becomes ready for confirmation only when:

Farmers receive at least their agreed minimum net price.

Buyers remain within their maximum delivered price.

Enough orders exist to make the delivery trip financially viable.

Vehicle capacity, produce compatibility and delivery deadlines are satisfied.

If these conditions cannot be met, the platform offers another delivery window or collection point. It does not silently reduce the farmer’s earnings.

What makes HarvestLoop distinctive:

A. Demand before dispatch
Confirmed orders are clearly separated from AI demand predictions. Farmers can see what is actually booked before committing produce for dispatch.

B. A visible “Rupee Receipt”
Every order displays the farmer payment, sorting and packaging cost, transport charge and platform fee. Buyers can see how much of their payment reaches the farmer.

C. Flexible delivery rewards
Buyers who choose a shared collection point or a wider delivery window receive a lower delivery charge when those choices create real savings.

D. Harvest rescue matching
If a buyer cancels or surplus remains, the platform suggests nearby alternative buyers whose requirements match the produce. For example, a restaurant may accept ripe tomatoes that a household does not prefer, provided they remain safe and meet agreed quality standards.

E. Small-farmer participation
Several farmers can fulfil one bulk order through an FPO, with contribution tracking and separate payment records.

## Technical Approach
User interface:React progressive web app for farmers, buyers and transporters

Backend:Python with Django REST Framework

Database:PostgreSQL with PostGIS for orders and location matching

Demand forecasting:A baseline forecast followed by XGBoost when sufficient historical data exists

Delivery planning:Google OR-Tools for constrained vehicle routing

Traceability:QR codes linked to harvest date, farmer/FPO, weight and quality records

Payments:Payment-provider sandbox for the prototype; supported settlement services for deployment

## Feasibility and Viability
Begin with one FPO, a limited delivery area, three vegetables, a few institutional buyers and scheduled delivery days.

Use existing FPO collection facilities and local transport partners. This reduces the initial need for owned warehouses and vehicles.

Revenue model

Charge a transparent service fee on completed transactions. Offer an optional subscription for institutional buyers requiring recurring procurement and reporting. Include all operating costs when checking whether a delivery is viable.

## Impact and Benefits

For farmers: Better visibility of confirmed demand, stronger control over minimum net earnings and access to pooled bulk orders.

For consumers: Transparent pricing and opportunities to reduce delivery charges through neighbourhood ordering.

For FPOs: Tools to coordinate farmer contributions, collection, quality records and payments.

For transporters: Better-planned trips and opportunities to carry fuller loads.

For the environment: Potential reductions in unnecessary trips and unsold produce, to be measured during the pilot.

How impact will be measured

Farmer net earnings per kilogram after deductions.

Buyer price per kilogram, including delivery.

Logistics cost per kilogram delivered.

Percentage of produce remaining unsold or spoiled.

Vehicle capacity utilization and on-time delivery.

Platform contribution margin after variable costs.

Compare results against existing purchasing and selling channels for similar produce, quality, location and dates. Any percentage improvement will be reported only after testing.

## Research and References

e-NAM: FPO participation — Explains aggregation and collective selling. Use this to establish existing capabilities and explain your additional coordination mechanism.FPOs

Government announcement: e-NAM FPO and logistics modules — Supports the relevance of trading from collection centres and transport coordination. Press Information Bureau

FAO: Food Loss and Waste Platform — Provides background on measuring and reducing supply-chain losses. fao.org

Google: Route Optimization overview — Illustrates routing constraints such as vehicle capacity, time windows and shipment compatibility. This is a technical reference, not evidence that HarvestLoop has achieved savings.
