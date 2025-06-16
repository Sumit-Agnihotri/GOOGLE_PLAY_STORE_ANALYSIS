# 📱 GPlay Store Project – Task 1

**Sentiment Analysis & Visualization of Google Play Store App Reviews**  
> A Data Analysis & Visualization Project using Pandas, NumPy, and Plotly

---

## 🧠 Objective

To visualize the **sentiment distribution (Positive, Neutral, Negative)** of user reviews on Google Play Store apps using a **stacked bar chart**, segmented by **rating groups** and limited to the **top 5 app categories**. Only apps with more than **1,000 reviews** were included.

---

## 📂 Dataset Overview

The dataset contains:
- App names, categories, ratings, reviews count
- Translated user reviews
- Sentiment labels: `Positive`, `Neutral`, `Negative`

---

## ✅ Key Steps

1. **Data Cleaning**
   - Removed missing values (`Rating`, `Reviews`, etc.)
   - Converted `Reviews` to numeric

2. **Filtering**
   - Included only apps with more than `1000` reviews
   - Selected top 5 most frequent categories

3. **Rating Group Buckets**
   - 1–2 Stars
   - 3–4 Stars
   - 4–5 Stars

4. **Grouping**
   - Grouped by `Category`, `Rating Group`, and `Sentiment`

5. **Visualization**
   - Created a **stacked bar chart** using Plotly
   - Faceted by `Rating Group` for comparison

---

## 📊 Output Chart

The final chart is an **interactive stacked bar chart**:
- X-axis: App categories  
- Y-axis: Number of reviews  
- Colors: Sentiment (green, orange, red)  
- Facet columns: Rating groups (1–2, 3–4, 4–5 Stars)

---

## 🔁 Enhancements

- ✅ Pie chart of overall sentiment distribution
- 🔜 Word Cloud (to be added)
- 🔜 Streamlit dashboard version

---

## 💡 Insights

- 📉 Most negative reviews came from apps with low (1–2 star) ratings in the Games category.
- 📈 Productivity and Tools apps with high ratings (4–5 stars) had mostly positive reviews.
- 🟠 Neutral sentiment is consistent across all categories and rating ranges.

---

## 🛠 Tech Stack

| Tool      | Purpose                   |
|-----------|---------------------------|
| Python    | Programming language      |
| Pandas    | Data manipulation         |
| NumPy     | Numerical operations      |
| Plotly    | Interactive visualization |

---

## 🚀 How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/yourusername/gplay-store-task1.git
   cd gplay-store-task1
