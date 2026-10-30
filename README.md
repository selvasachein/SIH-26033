# Smart India Hackathon Workshop
# Date:
30.10.2026
## Reference Number:
26018192
## Name:
K Dharsan Raj

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

1. Detailed Explanation of the Proposed Solution

HarvestLink – A Demand-Driven Farm-to-Consumer Marketplace

HarvestLink is a digital agricultural marketplace designed to connect farmers, Farmer Producer Organisations (FPOs), consumers, retailers and bulk buyers through a single platform.

The main idea is to introduce a demand-first selling model. Instead of farmers producing and searching for buyers afterwards, the platform collects buyer requirements in advance and helps farmers plan their sales based on actual demand.

The platform provides the following features:

Direct Farmer-to-Buyer Connection: Farmers can list their agricultural products and receive orders directly from consumers and bulk buyers.

Community Group Purchasing: Consumers in nearby locations can combine their orders to reduce delivery and transportation costs.

Transparent Pricing: The platform displays farmer selling prices, transportation charges, packaging expenses and platform fees separately.

AI-Based Demand Forecasting: Machine learning analyses previous sales and seasonal trends to predict future product demand.

Smart Logistics: The system groups nearby orders and suggests efficient delivery routes.

QR-Based Product Tracking: Each agricultural batch receives a unique QR code to provide product origin and delivery information.

2. How It Addresses the Problem

Traditional agricultural supply chains often involve multiple traders and distributors, which can increase consumer prices and reduce the farmer's share of the final selling price.

HarvestLink addresses these issues through:

Connecting farmers directly with consumers and bulk buyers.

Reducing unnecessary trading layers.

Combining nearby consumer orders to reduce transportation expenses.

Providing transparent pricing information.

Helping farmers understand market demand before selling their products.

Improving delivery coordination through smart logistics.

The platform does not eliminate useful services such as transportation, storage and packaging. Instead, it makes their costs transparent and encourages efficient coordination.

3. Innovation and Uniqueness of the Solution

The main innovation of HarvestLink is its combination of demand-first selling, community group purchasing and coordinated agricultural logistics.

Its unique features include:

Demand-First Selling: Collecting buyer requirements before matching available agricultural products.

Community Basket: Combining nearby household orders to enable shared transportation.

Harvest Window Matching: Matching farmers' expected harvesting dates with future buyer requirements.

Transparent Price Distribution: Showing how the final consumer price is divided among the farmer and service expenses.

Farmer Choice Mechanism: Allowing farmers to compare different buyer offers and choose suitable prices.

These features make HarvestLink more than a normal agricultural shopping application. It focuses on improving the entire process of connecting agricultural supply with consumer demand.

## Technical Approach

1. Technologies to Be Used

Component

Technology

Frontend

HTML, CSS, JavaScript

Backend

Python, Django

Database

SQLite initially, PostgreSQL for deployment

AI and Machine Learning

Python, Pandas, Scikit-learn

Maps and Routes

OpenStreetMap and routing services

QR Code Generation

Python QR code libraries

Authentication

OTP-based authentication

Payment Integration

UPI-compatible payment gateway

Hosting

Cloud-based hosting

2. Methodology and Process for Implementation

Step 1: Farmer Registration

Farmers register on the platform and provide their basic details, location and available agricultural products.

Step 2: Product Listing

Farmers upload product details such as crop name, quantity, expected price, quality grade and harvesting date.

Step 3: Buyer Registration and Demand Collection

Consumers, retailers, restaurants and bulk buyers register and specify their product requirements.

Step 4: Supply and Demand Matching

The system compares available agricultural products with buyer requirements based on quantity, location, product type and price.

Step 5: AI-Based Demand Forecasting

The AI module analyses historical sales and seasonal trends to predict approximate future product demand and provide suggestions to farmers.

Step 6: Transparent Price Calculation

The system displays the farmer's selling price, packaging expenses, transportation charges and platform fees separately.

Step 7: Smart Logistics Management

The platform groups nearby orders and identifies suitable collection points to reduce repeated transportation.

Step 8: Delivery and Payment

Products are delivered to buyers, and digital transaction records are maintained for completed orders.

Technical Workflow Diagram

