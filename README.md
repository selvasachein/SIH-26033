# Smart India Hackathon Workshop
# Date:19.01.26
## Reference Number:26014166
## Name: Sanjith S

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
### 1.1 Detailed Explanation of the Proposed Solution

FarmLink Direct is a digital marketplace that connects farmers and Farmer Producer Organisations (FPOs) directly with consumers, hostels, restaurants and local shops.

Farmers can upload product details, available quantities, location and selling prices. Buyers can view products, compare prices and place orders directly through the platform.

The main feature is Group Buying, which combines orders from nearby buyers to help reduce transportation costs. The platform can also provide surplus produce alerts and demand forecasts.

### 1.2 How It Addresses the Problem

The platform helps farmers find buyers without depending on multiple unnecessary intermediaries. Buyers can compare prices and purchase products directly from farmers.

Group buying can reduce delivery costs, while transparent pricing helps farmers and buyers understand the cost of each transaction.

### 1.3 Innovation and Uniqueness

The main innovation is a group-buying system designed for hostels, restaurants and local retailers.

Key features include:

- Direct farmer-to-buyer connections.
- Group buying for nearby buyers.
- Transparent product and delivery pricing.
- Surplus produce notifications to reduce waste.
- Demand forecasting to help farmers plan supply.
- Regional language support for easier access.

## Technical Approach
```mermaid
flowchart TD
    A["Farmers / FPOs"] --> B["Upload crops and prices"]
    B --> C["FarmLink Direct Platform"]
    C --> D["Display products and transparent prices"]
    D --> E["Group Buying by Nearby Buyers"]
    E --> F["Combine Orders"]
    F --> G["Direct Delivery"]
    G --> H["Better Farmer Earnings"]
    G --> I["Affordable Prices for Consumers"]
```
### 2.1 Technologies to Be Used

- Frontend: HTML, CSS, JavaScript and Bootstrap.
- Backend: Python with Django.
- Database: SQLite for the initial prototype.
- Maps: OpenStreetMap for location-based features, if required.

### 2.2 Methodology and Implementation Process

1. Register farmers and buyers on the platform.
2. Allow farmers to upload products, prices and quantities.
3. Display products for buyers to browse and compare.
4. Combine nearby buyers' orders using the group-buying feature.
5. Process orders and display transparent cost details.
6. Store product and order information in the database.
7. Test the system with sample farmers, products and buyers.

### 2.3 Technical Flow Diagram

Farmer Registration
        |
        v
Upload Products and Prices
        |
        v
FarmLink Direct Platform
        |
        v
Product Listing and Price Comparison
        |
        v
Group Order Matching
        |
        v
Order Confirmation and Delivery
        |
        v
Consumer Receives Products
## Feasibility and Viability
### 3.1 Feasibility of the Idea

FarmLink Direct can be developed as a web application using HTML, CSS, JavaScript, Python Django and SQLite. A basic prototype can be created with product listings, buyer registration, order management and group buying.

The platform can initially be tested with a small group of farmers and buyers in a local area before expanding to other regions.

### 3.2 Potential Challenges and Risks

- Farmers may have limited digital skills or internet access.
- Product prices and availability may change frequently.
- Delivering small quantities to distant buyers can be expensive.
- Product quality and delivery delays may affect buyer trust.

### 3.3 Strategies to Overcome Challenges

- Provide a simple interface and regional language support.
- Allow farmers to update prices and quantities regularly.
- Group nearby orders to reduce delivery costs.
- Introduce order tracking, buyer feedback and clear delivery policies.
## Impact and Benefits
### 4.1 Potential Impact on the Target Audience

The platform aims to help farmers reach more buyers and improve their access to markets. Consumers, hostels, restaurants and retailers can compare prices and purchase agricultural products directly.

### 4.2 Benefits of the Solution

**Economic Benefits**
- Potentially improve farmers' share of the selling price.
- Help buyers find competitive prices.
- Reduce delivery costs through group buying.

**Social Benefits**
- Improve market access for small farmers.
- Connect local farming communities with nearby buyers.
- Support easier access through regional language options.

**Environmental Benefits**
- Reduce food waste through surplus produce alerts.
- Improve delivery efficiency by grouping nearby orders.
- Encourage local sourcing where practical.
## Research and References
### 5.1 References and Research

1. Ministry of Agriculture and Farmers Welfare, Government of India: https://agriwelfare.gov.in/
2. e-NAM (National Agriculture Market): https://www.enam.gov.in/
3. Digital India: https://www.digitalindia.gov.in/
4. Django documentation: https://docs.djangoproject.com/
5. OpenStreetMap: https://www.openstreetmap.org/

These resources can be used to research agricultural market access, digital platforms and the technologies proposed for the solution.
