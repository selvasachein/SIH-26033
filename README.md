# Smart India Hackathon Workshop
# Date:
## Reference Number:
## Name:

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

1. GradeLine is a website and mobile app where Farmer Producer Organisations (FPOs) sell tomatoes directly to buyers. There are three kinds of buyers:

Bulk buyers: hotels, shops and canteens
Households: families who order together as a neighbourhood
Processors: sauce and pickle makers

The system has four main parts:

Quality grading: The FPO takes photos of sample tomatoes. The app’s AI suggests a grade (A, B or C), and an FPO field officer checks and confirms it. Each grade gets its own price, so better tomatoes earn more money.
Traceability: Every crate gets a QR code. When the buyer scans it, they can see which FPO it came from, when it was harvested and its grade.
Logistics support: Instead of each farm sending its own vehicle, one truck collects from several nearby farms, takes the tomatoes to a city hub, and delivers to buyers.
Demand forecasting: The app predicts how many tomatoes buyers will need next week, so farmers can harvest the right amount.

2. Problem 1: Farmers earn too little. An RBI study found that farmers get around 33 per cent of the consumer rupee for tomato, 36 per cent for onion and 37 per cent for potato. In comparison, dairy farmers get around 70 per cent of the final price. GradeLine helps in two ways. Selling directly removes some middlemen, and grade-based pricing pays more for better-quality tomatoes.
Problem 2: Too much produce is wasted. A government-backed NABCONS study found tomato losses of 11.62%, with 8.37% at the farm stage and 3.25% during market handling. Most of the loss happens at the farm, so GradeLine reduces waste in three ways: 
global-agriculture
The forecast helps farmers harvest only what will sell.
Shared truck routes reduce handling and travel time.
Very ripe Grade C tomatoes are sold to sauce and pickle makers instead of being thrown away.

3. Connecting farmers directly to buyers is not new by itself. The government’s e-NAM platform had 1,522 mandis integrated as of June 30, 2025, with 1.79 crore farmers and 4,518 FPOs registered. Private companies like Ninjacart and DeHaat also work in this space. 
indiancooperative

What makes GradeLine different:

AI grading with a human check: The AI suggests the grade and a person confirms it. This is more reliable than AI alone and easier for buyers to trust.
A buyer for every grade: Even Grade C tomatoes have a market (processors), so less is wasted.
Crate-level traceability: Any buyer can check where their tomatoes came from with a phone.
FPO-first design: The seller is a farmer group, not individual farmers, which makes collecting produce and onboarding easier.
All in one app: Grading, buying, delivery and forecasting together. e-NAM mainly connects mandi traders. It does not sell to households or plan delivery routes.

## Technical Approach

1. Technologies to be used

Part	Technology	Why
Website (front end)	HTML, CSS, JavaScript	Simple and works on any browser
Server (back end)	Firebase (or Node.js)	Quick to set up for a student project
Database	Firebase Firestore	Stores listings, orders and batches
Grading AI	Google Gemini (image AI)	Can look at tomato photos and suggest a grade without training our own model
Demand forecasting	Python, using past mandi price data from AGMARKNET	A model learns from past prices and sales to predict future demand
Route planning	Google OR-Tools + Google Maps	Free tools that find the shortest route to visit many farms
Payments	UPI (through a payment service like Razorpay)	Fast payment to FPOs
Traceability	QR codes	Cheap and any phone can scan them
Hardware	Smartphone camera, weighing scale, printed QR stickers	No special equipment needed

Note: Route planning uses optimization algorithms (step-by-step methods for finding the best route), not machine learning. Demand forecasting and grading are the parts that use AI.
2. FPO harvests tomatoes
Upload sample photos
AI suggests grade A/B/C
Field officer confirms grade
Listing goes live with QRcrate tag
Demand forecast
Buyer places order
Route planner groupspickups
Truck: farms → city hub →buyers
Buyer scans QR on delivery
Payment sent to FPO

## Feasibility and Viability

1. Analysis of the feasibility of the idea

