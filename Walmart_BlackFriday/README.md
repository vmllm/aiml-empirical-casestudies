# Black Friday Customer Spend Analysis & Central Limit Theorem (CLT) Inference

## Problem Statement
Analyse **550,068 Black Friday retail transactions** across 10 demographic and merchandise attributes to evaluate whether female shoppers spend more per transaction than male shoppers, and extrapolate sample findings to a broader population of **50 million male and 50 million female customers** using the **Central Limit Theorem (CLT)** and **Confidence Intervals**[cite: 269].

## Technical Stack & Libraries
* **Data Manipulation & Memory Optimization:** `Pandas` (categorical type casting across 7 discrete features), `NumPy`[cite: 269, 270]
* **Statistical Inference:** `SciPy` (`scipy.stats.norm`), bootstrap sampling simulations ($n = 50, 200, 1000$ across 1,000 iterations), Tukey's $1.5 \times \text{IQR}$ & $3\sigma$ outlier checks[cite: 278, 279, 288, 289]
* **Data Visualization:** `Matplotlib`, `Seaborn` (KDE/Histograms, Boxplots, Correlation Heatmaps, Pairplots, Error-Bar Confidence Interval plots)[cite: 273, 274, 275, 276, 290]

## Key Empirical Findings
1. **Gender Spend Verdict:** Men spend **$702.96 more per transaction** on average than women (**$9,437.53** vs. **$8,734.57**; medians: **$8,098.00** vs. **$7,914.00**) and generate **76.72%** of total Black Friday revenue ($3.91B vs. $1.19B), driven by higher purchasing in big-ticket **Product Category 1** (27.89% of male purchases vs. 18.28% of female purchases)[cite: 287].
2. **Non-Overlapping Population Confidence Intervals:** At the 95% confidence level, true population mean spend is **$[$8,709.21, $8,759.92]** ($SE = \$12.94$) for female shoppers and **$[$9,422.02, $9,453.03]** ($SE = \$7.91$) for male shoppers—separated by a **$662.10** gap with zero overlap even at 99% confidence[cite: 288, 290, 291].
3. **Marital Status Neutrality:** Unmarried ($9,265.91) and married ($9,261.17) shoppers exhibit virtually identical spending with >85% overlap across 90%–99% confidence intervals[cite: 294, 295].
4. **Geographic & Life-Stage Drivers:** **City Category C** commands the highest average basket size (**$9,719.92**, median **$8,585.00**), while spending climbs monotonically across life stages from **$8,933.46** (ages 0–17) to **$9,463.66** (ages 51+)[cite: 282, 296, 298].
5. **Data Hygiene:** 0 missing values; 2,677 high-ticket transactions (> $21,400.50 upper Tukey fence; 0.487%) retained as valid luxury/electronics purchases[cite: 278, 279, 280].

## Strategic Recommendations
* **Lift Female Basket Size:** Introduce multi-item bundles and cart-threshold rewards in high-turnover Categories 5 and 8 where female purchases cluster[cite: 287, 291, 292, 303].
* **Upsell High-Ticket SKUs:** Feature Category 1 electronics, gaming gear, and extended warranties to male and 51+ shoppers[cite: 291, 303, 304].
* **Reallocate Inventory & Ad Spend:** Prioritize premium SKU allocation in **City Category C**, maintain high-volume stock in **City B** (42.03% of transactions), and discontinue marital-status ad segmentation[cite: 283, 303].
