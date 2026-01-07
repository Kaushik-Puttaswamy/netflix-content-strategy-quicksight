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
```
## 🎨 Design Principles
- Netflix dark theme (charcoal background with red accents)
- Red used **only for emphasis**, not decoration
- White values for high contrast and readability
- Gray labels for contextual information
- Free-form **1600px layout** for pixel-perfect alignment

---

## 🔗 Live Dashboard

**Amazon QuickSight Dashboard:**  
https://ap-south-1.quicksight.aws.amazon.com/sn/account/kaush-quicksight-project/dashboards/e6b938a8-e200-4889-83eb-fc150bf09594/views/7c5046bd-0bf7-4b9e-b729-54034e151a55

> ⚠️ Requires Amazon QuickSight access permissions

---

## 📌 Key Takeaways
- Netflix’s catalog has shifted strongly toward **TV Shows** in recent years
- **International content** is a major growth driver
- **TV-MA** dominates ratings, indicating an adult-focused content strategy
- Post-2015 content growth is significantly higher than earlier years

---

## 📄 License
This project is licensed under the **MIT License**.