flowchart TD
    A[Farmer Registration] --> B[Product Listing]
    C[Buyer Registration] --> D[Demand Collection]

    B --> E[Central Marketplace]
    D --> E

    E --> F[AI Demand Forecasting]
    E --> G[Supply and Demand Matching]

    F --> G

    G --> H[Transparent Price Calculation]
    H --> I[Order Confirmation]

    I --> J[Group Order Management]
    J --> K[Smart Logistics]

    K --> L[Collection and Verification]
    L --> M[Product Delivery]

    M --> N[Digital Payment Records]
    N --> O[Farmer Earnings Dashboard]

Implementation Plan

The project will be developed in three stages:

Stage 1 – Basic Marketplace

Farmer and buyer registration.

Product listing.

Product searching.

Order placement.

Stage 2 – Smart Marketplace

Community group purchasing.

Transparent price calculator.

Demand and supply matching.

Stage 3 – Advanced Features

AI-based demand forecasting.

Smart route optimization.

QR-based product tracking.

Digital payment integration.

## Feasibility and Viability

1. Analysis of the Feasibility of the Idea

Technical Feasibility:

HarvestLink can be developed using existing web technologies, Python frameworks, databases and machine-learning libraries. The initial version can be implemented as a web application and later expanded into a mobile application.

Economic Feasibility:

The platform can begin with limited infrastructure expenses by using open-source technologies and existing transportation providers. A small and transparent service fee can support the operation of the platform.

Operational Feasibility:

Farmers can access the platform through smartphones. A simple interface with regional-language support can help farmers who are not familiar with digital technology.

2. Potential Challenges and Risks

Low digital literacy among some farmers.

Difficulty in verifying product quality.

Uncertain agricultural demand.

Transportation and delivery expenses.

Perishable products and storage difficulties.

Internet connectivity problems.

Payment disputes between buyers and sellers.

3. Strategies for Overcoming These Challenges

Challenge

Proposed Solution

Low digital literacy

Simple interface and regional-language support

Product quality issues

Quality grading and product verification

Uncertain demand

AI-based demand forecasting

High transportation expenses

Shared delivery and route optimization

Perishable products

Demand-based collection and faster delivery

Internet connectivity

Lightweight and mobile-friendly application

Payment disputes

Digital transaction records and order confirmation

Long-Term Viability

HarvestLink can generate revenue through small transaction-based service fees, optional logistics coordination fees and subscription services for bulk buyers.

The platform can initially operate in a limited geographical area and gradually expand based on farmer participation and consumer demand.

## Impact and Benefits

1. Potential Impact on the Target Audience

The primary target audience includes:

Small and medium-scale farmers.

Farmer Producer Organisations (FPOs).

Individual consumers.

Retail shops.

Hotels and restaurants.

Agricultural wholesalers and bulk buyers.

Local transportation providers.

The platform aims to improve coordination between farmers and buyers while reducing unnecessary distribution expenses.

2. Benefits of the Solution

Social Benefits

Better market access for farmers.

Improved communication between farmers and consumers.

Increased awareness of digital agricultural services.

Support for rural digital development.

Economic Benefits

Improved opportunities for farmer earnings.

Better price transparency.

Reduced unnecessary supply chain expenses.

Affordable group purchasing opportunities.

Improved market access for small farmers.

Environmental Benefits

Reduced unnecessary transportation.

Better delivery route planning.

Potential reduction in fuel consumption.

Reduced food wastage through demand-based planning.

Expected Pilot Impact

The initial pilot can target:

50–100 participating farmers.

100–200 consumers.

5–10 bulk buyers.

5–10 agricultural product categories.

These are proposed targets and not measured results. Actual impact will be evaluated by comparing farmer earnings, consumer prices, transportation expenses and product wastage before and after implementation.

## Research and References

The following resources provide background information and technical guidance for the development of HarvestLink.

Smart India Hackathon – Problem Statement 26033

https://github.com/selvasachein/SIH-26033

National Agriculture Market (e-NAM)

https://www.enam.gov.in/

Reference for digital agricultural trading and market access.

Ministry of Agriculture and Farmers Welfare

https://agriwelfare.gov.in/

Reference for agricultural policies and farmer development programmes.

Small Farmers' Agribusiness Consortium (SFAC)

https://sfacindia.com/

Reference for Farmer Producer Organisations and agricultural market linkages.

Django Documentation

https://docs.djangoproject.com/

Reference for backend application development.

Scikit-learn Documentation

https://scikit-learn.org/

Reference for machine-learning implementation.

PostgreSQL Documentation

https://www.postgresql.org/docs/

Reference for database development.
