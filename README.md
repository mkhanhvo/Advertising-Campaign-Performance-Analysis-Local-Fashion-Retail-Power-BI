# Marketing Campaign Performance Overview: Revenue, Profit and Advertising Impact

### Author: Vo Tran Mai Khanh
### Date: 12/2025
### Tools Used: Power Query, PBI

## 📌 Background & Overview  

### Objective:
- Evaluate the overall effectiveness and profitability of advertising campaign
- Compare performance between advertising driven sales and direct sales channels
- Assess campaign-level efficiency (ROAS, revenue impact, profit contribution)
- Identify high performing products to scale investment and low performing products to reconsider
- Analyze product-level profitability to optimize budget allocation
- Provide data driven recommendations to improve marketing spend efficiency

### 👤 Who is this project for?  
- Marketing Manager – to evaluate campaign effectiveness and allocate budget
- Performance Marketing Team – to optimize ads and scale high-performing campaigns
- Sales Team – to compare Ads vs Direct sales performance
- Finance Team – to assess profitability and monitor cost efficiency

### Client Background
The business operates in the Vietnamese fashion market with nationwide coverage. This project focuses on analyzing online marketing campaigns for the women’s fashion category across 62 cities and provinces, spanning Northern to Southern Vietnam, the campaigns were conducted over a one month period and have entered the review stage. The analysis evaluates campaign performance based on revenue contribution, effectiveness across products and the efficiency of marketing spend allocation. The objective is to support data driven decisions on whether to maintain or adjust campaign setups, budget distribution, creative strategies and overall marketing execution

## 📂 Dataset Description & Data Structure  

### 📊 Data Source  
- Source: dataset including order data (Direct vs Ads), campaign spending distribution and product dimension tables, enabling performance and profitability analysis at channel and product levels
- Size: ~600+ records across two fact tables and supporting product dimensions
- Format: .xlsx

#### 1️⃣ Tables Used: 
- Fact_Order
- Fact_MKT camp by sku cost
- Dim_MKT camp cost
- Dim_danh sach san pham
- Dim_category
- Dim_product
- Dim_sale sources
- Date

#### 2️⃣ Table Schema & Data Snapshot

**Table 1: Campaigns Table**
<details>
<summary>Campaigns Table Schema</summary>
<img width="700" height="96" alt="image" src="https://github.com/user-attachments/assets/5eb6d783-9e0e-43df-82ee-ef39ce800842" />
<img width="700" height="92" alt="image" src="https://github.com/user-attachments/assets/3bd58a82-d1e6-489f-bdff-b7481fb9b8c0" />
<img width="700" height="95" alt="image" src="https://github.com/user-attachments/assets/a1fd058f-1aa9-4b8b-9f00-e107ec5f000d" />
<img width="700" height="80" alt="image" src="https://github.com/user-attachments/assets/eea5b0aa-b8d3-4fef-967a-287491a46cc7" />
<img width="700" height="91" alt="image" src="https://github.com/user-attachments/assets/5b01497e-f7c6-4cee-a530-96b048053a5a" />
</details>

**Table 2: Order Table**
<details>
<summary>Order Table Schema</summary>
<img width="700" height="94" alt="image" src="https://github.com/user-attachments/assets/cdf61317-0795-4555-a3ed-72fda80cea0e" />
<img width="700" height="92" alt="image" src="https://github.com/user-attachments/assets/648a27e7-7390-4bea-b7e6-d9720d38644f" />
</details>

**Table 3: Date**
<details>
<summary>Date Table Schema</summary>
<img width="488" height="92" alt="image" src="https://github.com/user-attachments/assets/138bce25-db57-4f5d-a533-68e8da782bfa" />
</details>

**Table 4: Dim Marketing Camp Cost**
<details>
<summary>Dim Marketing Camp Cost Table Schema</summary>
<img width="940" height="94" alt="image" src="https://github.com/user-attachments/assets/70aabf1a-cdbc-4f0d-add8-bb1b5a9d2b6a" />
<img width="405" height="92" alt="image" src="https://github.com/user-attachments/assets/89889eed-ab09-4a44-995c-09da88f4a6e2" />
</details>

**Table 5: Dim Danh Sach San Pham**
<details>
<summary>Dim Danh Sach San Pham Schema</summary>
<img width="1030" height="92" alt="image" src="https://github.com/user-attachments/assets/31f1151b-0695-4c2b-a9e6-ae6fe1495230" />
</details>

**Table 6: Dim Category**
<details>
<summary>Dim Category Table Schema</summary>
<img width="156" height="205" alt="image" src="https://github.com/user-attachments/assets/55b84d81-ea23-42d4-9bc3-993f0e0167bf" />
</details>

