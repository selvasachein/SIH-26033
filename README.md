# Smart India Hackathon Workshop
# Date: 30-10-2026
## Reference Number: 26019371
## Name: NARASIMHAN RM

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

# GaonSetu – A Demand-Pooled Direct Farm-to-Consumer Network

**Smart India Hackathon 2026 | Problem Statement Workshop | Problem Code: SIH-26033**

*Theme: Agriculture & Supply Chain | Problem: Multiple intermediaries reduce farmers' earnings and increase consumer prices*

## 1. Problem Understanding

In India, fresh produce typically travels from the farm to the consumer through a long chain: village trader → commission agent (arhtiya) at the mandi → wholesaler → semi-wholesaler → retailer → consumer. A Lok Sabha reply from the Ministry of Agriculture notes that the number of intermediaries in agricultural supply chains ranges from 6 to 8, which lowers the farmer's share of the consumer's rupee and raises the final price.

The root causes are not only "greedy middlemen". They are structural:

- **Information gap:** the farmer does not know the real price in the city market, so the trader sets the price.
- **No guaranteed buyer:** farmers harvest first and look for a buyer later, so they sell at whatever price is offered, especially for perishables.
- **Small lots:** one farmer cannot fill a truck, so aggregation depends on the trader.
- **Delayed and cash-based payment:** farmers are forced to accept lower rates for quick cash.
- **Poor logistics and storage:** high wastage adds to the marketing cost that finally lands on the consumer.

Intermediaries also perform real services (transport, grading, credit, risk-taking). So the aim is not to remove every middleman blindly, but to **replace unnecessary layers with a transparent, low-cost digital and community-run layer.**

## 2. Proposed Solution: GaonSetu

**GaonSetu** ("village bridge") is a mobile and web platform that connects farmers to buyers **before harvest** and moves produce through **Village Collection Points (VCPs)** run by Self-Help Groups (SHGs) or Farmer Producer Organisations (FPOs). Instead of the farmer searching for a buyer after harvest, buyers' demand is pooled first and farmers are matched to it.

**How it works, step by step:**

1. **Demand pooling:** Resident welfare associations, hostels, canteens, small retailers and households place weekly or forward orders (for example, 500 kg tomatoes for Friday).
2. **Farmer listing:** Farmers list expected harvest (crop, quantity, date, village) through a simple voice-enabled, multilingual app or an IVR/WhatsApp number for low-smartphone users.
3. **Matching engine:** The platform matches pooled demand with listed supply based on crop, date, distance and quality grade, and splits the order across several nearby farmers so that small farmers can fill a large order together.
4. **Fair price band:** An AI price engine uses mandi arrival and price data (Agmarknet / e-NAM), weather and seasonality to publish a *fair price band*. The farmer sees the expected market price before agreeing, which removes the information gap.
5. **Collection and grading at VCP:** The SHG operator weighs, grades and records produce. Quality grade and weight are logged in the app, which prevents disputes.
6. **Batched delivery:** A route optimiser groups orders by area and perishability into shared delivery runs (for example, using local pickup vehicles or the existing e-commerce style last-mile partners), which lowers transport cost per kg.
7. **Instant split payment:** The buyer pays through UPI. The platform's settlement logic splits the amount automatically between the farmer, the VCP operator, the transporter and a small platform fee, and the farmer is paid within 24 hours.
8. **Price waterfall for the consumer:** For every order the buyer sees where the money went: *farmer share %, collection, transport, platform fee*. This builds trust and keeps every layer's margin visible and capped.

## 3. What Makes It Different (Uniqueness)

- **Demand-first, not listing-first:** most "direct selling" apps only create a marketplace and hope buyers show up. GaonSetu pools demand in advance so the farmer already has a buyer at the time of harvest.
- **Price Waterfall transparency:** every rupee is traced to its recipient, with margin caps on each service role. This turns the middleman from a hidden price-setter into a visible, paid service provider.
- **Community-run VCPs:** SHG women or FPO members earn a fixed service fee, so the layer between the farmer and consumer stays local and does not become a new profit-maximising intermediary.
- **Works for low-digital-literacy farmers:** voice, regional language, IVR and WhatsApp access.
- **Fair-price band instead of fixed price:** protects the farmer from underpricing and the consumer from overpricing at the same time.

