# 🎬 # Netflix Data Analysis & Power BI Dashboard

An interactive Power BI dashboard analyzing Netflix's content catalog — built with a Python-based cleaning pipeline and a custom Netflix-branded theme.

---

## 📌 Project Overview

This project explores Netflix's content library (movies and TV shows) to uncover trends in release patterns, content ratings, genres, and geographic distribution. Raw data was cleaned and prepped in Python (Jupyter Notebook), then modeled and visualized in Power BI with a custom dark, Netflix-styled theme for a polished, presentation-ready dashboard.

---

## 🛠️ Tech Stack

| Stage | Tool |
|---|---|
| Data Cleaning & Preprocessing | Python (Pandas, NumPy) in Jupyter Notebook |
| Data Modeling & Visualization | Power BI Desktop |
| Theming | Custom Netflix-branded JSON theme |

---

## 🧹 Data Cleaning (Python)

Before loading into Power BI, the raw Netflix dataset was cleaned and structured in a notebook, including steps such as:
- Handling missing/null values (e.g., director, cast, country)
- Standardizing date formats (`date_added`, `release_year`)
- Splitting multi-value fields (genres, countries, cast) where needed
- Removing duplicate records
- Creating derived fields used across the dashboard (e.g., content age, recent vs. older content flags)

The cleaned dataset was exported and loaded into Power BI as the `netflix_cleaned` table.

---

## 📊 Dashboard Pages

### 1. Netflix Overview
A high-level snapshot of the catalog:
- Total Netflix Titles, Total Movies, Total TV Shows (KPI cards)
- Netflix Content by Rating
- Netflix Content by Release Year (trend line)
- Type filter slicer for interactive exploration

### 2. Content Analysis
A deeper look at content characteristics:
- Average Content Age by Type
- Recent vs. Older Content (donut breakdown)
- Ratings by Content Type
- Movie Duration Distribution
- Top 10 Countries by Content
- Rating Distribution by Content Type (100% stacked)
- Recent vs. Older Content by Type

### 3. Netflix Insights
Genre and geography-focused insights:
- Top 10 Genres by Content Type
- Top 10 Countries by Content Type
- Movie vs. TV Show Release Trend (line chart)
- Movies vs. TV Shows (donut breakdown)
- Recent Netflix Titles / Recent Content % (KPI cards)

All three pages share synced slicers for content type and other filters, so selections carry across the report.

---

## 🎨 Design — Netflix Theme

The report uses a fully custom Power BI theme built to match Netflix's brand identity:
- **Background:** near-black (`#141414` / `#0D0D0D`) across pages and visuals
- **Primary accent:** Netflix red (`#E50914`) for KPI cards, borders, and highlights
- **Supporting palette:** gold, teal, sky-blue, and purple accents for clear category/legend separation across charts
- **Typography:** white/light-grey text (Segoe UI) tuned for contrast on dark backgrounds
- **Cards & slicers:** rounded corners, subtle shadows, and red accent borders for a modern, branded look

---

## 🚀 How to Use

1. Open `Netflix_Dashboard_NetflixTheme.pbix` in **Power BI Desktop**
2. Use the slicers on each page to filter by content type, country, genre, or year
3. Hover over visuals for detailed tooltips
4. Switch between the three report pages using the tabs at the bottom

---

## 📂 Project Structure

```text
Netflix-Data-Analysis/
│
├── data/
│   ├── netflix_titles.csv
│   └── netflix_cleaned.csv
│
├── notebooks/
│   └── Netflix_EDA.ipynb
│
├── powerbi/
│   └── Netflix_Dashboard.pbix
│
├── images/
│   ├── dashboard_page1.png
│   ├── dashboard_page2.png
│   └── dashboard_page3.png
│
└── README.md
```
---

## ✨ Key Highlights

- End-to-end workflow: raw data → Python cleaning → Power BI modeling → styled dashboard
- Custom brand-matched theme for a polished, LinkedIn-ready presentation
- Multi-page report with cross-page synced filtering
- Mix of KPI cards, trend lines, bar/column charts, and donut charts for varied storytelling

---

## 👤 Author
Semon Neupane

Built as a personal data analytics project to practice end-to-end BI workflow: data cleaning, modeling, DAX/visual design, and dashboard theming.
