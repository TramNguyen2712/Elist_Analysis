<h1 align='center', front_size=250px>ELIST TECH</h1>
<h2 align='center'>Ecommerce Performance Report 2019-2022</h2>  

<div class='Overview'>
  <h1 align='center'>Overview</h1>
  <p>Founded in 2018, <strong>Elist is an e-commerce company that sells popular electronics products</strong> and has since expanded to a global customer base. Like most e-commerce companies, Elist sells products through its website as well as its mobile app. They use a variety of marketing channels to reach customers, including Email campaigns, SEO, and affiliate links. Over the last few years, their more popular products have been products from Apple, Samsung, and ThinkPad.</p>
  
  <h2> Business Questions </h2>
  <ul style='number'>
    <li><strong>What were the overall trends in sales from 2019-2022?</strong></li>
    <li><strong>What were Elist's monthly and yearly growth rates?</strong></li>
    <li><strong>How is the new loyalty program performing? Should we keep using it?</strong></li>
    <li><strong>What were our refund rates and average order values?</strong></li>
  </ul>
  
  <h2> North Star Metrics </h2>
  <ul>
    <li><strong>Sales trends</strong> - Focusing on key metrics like total sales, number of orders placed, and average order value (AOV) by region, product, and brand. </li>
    <li><strong>Growth rate</strong> - Analyzing growth rates by different dimensions, including sales and AOV.</li>
    <li><strong>Product performance</strong> - Analyzing different product categories, market impact, and refund rates to inform strategic product decisions.</li>
    <li><strong>Loyalty program performance</strong> - Evaluating the effectiveness of the company's loyalty program and providing recommendations to maximize customer engagement and retention. </li>
    <li><strong>Regional results</strong> - Evaluating regional demand and product performance within regions to identify areas for improvement. </li>
  </ul>
    
  
  <h2> Dataset Structure and ERD (Entity Relationship Diagram) </h2>
  <p>The company has a core dataset consisting of orders, order status, customers, products, and geographic information with a total of 108,127 rows.</p>
  <img width="1875" height="1114" alt="image" src="https://github.com/user-attachments/assets/6e2f221a-909a-4165-9ded-dd4acdec4393" />
</div>

<!-- <div class='Summary'>
  <h1 align='center'>Summary</h1>
  <img width="975" height="484" alt="image" src="https://github.com/user-attachments/assets/6b6434a8-db85-4f61-93a4-de2a4ec2bd65" />
  <p>Monthly sales at about $250-370k through 2019 climbed through 2020 to a peak of $1.25M in December 2020 and then dropped during 2021-2022 to the lowest amount of $0.18M in October 2022. </p>

</div> -->

