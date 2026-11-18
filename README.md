<h1 align="center">Elist Tech: E-commerce Performance Analysis, 2019–2022</h1>
 
<p align="center">
  <b>Analyst:</b> Tram Nguyen &nbsp;|&nbsp; <b>Tools:</b> Excel (cleaning, pivot tables), Tableau (visualization)
</p>
<!-- TODO: add your links on the next line, then delete this comment
<p align="center"><a href="TABLEAU_PUBLIC_URL">Tableau dashboard</a> &nbsp;|&nbsp; <a href="WORKBOOK_URL">Excel workbook</a> &nbsp;|&nbsp; <a href="LINKEDIN_URL">LinkedIn</a></p>
-->
Elist's sales nearly tripled during COVID and then fell back. The only lasting growth came from loyalty members, and that advantage was fading by late 2022. I recommend member-only bundles, an October campaign, and a laptop returns review, and I flag a refund-date error that makes refund trends unreliable.
 
## Contents
- [Project Background](#project-background)
- [Executive Summary](#executive-summary)
- [Deep-Dive Insights](#deep-dive-insights): [Sales](#sales-trends) · [Seasonality](#seasonality) · [Product](#product-performance) · [Region](#region) · [Loyalty](#loyalty-program) · [Refunds](#refunds)
- [Recommendations](#recommendations)
- [Data Quality & Limitations](#data-quality--limitations)
- [Dataset Structure and ERD](#dataset-structure-and-erd)

## Project Background
 
Founded in 2018, **Elist is an e-commerce company that sells popular electronics** (mainly Apple, Samsung, and Lenovo) to a global customer base through its website and mobile app. Customers arrive directly or through email, social media, and affiliate links.

This report analyzes Elist's sales performance from 2019 to 2022 to identify key trends, assess business growth, and understand changes in customer purchasing behavior. By examining sales volume, average order value (AOV), return rates, and loyalty program effectiveness, the report aims to identify opportunities to increase revenue, improve customer retention, and minimize potential losses from returns. These findings will help Elist make data-driven decisions regarding marketing strategies, product performance, and future business growth.
 
**North star metrics**
 
| Metric | 2019 | 2020 | 2021 | 2022 | 2022 vs 2019 |
|---|---:|---:|---:|---:|---:|
| **Total sales** | $3.87M | $10.16M | $9.13M | $4.96M | +28% |
| **Order count** | 14.3K | 28.9K | 30.7K | 19.0K | +33% |
| **Average order value (AOV)*** | $270 | $351 | $297 | $261 | −3% |
| **Loyalty share of sales** | 11% | 29% | 53% | 55% | +44 pts |
| **Refund rate** | 5.7% | 9.2% | 3.6%** | No data** | – |
 
<sub>*AOV = total sales ÷ number of distinct orders. **Refund data for 2021–2022 is incomplete. See [Data Quality & Limitations](#data-quality--limitations).</sub>
 
## Executive Summary
 
Elist's sales nearly tripled in 2020 as COVID-19 pushed shopping online, peaking at **$1.25M in December 2020**, then declined in steps through 2021 and 2022. Sales in 2022 ($4.96M) were still 28% above 2019, but that lasting gain came entirely from **more orders**, since AOV ended about 3% below 2019 ($261 vs $270), and entirely from **loyalty members**.
 
<div align="center">
  <img width="85%" alt=" Monthly sales, 2019–2022, with the December 2020 peak, step-downs and October 2022 low marked" src="https://github.com/user-attachments/assets/2f0b3f54-c88f-4688-b0af-717d66417a82" />
</div>
<p> </p>

**Key insights**

- **Sales:** 2020 growth came from both more orders (+102%) and higher AOV (+30%). Since then, AOV has fallen back slightly below its 2019 level, and orders fell 38% in 2022.
- **Seasonality:** Sales dip below September every **October** and recover in November–December, in all four years. October 2022 was the low of the period at $0.18M.
- **Product:** The 27-inch gaming monitor, MacBook Air and AirPods drive about **84% of sales**. The monitor alone grew to about half of sales by late 2022.
- **Region:** North America is about **half of sales** and held up best in 2022. APAC grew the most since 2019, while LATAM shifted most toward low-price accessories.
- **Loyalty:** Members overtook non-members in early 2021 and made up **55% of 2022 sales**, spending **$27 more per order** ($274 vs $247). Non-member sales are 35% below 2019. However, members fell behind non-members again from September 2022.
- **Refunds:** Laptops are refunded most often (about 1 in 6 orders in 2019–2020). Refund dates appear shifted by about 2 years, so refund trends after 2020 are unreliable.

**Top 3 recommendations**

1. **Grow the loyalty program through the Direct and Email channels.** Offer member-only bundles built around AirPods and monitors, and offer membership at checkout to AirPods, cable, and laptop buyers. Members spend $27 more per order, so closing that gap on the roughly 9K non-member orders in 2022 would be worth about $0.25M a year (rough estimate).
2. **Run an October campaign.** October made up only 3.6% of 2022 sales, against its usual 7–8%. Holding the usual share would have added roughly $170–220K (rough estimate).
3. **Review laptop returns, starting in North America, and fix the refund data** before any refund KPI is reported.
---
 
## Deep-Dive Insights
 
### Sales Trends
 
<div align="center">
  <img width="80%" alt="Total sales by year, 2019–2022" src="https://github.com/user-attachments/assets/c673476e-d1d1-4611-88f6-f7582044a3b3" />
</div>

- **2020: everything surged.** Sales grew 163% to $10.16M, AOV rose 30% to $351, and orders doubled (+102%). More customers were buying and spending more per order during pandemic-driven online shopping.
- **2021: orders kept growing, but baskets got smaller.** Orders rose 6% to a peak of 30.7K, while AOV fell 15% to $297, so sales dropped 10% to $9.13M. Customers bought fewer high-price products and more low-price ones.
- **2022 vs 2019: the business normalized on a larger base.** Sales were 28% above 2019 and orders 33% above, while AOV fell 12% in 2022 to $261, about 3% below 2019. The [Loyalty Program](#loyalty-program) section shows where this lasting gain came from: loyalty members grew, while non-member sales fell below 2019.

<div align="center">
  <img width="48%" alt="AOV by year, 2019–2022" src="https://github.com/user-attachments/assets/421ce22a-982c-4001-871c-907f364fb1b5" />
  <img width="48%" alt="Order count by year, 2019–2022" src="https://github.com/user-attachments/assets/b03d7b43-a284-45af-bea9-1e3a5b5f3f62" />
</div>

### Seasonality
 
The monthly sales chart in the [Executive Summary](#executive-summary) shows three step-downs:
 
- **Sales peaked in December 2020 at $1.25M, and the decline started right after.** Sales fell to about $0.71M by February 2021 and stayed at roughly $0.6–0.9M through 2021.
- **A second step-down came in early 2022.** Sales fell from about $0.88M in December 2021 to $0.47M in February 2022, then held at about $0.35–0.5M.
- **October 2022 was the low point of the period at $0.18M,** followed by a partial holiday rebound in November–December 2022.

<div align="center">
  <img width="85%" alt="Each month's share of the year's sales, one line per year, 2019–2022" src="https://github.com/user-attachments/assets/f5bf4938-fd6b-45bb-9851-ae72088cd130" />
</div>

- **October falls below September in every year, and November–December (the holiday season) always recover.** This suggests a September promotion pulls demand forward, or customers wait for Black Friday.
- **October 2022 was extreme.** It made up only 3.6% of 2022's sales, about half its usual share of 7–8%. 2022 also never reached its usual holiday level: December was 5.3% of the year's sales, versus about 12% in 2019–2020.
- **December was the best month in 2019 and 2020,** but in 2021 and 2022 January was the strongest month. Sales declined throughout those years, so the December holiday boost wasn't enough to make up for the drop since January.
- **The February dip is not consistent.** February was weak in 2019 and 2020 but close to average in 2021–2022. Averaged over the four years, February's sales per day (about $17K) are also slightly higher than October's (about $16K), so **October is the main seasonal weak spot**.

### Product Performance
 
<div align="center">
  <img width="80%" alt="Sales share by product, monthly, 2019–2022" src="https://github.com/user-attachments/assets/833ac49a-858e-4ea2-a1fd-033052e0e361" />
</div>

- **Three products drove about 84% of sales:** the 27-inch gaming monitor ($9.8M), MacBook Air ($7.7M), and AirPods ($6.2M). ThinkPad laptops made up most of the rest.
- **The long tail is very small.** iPhone, Bose headphones, the Samsung webcam, and charging cables are a thin slice of sales. Bose had the lowest revenue, about $3K in total, with no sales at all in some months.
- **Concentration risk is rising.** The monitor's share of sales grew from about 30% in 2020 to about 50% by December 2022, partly because other products shrank.
- **MacBook Air explains the AOV swing.** Its share of sales jumped from about 15% to about 30% in 2020 and then declined again, matching the rise and fall of AOV.

<div align="center">
  <img width="80%" alt="Order share by product, monthly, 2019–2022" src="https://github.com/user-attachments/assets/2b8e59ac-57c4-49e1-9629-32771956b498" />
</div>

- **Volume products and revenue products are different.** AirPods (~$160) and charging cables (~$20) make up most orders but little revenue per order. MacBook Air and ThinkPad are a small share of orders but a large share of revenue.
- **The monitor is both:** about 20% of orders and the largest revenue product. Its order share rose to about 29% by the end of 2022.
- **Samsung webcams,** launched in 2020, grew to about 10% of orders in 2021–2022. iPhone and Bose had the lowest order and sales shares in every year.

<div align="center">
  <img width="80%" alt="Order share by category, quarterly, 2019–2022" src="https://github.com/user-attachments/assets/9675d46b-98b8-44d1-9171-2fee2873040c" />
</div>

- **Headphones are the largest category by orders but are losing ground.** Their order share fell from 46–49% (2019–2020) to 41–43% (2021–2022).
- **Accessories grew, then reversed.** Their order share rose from 21% to a peak of 35% in Q2 2022, then fell back to 27% by Q4 2022. Each accessory order is worth little, so this growth pulled AOV down.
- **Monitors are the steadiest category,** at about 21–22% of orders every year, rising to 26% in Q4 2022, the highest of the period.
- **Laptops have an outsized effect on revenue.** They are only 4–9% of orders, but each is worth over $1,000. Their share doubled in 2020 (to 8–9%) and then fell back to about 5%.

### Region
 
<div align="center">
  <img width="80%" alt="Total sales by region and year, 2019–2022" src="https://github.com/user-attachments/assets/dd209dc8-4c6f-44d3-acac-92fe1316ac33" />
</div>

- **The COVID cycle was global.** Every region rose sharply in 2020 and fell in 2022, so this was a market-wide effect, not a regional problem.
- **NA is about half, and the 2021 dip came from NA**. Total sales fell about $1.0M, and the NA line dropped from about $5.3M to $4.5M in 2021, while the other three stayed almost flat.
- **APAC grew the most,** from about $0.42M in 2019 to $0.62M in 2022 (+48%).

<div align="center">
  <img width="80%" alt="Order share by category within each region, 2019–2022" src="https://github.com/user-attachments/assets/63d0357a-111e-41e1-9602-9fd1e7016432" />

</div>

- **APAC is shifting toward monitors.** Its monitor share rose every year, from 21% in 2019 to 25% in 2022 of orders, the highest of any region.
- **NA drives the global shift toward accessories.** NA's accessories share rose from 25% (2019) to 34% (2022) of orders, while headphones fell from 48% to 41%.
- **LATAM moved most toward cheap products.** Accessories went from about 30% to 50% of orders, while headphones fell from 45% to 30%, monitors from 19% to 16%, and laptops to about 4%. This cheaper mix coincided with LATAM's steepest 2022 drop (−56%), though its small sales base makes shares less stable.

### Loyalty Program
 
**The big picture:** loyalty members grew from $0.42M in sales (2019) to $2.72M (2022), while non-member sales fell from $3.45M to $2.24M (−35% vs 2019). **All net growth since 2019 came from loyalty members.** In 2022, members spent **$27 more per order** than non-members ($274 vs $247). Member AOV rose 6% since 2019 ($260 → $274), while non-member AOV fell 9% ($272 → $247).
 
<div align="center">
  <h4>Sales</h4>
  <img width="80%" alt="Loyalty vs non-loyalty share of sales, monthly, 2019–2022" src="https://github.com/user-attachments/assets/aef01d95-11d1-48ee-9833-c54982b5b9d9" />
  <h4>Order count</h4>
  <img width="80%" alt="Loyalty vs non-loyalty order count, monthly, 2019–2022" src="https://github.com/user-attachments/assets/58cbee54-02a6-4e04-86a8-b93274b40f7a" />
  <h4>AOV</h4>
  <img width="80%" alt="Loyalty vs non-loyalty AOV, monthly, 2019–2022" src="https://github.com/user-attachments/assets/6b3ec3d3-4ef5-4ee2-85b0-15a9ede53c1a" />
</div>

- **Inflection point: members overtook non-members in orders first (December 2020), then in sales three months later (March 2021).** Member AOV only passed non-member AOV in June 2021, so until then members needed more orders to match non-members in sales.
- **Members led for about 18 months.** From spring 2021 to August 2022, they made up about 50–63% of sales, and from June 2021 they also spent more per order.
- **The 2020 AOV spike came from non-members.** Non-member AOV jumped 48% to $402 in 2020, peaking near $595 in December 2020, likely from one-time laptop buyers. Member AOV barely moved for the year ($260 → $269) and stayed in a narrow $260–290 yearly range across all four years.
- **Both groups' orders fell from early 2021, but members fell faster in late 2022.** Member orders dropped from about 1,650 a month at the early-2021 peak to about 250 in December 2022. Non-members ended at about 470. From September 2022, non-members led again in orders, sales, and AOV.
  
**Why AOV rose for members but fell for non-members:** members shifted toward monitors (17% → 21% of member orders) and webcams, while non-members shifted toward $20 charging cables. Laptop buyers, the highest-value customers who drove non-member AOV in 2020, mostly never joined the program (see [What Direct and Email customers buy](#what-direct-and-email-customers-buy)).
 
#### What drove the inflection: marketing channel
 
<div align="center">
  <h4>Share of loyalty orders by channel</h4>
  <img width="80%" alt="Channel mix of loyalty orders by year: Direct 62–76%, Email 21–34%" src="https://github.com/user-attachments/assets/df5657b7-8a60-43ff-a8a8-0306d9a312d1" />


  <h4>Loyalty share of each channel's orders</h4>
  <img width="80%" alt="Loyalty share of orders by marketing channel, quarterly, 2019–2022" src="https://github.com/user-attachments/assets/4d33edfe-83fa-446c-8555-973171fafcb5" />

</div>

- **Direct is where most members buy.** Direct brings in 62–75% of loyalty orders and Email 21–32%. Social Media is only about 1–4% and Affiliate about 1%.
- **Email and Social Media customers joined first.** Both passed a 50% loyalty share in early 2020 (Social Media in Q1 2020 at 56%, Email in Q2 2020 at 63%), and Email peaked at 73% in Q4 2020. These channels likely reach customers who already know the brand.
- **Direct customers decided the crossover.** They joined more slowly (23% in Q1 2020 → 40% in Q4 2020 → 53% in Q1 2021). Because Direct is the largest channel, members only became the majority overall once Direct passed 50%, matching the overall crossover (December 2020 for orders, March 2021 for sales).
- **Something happened in Q1 2021.** Almost every channel jumped that quarter: Direct 40% → 53%, Affiliate 14% → 33%, Social Media 49% → 69%. Check whether there was a loyalty promotion or a sign-up change then.
- **Affiliate customers rarely join.** Their loyalty share never went above 36%.
- **The 2022 decline hit every channel, and Direct the hardest.** Direct fell from 55% to 34% between Q2 and Q4 2022, and Email from 57% to 48%.

#### What drove the inflection: region
 
<!-- TODO: add the "Loyalty share of orders by region" chart here -->
<div align="center">
  <img width="80%" alt="Loyalty share of orders by region" src="https://github.com/user-attachments/assets/ac2f44e2-4f01-4f96-b67e-5aa6d79ec3d5" />
</div>

 
- **Loyalty grew at the same pace in every region,** from under 5% in early 2019 to about 47–58% by 2021. So the inflection was **company-wide, not regional**, and it showed up mainly through the Direct and Email channels.
- **NA held up best in late 2022** (still 42% in Q4 2022), while **LATAM fell first and furthest** (54% in Q3 2021 → 26% in Q4 2022).

#### What Direct and Email customers buy
 
<div align="center">
  <img width="80%" alt="Product mix of Direct and Email orders, loyalty vs non-loyalty, 2021–2022" src="https://github.com/user-attachments/assets/b5d1a23a-e90b-4276-aba3-52bf624ea850" />
</div>

- **In Direct, members are AirPods buyers.** AirPods make up about 62% of Direct member orders, about twice the share among Direct non-members (27–31%). AirPods are the main product that brings Direct customers into the program.
- **Email members buy the highest-value mix.** Monitors are about 29% of Email member orders, the highest monitor share of any group, with webcams adding about 21% and headphones about 35%.
- **Non-members mostly buy the $20 charging cable.** It makes up 34–36% of Direct non-member orders and 65–67% of Email non-member orders, while members rarely buy it (about 1–2% in Direct, 12–14% in Email). Email reaches many non-members, but mostly for very low-value purchases.
- **Laptop buyers don't join the program.** MacBook Air is 4–7% of Direct non-member orders but only about 1–2% of member orders. These are the highest-value customers, and they explain the 2020 non-member AOV spike.
- **Webcams are a member product.** They make up 10–21% of member orders in both channels, compared with 4–10% for non-members.
### Refunds
 
<div align="center">
  <img width="80%" alt="Refund count and refund rate by product and year, 2019–2022" src="https://github.com/user-attachments/assets/23ba95a4-157d-449d-b2ee-464b4537ce66" />
</div>
 
- **Refunds spiked in 2020.** The refund rate rose from 5.7% to 9.2%, and the number of refunds more than tripled (965 → 3,120).
- **AirPods and monitors drove refund volume** (1,529 and 820 refunds in 2020), but **laptops had the highest refund rates:** MacBook Air (18.3% in 2019, 16.9% in 2020) and ThinkPad (17.1%, 17.0%), about 1 in 6 orders.
- **Accessories were rarely returned.** Charging cables had refund rates of 2.4–2.6% in 2019–2020. Bose shows 0%, but its sales volume is too low for that to be meaningful.
- **2021 and 2022 refund figures are incomplete.** 2022 shows no refunds at all, and the 2021 drop is likely missing data, not a real improvement (see the time-to-refund analysis below). Compare refund rates only between 2019 and 2020.
#### Time to refund
 
<div align="center">
  <img width="80%" alt="Histogram of days from delivery to refund by purchase year, 2019–2021" src="https://github.com/user-attachments/assets/8f9b5c61-e16a-4912-82bf-837ed40fe95e" />
</div>

- **Refund dates appear shifted by about 2 years.** In every purchase year (2019–2021), refunds are recorded about 680–800 days after delivery, with none earlier. Real refund timing would vary and include early returns, and the pattern is the same before and during COVID, so this points to an error in the refund timestamp rather than customer behavior.
- **This likely explains the missing refunds.** Refunds for 2022 orders would fall in 2024, after the data ends, and many refunds for 2021 orders would also be missing.
#### Why laptops are refunded more
 
<div align="center">
  <img width="80%" alt="MacBook Air and ThinkPad refund rates by region, marketing channel, platform and loyalty status, 2019–2021" src="https://github.com/user-attachments/assets/12dafeb6-a3ae-45f7-8fb5-c8000403f7dd" />
</div>

- **Laptop refunds are a product issue, not a channel issue.** MacBook Air and ThinkPad are refunded at about 13–15% in every channel with enough orders, and on the website, where almost all laptops are sold. (This is lower than the 17–18% for 2019–2020 above because 2021 refund data is incomplete.)
- **North America has the highest laptop refund rates** (MacBook ~15%, ThinkPad ~17%), compared with about 9–13% in EMEA and LATAM. NA is also the biggest laptop market, so its returns cost the most.
---
 
## Recommendations
 
### Sales & Seasonality
- **Use bundles to lift AOV above $230.** AOV hasn't grown since 2019, so bundles (see Loyalty below) and checkout upsells are the main lever. Track AOV monthly.
- **Fix October.** It is the weakest month every year and fell 55% in 2022. Run October-specific promotions, and avoid ending September campaigns abruptly so demand holds until the holiday season.
- **Prepare for November–December** with inventory and marketing campaigns in place ahead of the holiday peak.
### Product
- **Keep monitor stock secure, but reduce dependence on it.** The monitor is now about half of sales, so any supply or demand problem would hit revenue hard.
- **Bundle low-price accessories** such as charging cables and webcams with laptops and monitors to raise basket value.
- **Review Bose headphones and iPhone** before deciding whether to promote them, reduce inventory or discontinue them.
### Region
- **Protect and grow North America,** the largest and most resilient region.
- **Prioritize LATAM for further investigation** into its 56% sales decline in 2022 and its shift toward low-price products, and test monitor and headphone bundles there.
- **Promote monitors in APAC,** where monitor order share is rising (20.8% → 24.7%), and repeat the approach in other regions.
- **In NA, bundle accessories with laptops or monitors** to raise revenue per order.
### Loyalty Program
**Grow member spending with member-only bundles**
- **Email members: promote monitors and webcams.** These are already what Email members buy, so targeted campaigns should work well and lift AOV.
- **Direct members: build bundles around AirPods**, which make up about 62% of Direct member orders:
  - **AirPods + webcam:** Direct members already buy webcams (about 13% of their orders), and a webcam adds about $50 per order vs about $20 for a cable.
  - **AirPods buyers + monitor discount:** members already buy monitors (about 19% of Direct and 29% of Email member orders), so this has the biggest potential effect on AOV.
- **Test first:** offer bundles to part of Direct and Email members, and compare bundle take-up rate and member AOV with members who don't see the offer.
**Convert non-members with sign-up incentives at checkout**
- **Direct: use AirPods to convert non-members.** Direct non-members already buy AirPods (27–31% of their orders), so offer membership at AirPods checkout (member pricing or bonus points), and advertise the member-only bundles.
- **Email: turn cable buyers into bigger orders.** Two-thirds of Email non-member orders are $20 cables. Test "join and get a free cable", or bundle the cable with AirPods or monitors.
- **Offer membership to laptop buyers.** MacBook buyers are high-value but rarely join. A membership offer at laptop checkout (extended warranty, accessory discount) could keep them buying.
- **Investigate the late-2022 decline in member orders**, starting with the Direct channel, where the member share fell most: track repeat-purchase rate and churn, and check whether program benefits changed.
### Refunds
- **Review laptop returns** (product defects, shipping damage, mismatches between product descriptions and customer expectations), starting in North America, the largest laptop market.
- **Fix refund data before reporting refund KPIs.** Ask the data engineering team to verify the refund timestamps and recover the missing 2021–2022 refunds.
---
 
## Data Quality & Limitations
 
- **Refund dates appear shifted by about 2 years,** so 2022 shows no refunds and 2021 refunds are incomplete. Refund rates by product and region (2019–2020) are still usable; refund trends over time are not.
- **MacBook Air loyalty orders show a 0% refund rate on 134 orders,** which is unusual compared with about 14% for non-members. Verify with the data engineering team.
- **AOV is calculated as total sales ÷ distinct orders.** The source data has more rows (108,127) than distinct orders (92,930), so dividing by rows would understate AOV by about 14%.
- **iPhone data is missing for October–November 2022** (impact about $5–10K).
- **The "Unknown" marketing channel rises to about 5% of loyalty orders in 2022,** which suggests missing channel data.
- **No cost or margin data,** so the profitability of products, regions, and the loyalty program could not be assessed.
---
 
## Dataset Structure and ERD
 
The core dataset has **108,127 rows** across orders, order status, customers, products, and geographic tables.
 
<div align="center">
  <img width="85%" alt="Entity relationship diagram of the Elist dataset" src="https://github.com/user-attachments/assets/6e2f221a-909a-4165-9ded-dd4acdec4393" />
</div>
 
