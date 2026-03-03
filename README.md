<img width="1199" height="654" alt="image" src="https://github.com/user-attachments/assets/af69ee26-a612-4555-a653-671f2e794d2c" />

# 📊 Advertising Campaign Performance & Profitability Analysis

### Author: Vo Tran Mai Khanh
### Date: 12/2025
### Tools Used: Power Query, PBI

## 📌 Background & Overview  

### 📖 Objective:
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

### 👤 Client Background
The business operates in the Vietnamese fashion market with nationwide coverage. This project focuses on analyzing online marketing campaigns for the women’s fashion category across 62 cities and provinces, spanning Northern to Southern Vietnam, the campaigns were conducted over a one month period and have entered the review stage. The analysis evaluates campaign performance based on revenue contribution, effectiveness across products and the efficiency of marketing spend allocation. The objective is to support data driven decisions on whether to maintain or adjust campaign setups, budget distribution, creative strategies and overall marketing execution

## 📂 Dataset Description & Data Structure  

### 📊 Data Source  
- Source: dataset including order records (Direct vs Ads), campaign spending distribution and product dimension tables, enabling performance and profitability analysis at channel and product levels
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
### 1️⃣ Empathize 

<img width="641" height="337" alt="image" src="https://github.com/user-attachments/assets/29083f73-25f2-4cf8-a652-7c04bdf4ed04" />

### 2️⃣ Define point of view 

<img width="938" height="302" alt="image" src="https://github.com/user-attachments/assets/a5062b81-2b15-4a84-939a-8e30b6ac059f" />

### 3️⃣ Ideate  

<img width="1052" height="206" alt="image" src="https://github.com/user-attachments/assets/e3148cb8-2ee2-4c9e-8b91-51e8c7cfa9ba" />

## 📊 Key Insights & Visualizations  

### 1️⃣ Overview - Budget & Return

During 31 day campaign period, advertising played a central role in order generation by contributing 1,958 out of 2,858 orders (68.5%) and approximately 3 billion VND out of 5 billion VND in total revenue. However, profitability did not scale with sales volume: more than 60% of campaign days recorded negative profit and the ads channel alone showed negative profit on 22 out of 31 days (~70%), despite maintaining positive revenue

<img width="812" height="523" alt="image" src="https://github.com/user-attachments/assets/a270fdb7-17dd-479b-bccb-01474cb2714a" />

#### *Revenue by Channel*

<img width="392" height="247" alt="image" src="https://github.com/user-attachments/assets/1e41dbf8-20fb-4eb5-884e-0a79b84b1ca6" />

#### *% Budget used and ads profit by day*

<img width="387" height="244" alt="image" src="https://github.com/user-attachments/assets/45ccb705-2762-497f-84fe-314729c3d536" />

Deeper analysis indicates that the core issue is a uniform and prolonged discount policy applied across categories. This policy resulted in systematic profit losses across both ads and direct sales channels. At the same time, conversion performance varies significantly by product category, suggesting that budget allocation and sales strategy should be category specific rather than evenly distributed

#### *Discount impact on profit from ads channel*

<img width="674" height="209" alt="image" src="https://github.com/user-attachments/assets/2e4806ec-9dee-4ff6-bdb1-9584ff9bcbe3" />

#### *Discount impact on profit from direct channel*

<img width="672" height="209" alt="image" src="https://github.com/user-attachments/assets/e175a7c8-b9a5-4dc5-8f0e-5a45c7cd896c" />

### 📌 Analysis 1. Budget Control & Spending Efficiency
Budget utilization was well controlled for over 86% of the campaign duration, Only 13.33% of total days exceeded budget, mainly during the mid and late stages of the campaign

<img width="387" height="244" alt="image" src="https://github.com/user-attachments/assets/089872d6-62ad-40f6-8854-3a1d51614794" />

However, comparison between ads spend, ROAS and revenue shows no clear linear relationship. This indicates that budget level alone is not the primary driver of performance
- High ROAS and revenue days did not consistently coincide with overspending days
- Several days with controlled spending still delivered weak performance

<img width="425" height="269" alt="image" src="https://github.com/user-attachments/assets/164a7164-c20c-4932-b0da-28868f4f56b7" />

### Recommendations
- Avoid optimizing performance solely by increasing or tightening budgets
- Incorporate creative quality, product category and campaign timing when making scaling decisions