<div class='Insight'>
  <h1 align='center'>Deep-Dive Insight</h1>

  <div class='Sales Trends'>
    <h2>Sales Trends</h2>
    <div align='center'> <img width="1000" height="500" alt="image" src="https://github.com/user-attachments/assets/c673476e-d1d1-4611-88f6-f7582044a3b3" /> </div>
    <p>   </p>
    <p><strong>2020:</strong> Both metrics - total sales, AOV, and order count surged. Sales grew 163% to $10.16M, AOV rose 31% to $300, and order count doubled +101%. More customers are buying and spending more per order due to pandemic-driven online buying.</p>
    <p><strong>2021:</strong> Order volume kept growing 6% to a peak of 35.9K while sales dropped 10% to $9.13M and AOV fell 15% to $255. Customers bought fewer high-price products and more low-price ones. </p>
    <p><strong>2019 vs 2022:</strong> Sales in 2022 are 28% above 2019 and order 33% above, while AOV is unchanged. That raised open questions: Was 2020 a temporary spike, and is the business returning to normal when stores reopened in 2022?</p>
    <p>   </p>
    <img width="400" height="305" alt="image" src="https://github.com/user-attachments/assets/5ebfa3c4-3b1b-4caa-bdb1-65d20e19b2b1" /> <img width="400" height="305" alt="image" src="https://github.com/user-attachments/assets/b0e97f91-52eb-4c0f-b747-e208abd27e54" />
  </div>

  <div class='Growth Rate'>
    <h2>Seasonality</h2>
    <img width="975" height="563" alt="image" src="https://github.com/user-attachments/assets/b50d15ef-cbf1-4ac5-a88b-4a134f6d2a13" />
    <p>   </p>
    <p>September peaked, followed by an October crash every year. Sales fell every October: -18% (2019), -24% (2020), -26% (2021), and -55% (2022), while September was usually strong just before. Check whether any promotions or campaigns end in September and pull demand forward, or whether customers hold off until Black Friday</p>
    <p>November and December are holiday peaks in four years. Sales rose about 11-35% in November and again in December every year (Black Friday, Christmas, New Year). December is the best performance overall.</p>
    <p>February underperformed during 2019-2022. February sales dropped about 30% every year except in 2020 (+4%). On a per-day sales basis, February (~$67K/day) beat October (~$64k/day), so October is the weakest month. </p>
    <img width="482" height="305" alt="image" src="https://github.com/user-attachments/assets/09068e07-d52f-413d-adb1-cb813532af3e" /> <img width="482" height="305" alt="image" src="https://github.com/user-attachments/assets/ce8c3a16-4198-474d-955f-7e46c8b9b00b" />
    <p>    </p>
    <p>Order volume drives monthly sales. In most months, order growth and sales growth move in the same direction, and the largest fluctuations in sales are also reflected in order volume. The average order value (AOV) typically fluctuates within a range of +- 5%, and there are months when AOV does not move in the same direction as sales, so AOV rarely explains monthly sales changes.</p>
    <p>March 2020 saw the largest surge in orders. Orders increased by approximately 47% along with a 50% increase in sales, matching the start of COVID-19 lockdowns.</p>
    <p>Average order value (AOV) increased by approximately 18% in September 2022 - the largest increase - followed by a decrease of approximately 16% in October 2022 - the largest drop - coupled with a -28% drop in orders, resulting in a -55% decrease in sales.</p>
    <p>Sales increased by 17% in November and 26% in December 2022; AOV rose about 3-5%, but orders decreased slightly (approximately -8% and -3%), so the recovery came from larger orders, not from a higher number of orders in late 2022</p>


  </div>

  <div class='Product Performance'>
    <h2>Product</h2>
    <img width="975" height="566" alt="image" src="https://github.com/user-attachments/assets/040053f1-ec5b-473b-a92a-f9f832d14638" />
    <p>  </p>
    <p>Three main products drove about 90% of revenue: the 27-inch gaming monitor ($9.8 million), the MacBook Air ($7.7 million), and Apple AirPods ($7.7 million). ThinkPad laptops accounted for most of the rest. </p>
    <p>Apple's iPhone, Bose headphones, Samsung webcams, and charging cables contributed only about 10%. The Bose headphones had the lowest revenue at around $3,000 and even had no revenue in some months.</p>
    <p>Monitor revenue share increased from about 30% in 2020 to about 50% in December 2022. The proportion of MacBook Air revenue increased from about 15% to about 30% in 2020 before declining again, matching the fluctuations in AOV.</p>
    <p>  </p>
    <img width="919" height="580" alt="image" src="https://github.com/user-attachments/assets/2b8e59ac-57c4-49e1-9629-32771956b498" />
    <p>  </p>
    <p>AirPods ($160) and charging cables ($20) accounted for most orders, but revenue per order was very low. MacBook Airs and ThinkPads accounted for a small portion of orders but contributed significantly to revenue. Monitors combined both elements, accounting for approximately 20% of orders and being the largest revenue-generating product. Its order share increased to around 29% by the end of 2022. </p>
    <p>Samsung webcams, launched in 2020, increased to around 10% of orders in 2021-2022, while Apple's iPhones and Bose headphones had the lowest order and sales share in any year.</p>
