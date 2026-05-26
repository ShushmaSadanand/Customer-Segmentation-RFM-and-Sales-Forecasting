# Advanced Customer Segmentation (RFM + K-Means), LDA Validation, & Sales Forecasting

Welcome to the Advanced Customer Intelligence division of my portfolio. This repository contains a production-grade behavioral analytics engine designed to parse commercial retail datasets (such as the US Superstore framework), engineer dynamic customer profiles, statistically validate behavioral clusters, and project long-term sales velocities.

---

## Project Architecture & Analytical Framework
**File:** `Causal_Marketing_GrpProject.pdf` (Comprehensive Analytics & Forecast Report)

Modern corporate growth relies on shifting away from uniform mass-marketing toward hyper-targeted operational strategies. This project acts as an end-to-end data pipeline that transforms transactional log files into mathematical behavior maps, enabling optimized marketing spend and precise inventory management.

### Advanced Analytics & Modeling Framework

#### 1. RFM Feature Extraction & Unsupervised Clustering
* **Behavioral Vectorization:** Extracted transaction histories across **793 unique customers** to engineer three foundation dimensions: **Recency ($R$)**, **Frequency ($F$)**, and **Monetary Value ($M$)**.
* **Algorithmic Segmentation:** Built a **K-Means Clustering** pipeline to group customers into 4 distinct behavioral archetypes:
  * **Cluster 0 (Champions):** High-frequency, high-spending consumers with low recency.
  * **Cluster 1 (Potential Loyalists):** Moderate transaction depth with consistent visit velocities.
  * **Cluster 2 (Loyal High-Spenders):** Outlier-level spending profiles driving disproportionate margin value.
  * **Cluster 3 (At-Risk / Dormant):** Extended latency periods with deteriorating visit patterns.

#### 2. Multi-Class Validation via Linear Discriminant Analysis (LDA)
* **Statistical Verification:** Rather than trusting K-Means implicitly, I implemented a **Linear Discriminant Analysis (LDA)** classifier to test if these customer segments represent genuine behavioral archetypes rather than mathematical clustering artifacts.
* **Dimensional Projective Mapping:** Modeled the boundaries using 5 behavioral attributes (Recency, Frequency, Monetary Value, Total Profit, and Average Discount Rate). Projecting onto the discriminant coordinate axes ($LD_1$ and $LD_2$) confirmed clear spatial separation, with the *Loyal High-Spenders* completely isolated and *At-Risk* profiles pulled heavily along the negative discriminant trajectory.

#### 3. Customer Lifetime Value (CLV) & Sales Projections
* **Value Modeling:** Modeled transaction retention rates and average order values to project individual Customer Lifetime Value vectors over extended horizons.
* **Predictive Sales Forecasting:** Built mathematical trends and category-specific forecasting models to project future retail category growth, protecting supply chains against inventory stockouts or margin-draining overstocking.

---

## Key Technical Competencies
* **Advanced Segmentation Systems:** RFM Matrix Construction, Feature Scale Standardization
* **Unsupervised Learning & Matrix Partitioning:** K-Means Clustering, Distance Metrics
* **Supervised Classification & Dimensional Validation:** Linear Discriminant Analysis (LDA)
* **Financial Predictive Operations:** Customer Lifetime Value ($CLV$) Engineering, Time-Series / Trend Forecasting
* **Core Toolkit:** Python Analytics Stack (Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn)