**Table 7: Dim Product**
<details>
<summary>Dim Product Table Schema</summary>
<img width="350" height="93" alt="image" src="https://github.com/user-attachments/assets/99252f05-62d0-4d10-b5c1-ea82db4353d4" />
</details>

**Table 8: Dim Sale Sources**
<details>
<summary>Dim Sale Sources Table Schema</summary>
<img width="71" height="45" alt="image" src="https://github.com/user-attachments/assets/2bb80249-93de-468d-b133-84163460e444" />
</details>

#### 3️⃣ Data Relationships: 
- Fact_MKT camp by sku cost -> Dim_MKT camp cost: many to one
- Fact_MKT camp by sku cost -> Date: many to one
- Fact_MKT camp by sku cost -> Dim_danh sach san pham: many to one
- Fact Order -> Date: many to one
- Fact Order -> Dim_danh sach san pham: many to one
- Fact Order -> Dim Category: many to one
- Fact Order -> Dim Product: many to one
- Fact Order -> Dim Sale Sources: many to one

<img width="636" height="518" alt="image" src="https://github.com/user-attachments/assets/8e56a56a-35c8-420a-8ecc-5a6410ae7f51" />

## 🧠 Design Thinking Process  
1️⃣ Empathize 

<img width="641" height="337" alt="image" src="https://github.com/user-attachments/assets/29083f73-25f2-4cf8-a652-7c04bdf4ed04" />

2️⃣ Define point of view 

<img width="938" height="302" alt="image" src="https://github.com/user-attachments/assets/a5062b81-2b15-4a84-939a-8e30b6ac059f" />

3️⃣ Ideate  

<img width="1052" height="206" alt="image" src="https://github.com/user-attachments/assets/e3148cb8-2ee2-4c9e-8b91-51e8c7cfa9ba" />

## 📊 Key Insights & Visualizations  

### 🔍 Dashboard Preview  

#### 1️⃣ Overview page preview  



### *Revenue by Channel*