Technical (high): All the tools needed already exist and are free or cheap to start with. The hard part is getting good data, not writing the code.
Practical (medium): Many FPOs exist, and the government supports them through the 10,000 FPO Scheme, which encourages aggregation, processing, and collective marketing. But signing up is not the same as using the platform. In one Maharashtra district, out of 28,197 farmers registered, 10,437 have traded on e-NAM. GradeLine should expect a similar drop-off. 
Financial (uncertain): Transport is the biggest cost. Tomatoes are cheap per kg and spoil quickly, so a half-empty truck can wipe out the profit. The idea only makes money with enough regular orders.

 2. Potential challenges and risks

Buyers may disagree with the grade, and photos only show the outside of the tomato.
At the start there may not be enough buyers or sellers. Each side waits for the other to join first.
Delivery is costly, and tomatoes spoil in Chennai’s heat without cold storage.
Tomato prices change a lot with rain and festivals, making forecasts hard. A new app also has little past data to learn from.
Local traders may pay farmers more for a short time to keep them away from the platform.
Some farmers may not be comfortable using apps.
Late payments would break farmers’ trust.

3. Strategies for overcoming these challenges
Grading disputes: keep a person in the grading step, save photos as proof, and have a clear refund rule.
Not enough users: start small, with one crop, one FPO group, and a few big buyers like hotels and canteens, before adding households.
Delivery cost: run fixed truck routes (for example, three days a week) so trucks always go out full.
Weak forecasts: start with public mandi data and improve the forecast as our own order data grows.
Digital comfort: let the FPO staff run the app instead of each farmer, and provide it in Tamil.
Payment trust: promise payment to FPOs within a fixed time, for example 24 hours.

## Impact and Benefits

1. Potential impact on the target audience
Farmers and FPOs: earn more for better-quality tomatoes, get paid faster, and plan harvests better.
Bulk buyers: get steady quality with a clear grade, and know where the produce came from.
Households: get fresher tomatoes, possibly at a lower price if the savings beat delivery costs.
Processors: get a steady, cheap supply of ripe tomatoes.

2. Benefits of the solution (social, economic, environmental, etc.)
Economic: Our target is to raise the farmer’s share above today’s ~33% for tomato. This is a goal to test in a pilot, not a proven figure. Less waste also means more produce gets sold instead of thrown away.
Social: stronger farmer groups, clear and fair pricing, and less dependence on a single local trader.
Environmental: less food waste (NABCONS estimates annual losses of 11.97 million MT for vegetables), and fewer half-empty truck trips, which means less fuel burned.

## Research and References

1. Details / Links of the reference and research work
RBI Working Paper 08/2024, Vegetables Inflation in India: A Study of Tomato, Onion and Potato: https://rbi.org.in/scripts/PublicationsView.aspx?Id=22723
RBI press release on the same study: https://www.rbi.org.in/scripts/BS_PressReleaseDisplay.aspx?prid=58813
Business Standard summary of the RBI study: https://www.business-standard.com/amp/markets/capital-market-news/rbi-study-shows-tomato-onion-and-potato-farmers-get-only-a-third-of-retail-price-that-consumer-pays-124100400307_1.html
NABCONS post-harvest loss study, as cited in a Rajya Sabha answer (Feb 2025): https://rsdebate.nic.in/bitstream/123456789/758453/1/PQ_267_07022025_U572_p312_p312.pdf
Tomato loss figures from the NABCONS study: https://www.global-agriculture.com/india-region/indias-highest-post-harvest-losses-guava-and-tomato-among-the-worst-hit/
e-NAM status, Lok Sabha answer (July 2025): https://eparlib.sansad.in/bitstream/123456789/2998079/1/AU1504_HVk1tf.pdf
Government schemes on post-harvest losses: https://iasscore.in/current-affairs/government-schemes-to-mitigate-post-harvest-losses-in-india
e-NAM official site: https://enam.gov.in
AGMARKNET (mandi price data): https://agmarknet.gov.in
Google OR-Tools (route planning): https://developers.google.com/optimization/routing
