# 📊 Shopify App Success – Power BI Project

## 🔗 Dataset
- `shopify.xlsx` – Contains data scraped from the Shopify App Store

## 📁 Project Structure
```
ShopifyAppSuccess/
├── Screenshot1.3.png
├── Screenshot_103.png
├── Screenshot_104.png
├── Screenshot_105.png
├── Screenshot_106.png
├── Screenshot_107.png
├── Screenshot_109.png
├── Screenshot_110.png
├── README.md
```

---

## 🧠 Project Overview
Analyze the landscape of apps on the Shopify platform using Power BI. Build multiple visualizations to answer key questions about app success, developer responsiveness, and review quality.

### Goal
Use Power BI visualizations to:
- Understand app trends
- Evaluate review behavior
- Explore developer responsiveness

Each question should be visualized in a **dedicated report page** in Power BI and a screenshot saved.

---

## 📌 Task Breakdown

### Part 1: App Landscape
- Sheet: `App Landscape`
1. **KPI Card** – Count of unique apps
2. **Line Chart** – Sum of review counts by `lastmod` date (use flat date, not hierarchy)
3. **Scatterplot** – `reviews_count` (X-axis) vs `average_rating` (Y-axis); add annotation with `Text Box`

---

### Part 2: Reviews
- Sheet: `Reviews`
1. **New Column**: `helpful_reviews = rating * (1 + helpful_count)`
   - Show average as a KPI Card
2. **New Column**: `developer_answered` (1 if `developer_reply` is not blank, else 0)
   - Scatterplot: `developer_answered` (X-axis) vs `rating` (Y-axis)

---

### Part 3: App Reviews
- Sheet: `App Reviews`
1. **Modeling**: Create relationship from `Reviews.app_id` → `Apps.id`
   - Bar chart: `developer` (X-axis) vs `sum(rating)` (Y-axis)
2. **Better Analysis**:
   - Bar chart: `developer` vs average `helpful_review`
3. **Responsiveness**:
   - Bar chart: `developer` vs `developer_answered`
   - Apply filter: only `reviews_count > 500`

---

## 🖼️ Screenshots
One screenshot for **each question** on each Power BI page (8 total). Ensure the full screen is visible with annotations where applicable.

---

## ✅ Notes
> `.pbix` files not shared — only screenshots are uploaded. Make sure `.pbix` is organized with one page per section.
