# Smart India Hackathon Workshop
# Date:21/11/2026
## Reference Number:26019361
## Name: Gunaseelan.K

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

1. Detailed explanation of the proposed solution:

    FarmDirect is a real-time digital marketplace where farmers and Farmer Producer Organisations (FPOs) list their produce and sell directly to households, restaurants, retailers and bulk buyers, without wholesalers, commission agents or multiple retailers in between.
    • Farmer/FPO app: post crop, quantity, harvest date and price in a few taps (voice input and regional languages for low-literacy users).
    • Consumer and bulk buyer app: browse live listings, see farmer details, place single or bulk orders and pay through UPI.
    • Logistics layer: pickup points, delivery partners and shared transport matched to each order.
    • AI engine: forecasts demand, suggests a fair price to farmers and optimises delivery routes.
    • Price transparency: every listing shows what the farmer receives, the small platform fee and the final consumer price, compared with the usual market price.
   
2. How it addresses the problem:

    • Removes intermediaries: the long chain (farmer, local trader, mandi agent, wholesaler, retailer) is replaced by one direct link plus a flat, visible platform fee.
    • Raises farmer income: farmers set their own price and receive payment directly, instead of accepting a price decided by the chain.
    • Lowers consumer prices: the margins taken by each middleman are cut, so the final price falls while the farmer still earns more.
    • Cuts waste and inefficiency: demand forecasting tells farmers what to grow and sell, and route optimization reduces transport time and spoilage of perishables.
   
3. Innovation and uniqueness of the solution:
   
    • Real-time marketplace: listings, stock and orders update live for every user.
    • Transparent price breakdown on every item, so trust is built into the product.
    • AI-assisted fair pricing using mandi price trends, so farmers are not underpricing out of lack of information.
    • FPO and bulk-buyer mode, so small farmers can pool produce and reach large buyers.
    • Inclusive design: regional languages, voice input and OTP login suited to rural users.
    • Traceability: a QR code per batch showing the farm, village and harvest date.

## Technical Approach

1. Technologies to be used

    • Frontend: HTML, CSS, JavaScript (React or Flutter for the mobile app).
    • Backend: Node.js with Express.
    • Real-time communication: Socket.IO (Web Sockets).
    • Database: MongoDB or PostgreSQL.
    • AI/ML: Python with scikit-learn or Prophet for demand forecasting; Google OR-Tools for route optimization.
    • Data sources: Agmark net / data.gov.in for live mandi prices; weather API for harvest and delivery planning.
    • Payments: UPI / Razor pay.
    • Maps and logistics: Google Maps or OpenStreetMap APIs.
    • Authentication: mobile OTP.
    • Languages: multilingual interface (Tamil, Hindi, English and more).
   
2. Methodology and process for implementation

    1.  Onboard: farmers/FPOs and buyers register with mobile OTP.
    2.  List: the farmer posts produce and price; the AI suggests a fair price from market trends.
    3.  Broadcast: the listing appears instantly to all nearby consumers and bulk buyers.
    4.  Order and pay: the buyer orders and pays by UPI; stock updates live and the farmer is notified.
    5.  Logistics: the system assigns a delivery partner or pickup point and computes the optimized route.
    6.  Deliver and settle: the buyer receives the produce and the farmer is paid directly, with the platform fee shown.
    7.  Learn: order data feeds the forecasting model, which improves price and planting suggestions.

<img width="1001" height="381" alt="image" src="https://github.com/user-attachments/assets/79da2b54-5b81-4075-9910-5c2aca9464d1" />


## Feasibility and Viability

    • Technical feasibility: built on mature, open-source tools and public APIs; a working prototype already exists.
    • Scalability: a cloud deployment and a standard database can scale from a district pilot to state level.
    • Adoption: smartphone and UPI use is already widespread in rural India; FPOs give a ready channel to reach many farmers at once.
    • Revenue model: a low flat platform fee (for example 3%), plus optional logistics charges, keeps the model sustainable while staying far cheaper than the intermediary chain.
    • Challenges and mitigation:
        ◦ Digital literacy: voice input, regional languages and FPO field agents.
        ◦ Cold chain and delivery cost: shared transport, pickup points and route optimization.
        ◦ Trust and quality: ratings, grading and batch traceability.
        ◦ Buyer reach in early stages: start with local clusters of households, hotels and bulk buyers.
        
## Impact and Benefits

    • Farmers: higher and faster income through direct payment and fair pricing.
    • Consumers: fresher produce at lower prices with full price transparency.
    • Bulk buyers: reliable supply directly from FPOs.
    • Economy and society: reduced supply chain inefficiencies, less food wastage and stronger rural development.
    • Government: better data on supply and demand to support price monitoring and policy.
    • Environment: shorter supply chains and optimized routes reduce fuel use and spoilage.

## Research and References

    1.  Agmarknet, Ministry of Agriculture & Farmers Welfare. Daily mandi arrival and price data. https://agmarknet.gov.in
    2.  e-NAM (National Agriculture Market). Online trading platform for agricultural commodities. https://enam.gov.in
    3.  Open Government Data Platform India. Datasets on crop prices, production and weather. https://data.gov.in
    4.  Open Network for Digital Commerce (ONDC). Open protocol for digital commerce. https://ondc.org
    5.  Department of Agriculture & Farmers Welfare. Scheme for formation and promotion of 10,000 Farmer Producer Organisations (FPOs). https://agriwelfare.gov.in
    6.  Department of Consumer Affairs, Ministry of Consumer Affairs, Food & Public Distribution. Price monitoring of essential commodities. https://consumeraffairs.nic.in
    7.  Socket.IO documentation. Real-time communication. https://socket.io/docs/v4/
    8.  Google OR-Tools documentation. Route optimisation. https://developers.google.com/optimization
    9.  Prophet documentation. Time-series demand forecasting. https://facebook.github.io/prophet/