## 4. Technical Approach

The system has five layers: user apps, an API gateway, core services (matching, pricing, logistics, payments), a data layer and external integrations. The architecture diagram is shown below.

&#91;embedded content: system architecture · 4 layers\]

Users reach the platform through one gateway. The matching engine (highlighted) pools buyer orders and assigns them to nearby farmers, while pricing, routing and payments plug into it and share one data layer.

<img width="2055" height="1580" alt="1_architecture_diagram" src="https://github.com/user-attachments/assets/5d4b8d7f-6274-4466-a98e-aad9d5998371" />
<img width="2055" height="1272" alt="2_workflow_diagram" src="https://github.com/user-attachments/assets/2c3609fb-8090-4407-9cc9-cceee06b235f" />


**Technology stack (proposed):**

- **Frontend:** React Native mobile app (Android first), React web dashboard for FPO and admin; Bhashini / speech-to-text for voice input in regional languages.
- **Backend:** Python (FastAPI) microservices, REST APIs, Redis queue for order events.
- **Database:** PostgreSQL (orders, users, ledger) and PostGIS for location queries; object storage for produce photos.
- **AI/ML:** Time-series forecasting (e.g., Prophet / gradient boosting) for fair price band and demand forecasting; clustering plus a vehicle routing solver (OR-Tools) for batched delivery; image-based quality grading as a later phase.
- **Payments:** UPI with split settlement through a payment aggregator, and an ledger service for the price waterfall.
- **Data sources:** Agmarknet / e-NAM price and arrival data, weather API, and optional integration with government farmer registries for verification.

## 5. Feasibility and Viability

- **Technical feasibility:** every component uses mature, open technologies and public data sources, so a working pilot can be built with a small team.
- **Operational feasibility:** FPOs and SHGs already exist across India and already do aggregation, so GaonSetu digitises and supports an existing structure rather than creating a new one.
- **Financial viability:** a small platform fee (a few percent) on each order plus VCP service fees sustains the network, while the total chain cost remains lower than the traditional 6 to 8 layer chain.
- **Pilot plan:** start with one district, 2 to 3 high-volume perishable crops (tomato, onion, leafy vegetables), 5 to 10 VCPs and 3 to 5 institutional buyers; measure farmer realisation, consumer price and wastage; then scale.

## 6. Expected Impact

- **Farmers:** higher share of the consumer's rupee, assured buyer before harvest, payment within a day.
- **Consumers:** fresher produce and lower prices through fewer layers and lower wastage.
- **Community:** local employment for SHG and FPO members, and women's participation in the supply chain.
- **Environment:** less food wastage and fewer empty-return trips through batched delivery.
- **Alignment:** supports SDG 1 (No Poverty), SDG 2 (Zero Hunger) and SDG 12 (Responsible Consumption), and complements government initiatives such as e-NAM and FPO promotion.

## 7. Challenges and Mitigation

| Challenge | Mitigation |
| --- | --- |
| Farmers' low digital literacy | Voice-based app, regional languages, IVR/WhatsApp, VCP operators as assisted users |
| Side-selling (farmer sells to a trader at the last moment) | Advance token, rating system, priority in future orders for reliable farmers |
| Quality disputes | Grading and weighing at VCP with photo and weight record |
| Perishability and delays | Short collection-to-delivery windows, batched routes, nearby buyer matching |
| Trader resistance | Offer traders a role as licensed VCP operators or transporters with capped service fees |
| Cold start (not enough buyers) | Begin with institutional and community buyers who order in bulk and on a schedule |

## 8. References

- Government of India, Lok Sabha (Ministry of Agriculture), reply on intermediaries in the agricultural supply chain: https://eparlib.nic.in/bitstream/123456789/611033/1/113092.pdf
- Agmarknet (market arrivals and prices) and e-NAM (National Agriculture Market) public portals.
- Kerala Startup Mission, AgriNext challenge on high intermediary costs: https://agrinext.startupmission.in/challenges/cat-E/E1
