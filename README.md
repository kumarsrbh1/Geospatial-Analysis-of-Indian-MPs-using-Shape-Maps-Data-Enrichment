# 📊 India MP Dashboard (Geospatial + Data Augmentation)

🚀 End-to-end data project combining web scraping, data augmentation, and geospatial visualization using Power BI.

---

## 🎯 Project Overview

This project extracts and augments data of Members of Parliament (MPs) from PRS India and builds a **geospatial dashboard using Shape Maps** to analyze state-wise distribution.

---

## 🔥 Key Highlights

- ✅ Web scraping using Python
- ✅ DOM inspection & CSS selector usage
- ✅ Data augmentation with MP profile images
- ✅ Handling real-world data inconsistencies
- ✅ Geospatial analysis using Power BI Shape Maps

---

## 📂 Dataset

- Source: PRS India (https://prsindia.org/mptrack/18th-lok-sabha)
- Raw file: `18 LS MP Track.csv`
- Processed file: `MPwithImageLink.csv`

---

## ⚙️ Workflow

### 1. Data Augmentation
- Clean MP names into URL slugs
- Handle inconsistencies using manual mapping
- Extract profile images via web scraping

### 2. Web Scraping
- Fetch MP profile pages using `requests`
- Parse HTML using BeautifulSoup
- Extract images using CSS selectors:

### 3. Data Processing
- Convert relative image paths to full URLs
- Store results in `imageLink` column

### 4. Geospatial Visualization
- Use Power BI Shape Maps to analyze:
- MP distribution across states
- Region-wise insights

---

## 🗺️ Geospatial Analysis (Shape Map)

### 🎯 Objective
Visualize parliamentary representation across Indian states.

### ⚙️ Approach
- Location field: `state`
- Metric: MP count per state
- Visual: Power BI Shape Map

### 💡 Insights
- Identify states with higher MP representation
- Compare regional distributions
- Enable state-level filtering

---

## ⚠️ Challenges

- PRS URLs are not standardized
- Name mismatches (spelling, prefixes, missing words)
- Required manual corrections for ~10% of cases

---

## 💡 Solution Approach

Implemented a hybrid strategy:

- ✅ Automated name cleaning
- ✅ Manual mapping for mismatched names

---

## 🚀 Output

- Enriched dataset with image links ✅
- Power BI dashboard (Shape Map) ✅