![image alt](https://github.com/mkhanhvo/Business-Performance-Overview-Revenue-Profit-Advertising-Impact/blob/f8bb11ba10f43e19611ed8eb6be629bd56f778e6/Insight%20-%20Revenue%20by%20Channels.png)

### *% Budget used and ads profit by day*

![image alt](https://github.com/mkhanhvo/Business-Performance-Overview-Revenue-Profit-Advertising-Impact/blob/a3ad2e2214eb3e33920b1f0692f350fd4cbe1b28/Overall%20-%20%25%20budget%20used%20vs%20profit.png)

Deeper analysis indicates that the core issue is a uniform and prolonged discount policy applied across categories. This policy resulted in systematic profit losses across both ads and direct sales channels. At the same time, conversion performance varies significantly by product category, suggesting that budget allocation and sales strategy should be category specific rather than evenly distributed

### *Discount impact on profit from ads channel*

![image alt](https://github.com/mkhanhvo/Business-Performance-Overview-Revenue-Profit-Advertising-Impact/blob/49e48f30846442ad27327c60ce3170fcd1ab0397/Insight%20-%20Discount%20impact%20on%20profit%20(ads).png)

### *Discount impact on profit from direct channel*

![image alt](https://github.com/mkhanhvo/Business-Performance-Overview-Revenue-Profit-Advertising-Impact/blob/49e48f30846442ad27327c60ce3170fcd1ab0397/Insight%20-%20Discount%20impact%20on%20profit%20(direct).png)

## I. Marketing Performance – Insights & Recommendations
### 1. Budget Control & Spending Efficiency
Budget utilization was well controlled for over 86% of the campaign duration, Only 13.33% of total days exceeded budget, mainly during the mid and late stages of the campaign

![image alt](https://github.com/mkhanhvo/Business-Performance-Overview-Revenue-Profit-Advertising-Impact/blob/a68cc732f12c57b70d6ac3a97dcaa4549390404e/Overall%20-%20%25%20budget%20used.png)

However, comparison between ads spend, ROAS and revenue shows no clear linear relationship:
- High ROAS and revenue days did not consistently coincide with overspending days
- Several days with controlled spending still delivered weak performance

![image alt](https://github.com/mkhanhvo/Business-Performance-Overview-Revenue-Profit-Advertising-Impact/blob/160bc71f2bad3a2f5db199364a1bb5b86333a493/Overall%20-%20Buget%2C%20ROAS%2C%20Rev%20by%20day.png)

### -> This indicates that budget level alone is not the primary driver of performance

## Recommendations
_ Avoid optimizing performance solely by increasing or tightening budgets
_ Incorporate creative quality, product category and campaign timing when making scaling decisions

### 2. High Ads Revenue but Weak Profitability
- Out of 2,858 total orders, 1,958 orders (68.5%) were generated through ads, confirming ads as the primary order driving channel. However, when comparing ads spend and ads profit, over 60% of ad days recorded negative profit regardless of spend level. Ads successfully generate volume but fail to deliver consistent profitability
- From a daily perspective: only 29% of days (9/31) were profitable overall. For ads channel specifically, there were 22 days showed negative profit, only 5 days were profitable while the remaining days recorded zero or negative revenue

![image alt](https://github.com/mkhanhvo/Business-Performance-Overview-Revenue-Profit-Advertising-Impact/blob/1a3d54a785ce8eb3cb63fd350252667274469c7e/Overall%20-%20Total%20revenue%20%26%20Profit.png)

## Recommendations
- Shift ads evaluation from revenue generated to revenue generated under a profitable cost structure
- Treat ads as a conditional sales enabler, not a channel for unrestricted scaling

### 3. Revenue Concentration & Campaign-Level Performance
Ads revenue is highly concentrated in a small number of core campaigns: top 5 revenue generating campaigns are mainly driven by Audrey LAL, Flowers Make My Day, Anivan Dress and Margnet Dress
- Category Vay Chiet Eo Xoe (*waist-flare dresses*) account for over 50% of revenue in the Flowers Make My Day campaign
- In contrast, clothing sets generate almost no revenue within these high-performing campaigns.

### *Top 5 campaigns drive revenue*

![image alt](https://github.com/mkhanhvo/Business-Performance-Overview-Revenue-Profit-Advertising-Impact/blob/f5499109bfff2f6bea5496d9b443cfe01c109b76/Top%205%20campaign%20revenue%20.png)

### *Detail revenue of each category from Flowers Make My Day campaign*

![image alt](https://github.com/mkhanhvo/Business-Performance-Overview-Revenue-Profit-Advertising-Impact/blob/f5499109bfff2f6bea5496d9b443cfe01c109b76/Insight%20-%20Category%20%26%20Revenue%20of%20Flower%20make%20my%20day%20camp.png)

In terms of ROAS:
- Category Vay Chiet Eo Om (*waist-fitted dresses*) recorded the highest ROAS (22.9), peaking in Weeks 4–5
- Campaigns launched earlier (Weeks 1–3) did not achieve comparable efficiency
- Out of 175 campaigns, only 7 campaigns (~4%) generated zero revenue, indicating that poor performance is not driven by widespread campaign failure.

### *ROAS and weekly camplaigns run by category*

![image alt](https://github.com/mkhanhvo/Business-Performance-Overview-Revenue-Profit-Advertising-Impact/blob/6ea92a0644f087c108cf4f11163b827c3c3f169f/ROAS%20by%20category.png)

### *Lowest Performing Campaigns by Ad Revenue* 

![image alt](https://github.com/mkhanhvo/Business-Performance-Overview-Revenue-Profit-Advertising-Impact/blob/d12ddaf6183d82e34b7a8d9098d3a74e974bee12/Top%207%20campaign%20with%20lowest%20revenue.png)

## Recommendations
- Reallocate budgets from low performing campaigns and categories toward proven core campaigns
- Prioritize spending during validated high-performance periods (Weeks 4–5) rather than scaling early
- For the 4% of zero-revenue campaigns, optimize creatives or targeting before elimination

## II. Product & Sales Performance – Insights & Recommendations
### 1. Systematic Profit Loss by Category
Category × channel analysis shows: 03 product categories including Ao tach set (*apparels*), Chan vay tach set (*standalone skirts*) and Quan tach set (*standalone pants*) are the primary drivers of negative profit, recording losses in both ads and direct sales for over 80% of campaign days

### *Profit performance and channel contribution analysis of category Ao tach set (*apparel*)*

![image alt](https://github.com/mkhanhvo/Business-Performance-Overview-Revenue-Profit-Advertising-Impact/blob/e360001bdb2216be9f2a8da18d3c7503619a4e7f/Overall%20-%20Revenue%20%26%20Profit%20by%20category%20Ao%20Tach%20Set.png)

### *Profit performance and channel contribution analysis of category Chan vay tach set (*standalone skirts*)*

![image alt](https://github.com/mkhanhvo/Business-Performance-Overview-Revenue-Profit-Advertising-Impact/blob/e360001bdb2216be9f2a8da18d3c7503619a4e7f/Overall%20-%20Revenue%20%26%20Profit%20by%20category%202%20(Chan%20Vay%20Tach%20Set).png)

### *Profit performance and channel contribution analysis of category Quan tach set (*standalone pants*)*

![image alt](https://github.com/mkhanhvo/Business-Performance-Overview-Revenue-Profit-Advertising-Impact/blob/e360001bdb2216be9f2a8da18d3c7503619a4e7f/Overall%20-%20Revenue%20%26%20Profit%20by%20category%203%20(Quan%20Tach%20Set).png)

Other categories experience negative profit for less than 10% of campaign duration. Discount rate is the direct cause of negative profit across all advertised categories, regardless of sales volume or revenue

![image alt](https://github.com/mkhanhvo/Business-Performance-Overview-Revenue-Profit-Advertising-Impact/blob/191a11ad0b63784cba83070463908515f3a3e0af/Overall%20-%20Discount%20impact.png)

All categories record negative profit in both ads and direct sales confirming tha the issue is not channel related, not driven by scale but rooted in pricing and discount policy

### *Profit trends move in the same direction across channels*

![image alt](https://github.com/mkhanhvo/Business-Performance-Overview-Revenue-Profit-Advertising-Impact/blob/55429104f580ee4b77b7dc831ce8812a2d4ee0a8/Overall%20-%20Channel%20contribution%20by%20Profit%20(daily%20level).png)

## Recommendations
- Review and adjust discount levels by category instead of applying a uniform policy
- Reduce discounts for high-volume but high-loss categories to prevent scaling losses
- Prioritize profit per order stability before pushing for higher sales volume

### 2. Conversion Performance by Category
Overall funnel trends:
- CTR remains stable at 0.6% - 1.0%
- Click → Comment/Inbox rates are high (25% - 40%), indicating strong initial interest
- However, Click → Order conversion is only 10% - 23%, showing friction at the purchase decision stage

Budget scaling:
- Does not improve conversion cost
- Conversion cost remains flat or increases slightly as spend grows
- CPM ranges between 60K–100K with no meaningful decline as impressions increase

Category level highlights
- Vay chiet eo xoe (*waist flare dresses*): stable funnel, Click → Order ~20%+, conversion cost does not worsen with increased spend

![image alt](https://github.com/mkhanhvo/Business-Performance-Overview-Revenue-Profit-Advertising-Impact/blob/c6b8fdbab92b15130bd7b583cfdf9bea30123414/Insight%20-%20Conversion%20rate%20funnel%20(v%C3%A1y%20chi%E1%BA%BFt%20eo%20x%C3%B2e).png)
  
- Vay chiet eo om (*waist fitted dresses*): good engagement but unstable conversion efficiency

![image alt](https://github.com/mkhanhvo/Business-Performance-Overview-Revenue-Profit-Advertising-Impact/blob/c39a0ce72313a10a856f46bd002e7538b2537616/Insight%20-%20Conversion%20rate%20funnel%20(Category%207%20-%20v%C3%A1y%20chi%E1%BA%BFt%20eo%20%C3%B4m).png)

- Set quan ao (*clothing sets*): significant drop at Comment/Inbox → Order, typically below 15%

![image alt](https://github.com/mkhanhvo/Business-Performance-Overview-Revenue-Profit-Advertising-Impact/blob/c6b8fdbab92b15130bd7b583cfdf9bea30123414/Insight%20-%20Conversion%20rate%20funnel%20(Category%205%20-%20set%20qu%E1%BA%A7n%20%C3%A1o).png)
  
+ Separated items (tops, pants, skirts): good engagement but low and unstable order conversion.

![image alt](https://github.com/mkhanhvo/Business-Performance-Overview-Revenue-Profit-Advertising-Impact/blob/c6b8fdbab92b15130bd7b583cfdf9bea30123414/Insight%20-%20Conversion%20rate%20funnel%20(Category%202%20-%20%C3%A1o%20t%C3%A1ch%20set).png)

![image alt](https://github.com/mkhanhvo/Business-Performance-Overview-Revenue-Profit-Advertising-Impact/blob/c6b8fdbab92b15130bd7b583cfdf9bea30123414/Insight%20-%20Conversion%20rate%20funnel%20(Category%204%20-%20qu%E1%BA%A7n%20t%C3%A1ch%20set).png)

![image alt](https://github.com/mkhanhvo/Business-Performance-Overview-Revenue-Profit-Advertising-Impact/blob/c6b8fdbab92b15130bd7b583cfdf9bea30123414/Insight%20-%20Conversion%20rate%20funnel%20(Category%203%20-%20ch%C3%A2n%20v%C3%A1y%20t%C3%A1ch%20set).png)

## Recommendations
- Focus optimization on the purchase decision stage, not media exposure
- Scale waist-flare dresses with tight control
- Keep waist fitted dresses category in a testing phase
- Limit conversion-focused ads for sets and separated items, instead use bundles styling suggestions and conditional promotions

## Overall Conclusion
The campaign did not fail in generating demand or orders; it failed in converting revenue into profit. Advertising effectively drives volume, but misaligned discount strategy and non-selective scaling have created systematic losses. Sustainable improvement requires restructuring discount policies and reallocating budgets based on category-level effectiveness, rather than increasing spend indiscriminately