### 📌 Analysis 2. High Ads Revenue but Weak Profitability
- Out of 2,858 total orders, **1,958 orders (68.5%) were generated through ads,** confirming ads as the primary order driving channel. However, when comparing ads spend and ads profit, **over 60% of ad days recorded negative profit regardless of spend level.** Ads successfully generate volume but fail to deliver consistent profitability
- From a daily perspective: only 29% of days (9/31) were profitable overall. For ads channel specifically, there were 22 days showed negative profit, only 5 days were profitable while the remaining days recorded zero or negative revenue

<img width="425" height="266" alt="image" src="https://github.com/user-attachments/assets/cc423335-4c77-4f4f-a8bb-a48856dddcfc" />

### Recommendations
- Shift ads evaluation from revenue generated to revenue generated under a profitable cost structure
- Treat ads as a conditional sales enabler, not a channel for unrestricted scaling

### 📌 Analysis 3. Systematic Profit Loss by Category
Category × channel analysis shows: 03 product categories including Apparels *(Ao tach set)*, Standalone skirts (*Chan vay tach set*) and Standalone pants *(Quan tach set)* are the primary drivers of negative profit, **recording losses in both ads and direct sales for over 80% of campaign days**

#### *Profit performance and channel contribution analysis of category Apparel *(Ao tach set)**

