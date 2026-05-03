## Site Selection for Startup Investment Firm in Michigan

---

## 📌 Overview
This project analyzes financial, demographic, geographic, and construction data to identify optimal locations for establishing a startup investment firm in Michigan.  

Data sources include:
- Financial Industry Regulatory Authority (FINRA) study (2015)
- U.S. Census Bureau datasets
- U.S. Geological Survey (USGS) data
- State of Michigan open GIS data
- Building Advisor construction guidance

The analysis identifies **Oakland County** as the primary location and **Livingston County** as a secondary alternative.

---

## 📊 Investment Behavior & Demographics

Key findings from the FINRA study:
- Households earning **$50,000+**
- Individuals with **college education**
- Education attained **after marriage**

These factors significantly increase the likelihood of owning taxable investment accounts.

### Data Analysis
Census data were joined to vector datasets representing:
- Income
- Education
- Marriage rates
- Population

### Key Insights
- Highest % of $50K+ households: **Oakland & Livingston Counties**
- Both counties rank in the **3rd highest quartile for education**
- **Oakland County** is the wealthiest county in Michigan
- Marriage rates: Moderate in both counties

---

## 👥 Population Analysis

- **Wayne County** has the largest population
- **Oakland County** ranks second
- Population differences help explain:
  - Higher income concentration in Oakland vs. Livingston

---

## 🏙️ Site Selection Decision

### Primary Location:
**Oakland County**
- Higher income concentration
- Strong education levels
- Larger population base

### Secondary Location:
**Livingston County**
- Strong income levels (2nd highest)
- Viable alternative option

---

## 🗺️ Site Selection Methodology

### Data Layers Used:
- Slope (USGS DEM – 10m resolution)
- Land Cover (2011)
- Road Networks (Michigan GIS data)

### Slope Criteria
- Suitable: **< 10% slope**
- Reason: Lower construction cost

> “Flat sites or gentle grades of less than about 10% are easiest to build on.”  
> — BuildingAdvisor (2016)

---

### Land Cover Criteria
Selected:
- Barren land
- Developed open space

---

### Road Accessibility
Buffers created:
- **500m** → Primary roads  
- **25m** → Secondary roads  

Converted to raster for analysis.

---

### Output
- Combined raster analysis
- Classified:
  - Suitable areas
  - Non-suitable areas

---

## ⚠️ Data Limitation & Workaround

### Issue:
Parcel-level data unavailable for both counties

### Solution:
Three-step process:
1. Select polygons between **3,000–20,000 sq ft**
2. Convert polygons → point features
3. Generate **point density (per square mile)**

### Benefit:
- Reduced map clutter
- Improved visualization clarity

---

## 📍 Site Selection Results

| County        | Candidate Areas |
|--------------|----------------|
| Oakland      | 9              |
| Livingston   | 5              |
| **Total**    | **14**         |

### Interpretation:
- Oakland has more sites due to:
  - Higher development
- Livingston is more rural

---

## ✅ Final Recommendation

**Preferred Location:**  
➡️ Oakland County  

**Alternative Location:**  
➡️ Livingston County  

Rationale:
- Strong demographics for investment behavior
- Higher income concentrations
- Greater site availability (Oakland)

---

## 📚 Works Cited

- FINRA Investor Education Foundation (2015)  
- U.S. Census Bureau – American Community Survey  
- U.S. Geological Survey (USGS) – National Elevation Dataset  
- National Land Cover Database (2011)  
- Michigan GIS Open Data Portal  
- BuildingAdvisor (2016)  
- ESRI Basemaps (World Imagery & National Geographic)

---

## 🧭 Tools & Technologies

- GIS Analysis (ArcGIS / QGIS)
- Raster & Vector Processing
- Spatial Buffering
- Point Density Analysis

---

## 📈 Outputs

- Thematic Maps (Map 1–9)
- Suitability Analysis Layers
- Site Selection Visualizations

---
