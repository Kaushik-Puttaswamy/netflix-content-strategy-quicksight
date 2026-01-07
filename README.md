# 🎬 Netflix Content Strategy Analysis using Amazon QuickSight

## 📌 Project Overview
This project analyzes Netflix’s global content catalog to uncover **trends across regions, genres, and time** using **Amazon QuickSight**.

The dashboard is designed for **executive decision-making**, combining:
- Governed KPIs  
- AI-assisted analytics using **QuickSight Q**  
- A **Netflix-inspired dark theme** for high-contrast, professional storytelling  

---

## 🎯 Business Objectives
- Understand **content mix evolution** (Movies vs TV Shows)
- Identify **regional production patterns**
- Analyze **genre dominance and ratings distribution**
- Track **content growth trends over time**
- Demonstrate **enterprise BI best practices** using AWS

---

## 📊 Dataset
- **Source:** Kaggle – Netflix Movies and TV Shows  
- **Link:** https://www.kaggle.com/datasets/shivamb/netflix-shows/data  
- **Records:** 8,807 titles  

### Key Fields
- `type`
- `country`
- `release_year`
- `rating`
- `duration`
- `listed_in`

---

## 🧠 Analytics & BI Stack
- **Amazon QuickSight**
  - SPICE in-memory engine
  - Dataset-level calculated fields (governance)
  - QuickSight Q (AI / natural language queries)
- **Amazon S3**
  - Dataset storage
- **Netflix-inspired Dark Theme**
  - High contrast
  - Accessibility-friendly
  - Executive presentation ready

---

## 📌 Key Performance Indicators (KPIs)

| KPI | Description |
|----|------------|
| Total Titles | Total content available |
| Total Movie Titles | Count of movies |
| Total TV Show Titles | Count of TV shows |
| Distinct Countries | Number of production regions |
| Average Release Year | Recency of catalog |

---

## 📈 Dashboard Pages

### 1️⃣ Executive Overview
High-level insights for leadership:
- KPI summary
- Movies vs TV Shows over time
- Genre distribution
- Ratings breakdown
- Country vs Titles

📄 **Export:** `dashboards/Executive_Overview.pdf`

---

### 2️⃣ Deep Dive Analysis
Analyst-level exploration:
- Release Year vs Type (stacked)
- Titles added by date
- Top genres post-2015
- Detailed breakdown tables

📄 **Export:** `dashboards/Deep_Dive_Analysis.pdf`

---

## 🧮 Calculated Fields (Examples)

```text
-- Total Movies
ifelse(type = 'Movie', 1, null)

-- Total TV Shows
ifelse(type = 'TV Show', 1, null)