</p>
    <img width="975" height="469" alt="image" src="https://github.com/user-attachments/assets/9675d46b-98b8-44d1-9171-2fee2873040c" />
    <p>   </p>
    <p>Headphones remain the largest contributor to sales but saw a slight decline in 2022. Their order share decreased from 46-49% (2019-2020) to 41-43% (2021-2022).</p>
    <p>Accessory order share increased from 21% to a peak of 35% in Q2 2022, then fell back to 27% by the end of 2022.</p>
    <p>Monitor share remained around 21-22% every year but surged to 26% by the end of 2022, the highest level for this period.</p>
    <p>Laptops accounted for a small fraction of total orders (4-9%), but with order values exceeding $1,000, they had a significant impact on revenue. This share doubled in 2020 (to 8-9%) and then fell back to around 5%, returning to 2019 levels.</p>
  </div>
  
  <div class='Region'>
    <h2>Region</h2>
    <img width="919" height="497" alt="image" src="https://github.com/user-attachments/assets/e770af63-b96b-4737-86cd-5f104d19f71a" />
    <p>  </p>
    <p>The COVID cycle was global. Every region roughly increased in 2020 and fell in 2022, so it is a market-wide effect, not one region’s problem.</p>
    <p>The 2021 dip came mostly from NA. Total sales fell about $1 million, and NA accounted for about $0.8M of it, while other regions were nearly flat (-3 to -6%).</p>
    <img width="919" height="502" alt="image" src="https://github.com/user-attachments/assets/b081bf32-a628-4765-a979-38b961789038" />
    <p>  </p>
    <p>APAC is shifting toward monitor products. Its monitor share rose every year, from 20.8% to 24.66%, the highest of any region. </p>
    <p>NA drives the global shift toward accessories. NA accessories share rose from 21% (2020) to 33% (2022) of orders, while headphones fell from 48% to 41%.</p>
    <p>LATAM moved most toward cheap products. Accessories went from about 28% to 50% of orders while headphones fell from 42% to 30%, monitors from 20% to 16%, and laptops to about 3%. More low-price orders and fewer high-value ones happened in LATAM that led to the steepest drop in 2022 (-56%).</p>

    
  </div>
  
  <div class='Loyalty Program'>
    <h2>Loyalty Program</h2>
    <img width="975" height="459" alt="image" src="https://github.com/user-attachments/assets/c2b9f119-8cad-4b50-a900-831eaf1430ba" />
    <p>  </p>
    <p>Loyalty members kept growing after the pandemic boom. Their sales rose from $0.43M (2019) to $2.72M (2022) about $2.3M, and AOV grew 18% ($207 to $245), while non-loyalty sales fell from $3.45M in 2019 to $2.24M in 2022, and AOV declined 8% ($233 to $214). </p>
    <p>In 2022, loyalty members spent about $31 more per order than non-loyalty customers ($245 vs $214). Loyalty AOV stayed nearly flat from 2021 (−1.6%), while non-loyalty AOV fell about 18%.</p>
    <img width="919" height="536" alt="image" src="https://github.com/user-attachments/assets/33e6fc1c-70ed-4837-8dad-83203ec07c21" />
    <p></p>
    <p>Members are mostly headphone buyers. More than half of orders from members were headphones every year (59% in 2019 and 54% in 2022). Loyalty customers are shifting toward monitors (270 orders in 2019 to 2k orders in 2022) that explains why loyalty AOV kept rising. They rarely bought laptops. Laptops are only 2-4% of their orders.</p>

  </div>

 <div class='Refund'>
    <h2>Refund</h2>
    <img width="919" height="553" alt="image" src="https://github.com/user-attachments/assets/23ba95a4-157d-449d-b2ee-464b4537ce66" />
    <p>   </p>
    <p>The refund rate increased from 5.7% to 9.2%, and the number of returned items more than tripled (from 965 to 3,120) in 2020.</p>
    <p> AirPods and monitors drove refund volume. AirPods had 1,529 refunds, and monitors had 820 refunds in 2020. However, laptops had the highest refund rates: MacBook Air (18.3% in 2019, 16.9% in 2020) and ThinkPad (17.1%, 17%).</p>
    <p>Accessories were rarely returned. Charging cables had low refund rates (2.36% in 2019 and 2.59% in 2020). Bose had a 0% rate, but due to the low sales volume, this number is not significant.</p>
    <p>All products recorded no refunds in 2022, which is almost certainly due to a lack of data or a change in the refund policy. Additionally, many refunds were recorded more than two years after delivery. Both of these need to be confirmed with the data engineering team before reporting refund KPIs.</p>
</p>
  </div>  
</div>

<div class='Recommendation'>
  <h1 align='center'>Recommendations</h1>

  <div class='Sales Trends'>
    <h2>Sales</h2>
    <p>Sales usually fell sharply in October, with a 55% decline in October 2022. Introduce October promotions, targeted discounts, or product bundles to maintain demand between September and the holiday season.</p>
    <p>November and December were consistently strong months during 2019-2022. Prepare inventory and marketing campaigns ahead of November and December to capture peak holiday demand.</p>

  </div>

  <div class='Product Performance'>
    <h2>Product</h2>
    <p>With three main products, gaming monitor, MacBook Air, and AirPods, maintain sufficient inventory, especially for the monitor, to capture order share gains toward the end of 2022.</p>
    <p>Bundle lower-priced accessories such as charging cables with laptops and monitors to increase basket value.</p>
    <p>Investigate the low sales of Bose Headphones and Apple iPhones before deciding whether to reduce inventory or discontinue products. </p>

  </div>

  <div class='Loyalty Program'>
    <h2>Loyalty Program</h2>
    <p>Expand loyalty benefits by promotions, reward points, and personalized product recommendations.</p>
    <p>Convert repeat non-loyalty customers into loyalty members through sign-up incentives at checkout.</p>

  </div>

  <div class='Region'>
    <h2>Region</h2>
    <p>All regions experienced a similar pandemic-related sales cycle, but LATAM had the biggest sales decline in 2022 at 56%. Prioritize LATAM for further investigation into the sales decline and the shift toward lower-priced products.</p>
    <p>Promote monitors in APAC, where monitor order share increased from 20.8% to 24.66%.</p>
    <p>In NA, use accessories with laptop or monitor bundles to increase revenue per order. </p>

  </div>

  <div class='Refund Rate'>
    <h2>Refund Rate</h2>
    <p>MacBook Air and ThinkPad laptops had the highest refund rate, so investigate the reasons for laptop returns (product defects, shipping damage, and mismatches between product descriptions and customer expectations). </p>
    <p>Work with the data engineering team to investigate missing 2022 refund records.</p>

  </div>
</div>