![image alt](https://github.com/mkhanhvo/Business-Performance-Overview-Revenue-Profit-Advertising-Impact/blob/e360001bdb2216be9f2a8da18d3c7503619a4e7f/Overall%20-%20Revenue%20%26%20Profit%20by%20category%20Ao%20Tach%20Set.png)

#### *Profit performance and channel contribution analysis of category Chan vay tach set (*Standalone skirts*)*

![image alt](https://github.com/mkhanhvo/Business-Performance-Overview-Revenue-Profit-Advertising-Impact/blob/e360001bdb2216be9f2a8da18d3c7503619a4e7f/Overall%20-%20Revenue%20%26%20Profit%20by%20category%202%20(Chan%20Vay%20Tach%20Set).png)

#### *Profit performance and channel contribution analysis of category Quan tach set (*standalone pants*)*

![image alt](https://github.com/mkhanhvo/Business-Performance-Overview-Revenue-Profit-Advertising-Impact/blob/e360001bdb2216be9f2a8da18d3c7503619a4e7f/Overall%20-%20Revenue%20%26%20Profit%20by%20category%203%20(Quan%20Tach%20Set).png)

Other categories experience negative profit for less than 10% of campaign duration. Discount rate is the direct cause of negative profit across all advertised categories, regardless of sales volume or revenue. All categories record negative profit in both ads and direct sales confirming tha the issue is not channel related, not driven by scale but rooted in pricing and discount policy

#### *Profit trends move in the same direction across channels*

<img width="386" height="242" alt="image" src="https://github.com/user-attachments/assets/d6277e2e-d002-415b-a97b-16a637a15cad" />

### Recommendations
- Review and adjust discount levels by category instead of applying a uniform policy
- Reduce discounts for high-volume but high-loss categories to prevent scaling losses
- Prioritize profit per order stability before pushing for higher sales volume

### 2️⃣ Adsvertising Campaign Effectiveness & Profitability

<img width="882" height="517" alt="image" src="https://github.com/user-attachments/assets/29b7b65f-4e1d-43fa-bdab-1f69efe41ce5" />

### 📌 Analysis 1. Revenue Concentration & Campaign Level Performance
Ads revenue is highly concentrated in a small number of core campaigns: top 5 revenue generating campaigns are mainly driven by Audrey LAL, Flowers Make My Day, Anivan Dress and Margnet Dress
- Category Vay Chiet Eo Xoe (*waist-flare dresses*) account for over 50% of revenue in the Flowers Make My Day campaign
- In contrast, clothing sets generate almost no revenue within these high-performing campaigns

#### *Top 5 campaigns drive revenue*

<img width="411" height="297" alt="image" src="https://github.com/user-attachments/assets/8722c978-a3f2-4dfc-8fea-82cddb1817ca" />

#### *Lowest Performing Campaigns by Ad Revenue* 

<img width="413" height="296" alt="image" src="https://github.com/user-attachments/assets/682f876d-4672-4f39-b4d7-2c4576b848cf" />

### Recommendations
- Reallocate budgets from low performing campaigns and categories toward proven core campaigns
- Prioritize spending during validated high-performance periods (Weeks 4–5) rather than scaling early
- For the 4% of zero-revenue campaigns, optimize creatives or targeting before elimination

### 📌 Analysis 2. Conversion Performance by Category
**Overall funnel trends:**
CTR remains stable at 0.6% - 1.0%, Click → Comment/Inbox rates are high (25% - 40%), indicating strong initial interest. However, Click → Order conversion is only 10% - 23%, showing friction at the purchase decision stage

**Budget scaling:**
- Does not improve conversion cost
- Conversion cost remains flat or increases slightly as spend grows
- CPM ranges between 60K–100K with no meaningful decline as impressions increase

**Category level highlights**

**Waist flare dresses *(*Vay chiet eo xoe*)*:** stable funnel, Click → Order ~20%+, conversion cost does not worsen with increased spend

<img width="1003" height="180" alt="image" src="https://github.com/user-attachments/assets/a0f62f29-a476-4866-bcf4-2105f749ea3f" />

**Waist fitted dresses *(*Vay chiet eo om*)*:** good engagement but unstable conversion efficiency

<img width="998" height="176" alt="image" src="https://github.com/user-attachments/assets/baa388c1-ad76-4341-a10b-9e8b8e66cb4e" />

**Clothing sets *(*Set quan ao*)*:** significant drop at Comment/Inbox → Order, typically below 15%

<img width="1000" height="180" alt="image" src="https://github.com/user-attachments/assets/5e9cdcaa-35c7-4b12-a610-047b04a41661" />

**Separated items (tops, pants, skirts):** good engagement but low and unstable order conversion.

<img width="1006" height="180" alt="image" src="https://github.com/user-attachments/assets/5e1a683a-43a2-4835-905e-f23a8e0ee874" />

<img width="1002" height="179" alt="image" src="https://github.com/user-attachments/assets/fdeb30c5-4f20-4b06-bfff-5b0fd118b0c2" />

<img width="1001" height="176" alt="image" src="https://github.com/user-attachments/assets/6976f65f-1960-4e80-a7b8-4bca749e616e" />

### Recommendations
- Reallocate budget from near zero revenue campaigns to validated top performers but scale only after confirming sustainable ROAS and margin contribution
- Establish a minimum performance threshold (revenue + profit-adjusted ROAS) to automatically pause inefficient campaigns and reduce budget leakage
- Reduce dependency on a small number of revenue driving campaigns by strengthening mid tier performers with stable conversion efficiency
- Shift strategic focus from traffic expansion to purchase stage optimization, as Click → Order conversion (10–23%) remains the primary bottleneck despite strong engagement
- Improve pricing structure, discount depth and offer clarity for low conversion categories before increasing spend
- Scale only categories with stable conversion cost and margin sustainability, avoid expanding budget where conversion efficiency does not improve with volume

### 3️⃣ Sales & Product Performance Analysis 

<img width="856" height="540" alt="image" src="https://github.com/user-attachments/assets/3a8fd301-0dd0-46d4-aab8-3c72564c54a7" />

### 📌 Analysis 1. In terms of ROAS:
- Category Vay Chiet Eo Om (*waist-fitted dresses*) recorded the highest ROAS (22.9), peaking in Weeks 4–5
- Campaigns launched earlier (Weeks 1–3) did not achieve comparable efficiency
- Out of 175 campaigns, only 7 campaigns (~4%) generated zero revenue, indicating that poor performance is not driven by widespread campaign failure.

#### *ROAS and weekly camplaigns run by category*

<img width="761" height="231" alt="image" src="https://github.com/user-attachments/assets/d3143994-ad79-43e3-8017-72922c08b016" />

### Recommendation
- Scale high ROAS categories selectively, particularly Váy Chiết Eo Ôm, while validating sustainability of late week spikes before aggressive budget expansion
- Re-evaluate early phase campaign structure, optimizing targeting and creatives to improve efficiency in Weeks 1–3
- Since zero-revenue campaigns are minimal (~4%), focus on performance optimization rather than campaign elimination, refining underperforming segments instead of broad cuts

### 📌 Analysis 2. Weekly Order Trend & Channel Dynamics:
Across the 5-week campaign, both Ads and Direct Sales show a clear growth pattern followed by a decline in the final week, with Ads consistently driving higher order volume. The strongest acceleration occurred from Week 1 to Week 2, where **Ads orders surged by +296% (112 to 443) and Direct Sales increased by +157% (84 to 216)**, indicating the campaign’s initial impact phase. Growth then **stabilized in Week 2 to Week 3,** with **Ads rising only +6% and Direct Sales +1%,** suggesting performance plateauing

Momentum picked up again in Week 3 to Week 4, particularly for **Direct Sales (+28% vs. Ads +8%),** **reflecting improved channel balance.** However, Week 4 to Week 5 marked a contraction, **with Ads declining –5% and Direct Sales dropping more sharply at –13%,** **signaling late stage fatigue.** Overall, while Ads remains the dominant volume driver, Direct Sales exhibits greater volatility and stronger relative swings, implying that channel performance dynamics shift throughout the campaign lifecycle rather than growing linearly

<img width="1026" height="208" alt="image" src="https://github.com/user-attachments/assets/90c21196-7cdb-471f-b040-e6d6bc71a334" />

### Recommendation
- Implement campaign refresh cycles before Week 5 to mitigate late-stage fatigue (creative rotation, offer variation)
- Leverage Ads for acquisition momentum in early phases, then strengthen Direct Sales activation in mid to late campaign stages to stabilize volume
- Introduce performance checkpoints weekly to adjust budget dynamically rather than waiting until decline appears

### 📌 Analysis 3. Campaign Volume vs ROAS Efficiency
The relationship between ad spend and revenue contribution shows uneven efficiency across categories. While **Áo Tách Set combines high spend (~$100M+) with over 80% contribution**, other high spend categories such as Váy Chiết Eo Xòe deliver only around 65%, indicating weaker marginal returns. Several mid and low spend categories remain within the 40–50% contribution range. Overall, **higher spend does not consistently translate into proportionally higher revenue contribution,** suggesting diminishing returns in certain segments and the need for performance based budget allocation

Across categories, **performance is uneven and not directly correlated with campaign volume.** While overall ROAS improved from 5.72 (Week 1) to 9.05 (Week 5), this increase was not driven by a proportional rise in the number of campaigns. For example, in Week 3 several categories reached peak campaign counts, yet overall ROAS remained at 7.55, lower than Week 5 where campaign numbers declined but ROAS climbed to 9.05. Similarly, some categories expanded campaigns from Week 1 to Week 2 without a consistent ROAS lift, indicating that scaling volume alone did not improve efficiency. At the category level, ROAS dispersion is substantial: most categories operate within a 4–11 ROAS range, while Váy Chiết Eo Ôm spiked to 72.19 (Week 4) and 43.67 (Week 5), suggesting outlier driven performance rather than systematic gains

<img width="992" height="220" alt="image" src="https://github.com/user-attachments/assets/fcc63f6d-6cb5-4243-a999-438aed4453cc" />

### Recommendation
- Shift from volume driven scaling to efficiency driven scaling, prioritizing stable 6–11 ROAS categories over outlier spikes
- Consolidate campaigns in mid performing categories to reduce budget fragmentation
- Apply category-specific budget allocation, increasing investment only where marginal ROAS remains stable rather than expanding campaign count broadly
- Monitor diminishing return effects in high spend categories through incremental budget testing

## 🔎 Final Conclusion & Recommendations  

### 1️⃣ Shift KPI from Revenue Growth → Profit Adjusted ROAS
- Evaluate campaigns based on Profit per Order and Margin adjusted ROAS, not revenue alone
- Set minimum acceptable ROAS threshold aligned with break-even margin

### 2️⃣ Category Specific Budget Allocation
- Increase budget only in categories with stable 6–11 ROAS performance
- Avoid scaling based on short term spikes (e.g., Week 4–5 outliers) without validation
- Reduce spend in high volume but structurally loss-making categories

### 3️⃣ Redesign Discount Strategy
- Replace uniform discounting with category level pricing control
- Reduce discount depth in high volume categories to prevent scaling losses
- Protect contribution margin before pushing volume

### 4️⃣ Efficiency Driven Scaling Framework
- Stop expanding campaign count as a growth lever
- Use incremental budget testing to detect diminishing returns
- Consolidate fragmented campaigns to improve budget efficiency

### 5️⃣ Funnel Optimization at Purchase Stage
- Prioritize improving Click → Order conversion (currently 10–23%) by addressing purchase-stage friction rather than increasing traffic volume
- Improve checkout friction
- Test urgency mechanics and offer framing
- Align creative messaging with margin friendly SKUs
