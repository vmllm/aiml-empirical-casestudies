# Netflix Global Content Catalog: Exploratory Data Analysis & Strategic Pivot

## Problem Statement
Perform comprehensive exploratory data analysis on **8,807 Netflix titles** across 12 metadata attributes (spanning 1925–2021) to uncover content format shifts, regional localization patterns, release-timing dynamics, and catalog freshness strategies[cite: 211, 212, 219].

## Technical Stack & Libraries
* **Data Wrangling & Preprocessing:** `Pandas`, `NumPy` (comma-separated attribute unnesting via `.str.split()` and `.explode()`, datetime parsing, regex duration extraction, memory optimization via `category` casting)[cite: 205, 211, 212, 216]
* **Outlier & Statistical Diagnostics:** Tukey's Interquartile Range ($1.5 \times \text{IQR}$) rule on movie runtimes, missing-value profiling[cite: 218, 219]
* **Visualization:** `Matplotlib`, `Seaborn` (Stacked Bar Charts, Line Trajectories, Pie/Count Subplots, Categorical Boxplots)[cite: 205, 206, 207, 208, 209, 216, 217]

## Key Empirical Findings
1. **Strategic Shift Toward Episodic Television:** While Movies comprise **69.62%** (6,131) of the historical catalog vs. **30.38%** (2,676) TV Shows, TV Show share of new releases climbed from ~25% (2016–2017) to **53.2% in 2021** (315 TV Shows vs. 277 Movies) to reduce subscriber churn[cite: 207, 209, 211, 221].
2. **Regional Content Polarization:** The US leads total volume (3,690 titles)[cite: 206]. **India** is overwhelmingly Movie-centric (**92.0%** movies; 962 vs. 84 TV shows), whereas **Japan** (63% TV shows) and **South Korea** (74% TV shows) are TV/Anime-first markets[cite: 206, 222].
3. **Release Timing & Binge Clustering:** **35% of all TV Shows (932 titles)** are added on **Fridays** to capture weekend binge-watching, with seasonal peaks in **December** (266), **July** (262), and **September** (251)[cite: 208].
4. **Catalog Freshness & Runtime Outliers:** **54.95%** of titles are onboarded within $\le 1$ year of release (0-year median lag for TV Shows vs. 2-year average lag for Movies)[cite: 211, 222]. Movie runtimes average **99.58 minutes** (median: 98 min; IQR: 87–114 min), with 450 IQR outliers representing valid short specials (< 46.5 min) and epic international films (> 154.5 min)[cite: 207, 219, 220].

## Strategic Recommendations
* **Regionalized Content Capital Allocation:** Prioritize theatrical/direct-to-digital film acquisitions in India while funding episodic dramas and anime in Japan and South Korea[cite: 206, 223].
* **Address the Kids & Family Gap:** Expand PG/TV-Y/TV-PG programming (currently 20.87% vs. >60% TV-MA/TV-14) to reduce multi-user household churn[cite: 220, 222, 223].
* **Friday Holiday Tentpoles:** Anchor major series launches on Fridays in July and December while scheduling mid-tier titles on Wednesdays/Thursdays in low-volume months[cite: 208].
