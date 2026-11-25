# AeroFit Treadmill Customer Profiling & Descriptive Statistical Analysis

## Problem Statement
Examine **180 customer purchase records** across 9 demographic, socioeconomic, and fitness attributes to establish distinct buyer profiles for AeroFit’s three treadmill models (**KP281** entry-level, **KP481** mid-tier, and **KP781** commercial flagship) and identify key drivers of product selection[cite: 242, 243].

## Technical Stack & Libraries
* **Data Wrangling & Statistical Summaries:** `Pandas`, `NumPy` (five-number summaries, skewness coefficients, interquartile range analysis, feature binning)[cite: 243, 245, 250]
* **Diagnostic & Multivariate Visualization:** `Matplotlib`, `Seaborn` (Histogram + KDE plots with Mean/Median annotations, segmented Boxplots, Pearson Correlation Heatmaps, and Hue-Segmented Pairplots)[cite: 250, 252, 253, 256, 257]

## Key Empirical Findings
1. **Product Market Share:** **KP281** accounts for **44.44%** ($n=80$) of sales, **KP481** for **33.33%** ($n=60$), and **KP781** for **22.22%** ($n=40$)[cite: 245, 248].
2. **The "Athletic Triad" & Flagship Separation:** Strong positive correlations link **Fitness & Miles** ($r = 0.79$), **Usage & Miles** ($r = 0.76$), and **Usage & Fitness** ($r = 0.67$)[cite: 258, 264]. Flagship **KP781** buyers separate sharply on income (median **$76,569** vs. $46,617–$49,460 for KP281/KP481), weekly mileage (median **160 miles** vs. 85 miles), and workout frequency (median **5 days/week** vs. 3 days/week)[cite: 255, 265, 266].
3. **KP281 vs. KP481 Feature Overlap:** Entry-level and mid-tier buyers share nearly identical demographic, income, and workout distributions, indicating weak product differentiation[cite: 255, 258, 264].
4. **Gender Disparity in Flagship Tier:** Male shoppers account for **82.5%** of KP781 purchases, highlighting an under-penetrated market among serious female runners[cite: 266, 267].
5. **Demographic Neutrality:** Age ($r = 0.02$ to $0.06$ with workout metrics) and Marital Status show no meaningful effect on treadmill tier selection[cite: 255, 258, 264].

## Strategic Recommendations
* **Differentiate KP281 & KP481:** Deploy side-by-side specification comparisons and bundle KP481 with heart-rate monitors or extended warranties[cite: 267].
* **Targeted Outreach to Female Endurance Athletes:** Partner with women's running clubs and feature female marathoners in KP781 campaigns[cite: 267].
* **Interactive 3-Question Product Finder & EMI Financing:** Guide visitors by workout goal/frequency/budget and offer 0% monthly installments on the volume-leading KP281[cite: 267, 268].
