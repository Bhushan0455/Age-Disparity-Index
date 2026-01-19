# Aadhaar Age Disparity Analysis

## 📌 Project Overview
This project analyzes **age-wise disparities in Aadhaar enrollment across Indian states** using a data-driven, dual-metric approach.  
Instead of relying on aggregate enrollment counts, the study evaluates **how effectively Aadhaar enrollment transitions across life stages**, from early childhood to adulthood.

The analysis is supported by an interactive **Power BI dashboard** and reproducible **Python-based data processing**.

---

## 🎯 Problem Statement
Aadhaar enrollment distribution varies significantly across age groups and states in India.  
High enrollment in early childhood does not necessarily ensure continued inclusion during school-age years or adulthood.

This project aims to:
- Identify age-based enrollment imbalances
- Detect transition gaps between key life stages
- Provide actionable insights for targeted policy intervention

---

## 📊 Dataset Description
- **Source:** UIDAI / Government open data
- **Granularity:** State-level
- **Age Groups:**
  - 0–5 years
  - 5–17 years
  - 18+ years

### Derived Fields:
- Percentage share of each age group
- Disparity metrics for cross-state comparison

---

## 🧮 Methodology

### 1️⃣ Data Processing
- Aggregated raw enrollment data at the state level
- Normalized enrollment counts into percentages to ensure fair comparison
- Cleaned and standardized state names for consistency

### 2️⃣ Key Metrics

#### 🔹 Child Transition Disparity (CTD)
CTD = % (Age 0–5) − % (Age 5–17)

- Measures transition effectiveness from early childhood to school-age
- **Lower values indicate better continuity**

#### 🔹 Adult Inclusion Gap (AIG)
AIG = % (Age 0–5) − % (Age 18+)

- Measures long-term inclusion into adulthood
- **Lower values indicate stronger adult Aadhaar coverage**

### Why Dual Metrics?
Using both metrics allows separation of:
- Short-term enrollment transition issues
- Long-term adult inclusion gaps

This avoids misleading conclusions from single-metric analysis.

---

## 📈 Visualization (Power BI)
The Power BI dashboard includes:
- **Filled Map:** Geographic distribution of Adult Inclusion Gap
- **Clustered Bar Charts:** State-wise CTD and AIG rankings
- **Stacked Bar Chart:** Age-wise enrollment composition
- **Interactive Slicers:** State-level filtering

---

## 🔍 Key Insights
- Strong early-child enrollment does not always translate into adult inclusion
- School-age transition (5–17 years) is a critical bottleneck in several states
- Regional enrollment patterns indicate the need for customized strategies
- Dual-metric analysis enables targeted, age-specific policy focus

---

## 🛠️ Tools & Technologies
- **Python** (Pandas, Jupyter Notebook)
- **Power BI** (Interactive dashboard & mapping)
- **Excel / CSV** (Intermediate data storage)
- **GitHub** (Version control & reproducibility)
