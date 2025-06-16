# 📱 Google Play Store Data Analysis – Internship Project (NullClass)

This project was completed as part of a data analytics internship program offered by **NullClass**. The objective was to extract insights, visualize patterns, and simulate production-level dashboard logic using Google Play Store data.

---

## 🎯 Project Objective

To explore and analyze user reviews, app ratings, category performance, and install trends on the Google Play Store using Python tools like Pandas, NumPy, and Plotly. The project focused on:

- Sentiment analysis of app reviews  
- Category-based comparisons  
- Data filtering based on real-world rules  
- Visualization dashboards with time-based logic  

---

## ✅ Tasks Covered

### Task 1 – Sentiment Distribution Analysis

**Goal:**  
Visualize the distribution of user sentiments (`Positive`, `Neutral`, `Negative`) for apps based on different rating groups.

**What was done:**
- Filtered apps with more than 1,000 reviews  
- Created custom rating buckets (1–2 stars, 3–4 stars, 4–5 stars)  
- Selected top 5 app categories  
- Grouped the data by category, sentiment, and rating group  
- Visualized it using a stacked bar chart (Plotly)  
- Ensured clean data with null handling and type conversion

---

### Task 2 – Rating vs Reviews by Category

**Goal:**  
Compare the **average rating** and **total review count** for the top 10 app categories by number of installs.

**What was done:**
- Filtered dataset to exclude:
  - Categories with average rating below 4.0  
  - Apps with size below 10MB  
  - Apps not updated in January  
- Selected top 10 categories by install count  
- Visualized data using a grouped bar chart  
- Implemented time restriction: chart only shows between **3 PM to 5 PM IST**

---

### Task 3 – Bubble Chart Analysis: Size vs Rating

**Goal:**  
Show the relationship between app size and rating, using bubble size for number of installs.

**What was done:**
- Applied multiple filters:
  - Rating > 3.5  
  - Reviews > 500  
  - Installs > 50,000  
  - Excluded app names containing letter **"S"**  
  - Sentiment subjectivity > 0.5  
  - Included only selected categories (Game, Beauty, Business, etc.)
- Enhanced with:
  - Translations: Beauty (Hindi), Business (Tamil), Dating (German)  
  - Highlighted the Game category in **pink**  
  - Chart shown only between **5 PM to 7 PM IST**

---

## 📚 Concepts & Techniques Used

- **Data Cleaning:**  
  Handling missing values, converting types (`Reviews`, `Size`, `Installs`)

- **Categorization:**  
  Created custom rating groups using `pd.cut()`

- **Group Aggregations:**  
  Used `.groupby()` to summarize and compare metrics

- **Sentiment Simulation:**  
  For learning purposes, generated random sentiments when missing

- **Date and Time Filtering:**  
  Used Python’s `datetime` and `pytz` to restrict chart visibility based on IST hours

- **Visualization with Plotly:**  
  Created stacked bar charts, grouped bar charts, and bubble charts

- **Language Translations:**  
  Translated category names into regional languages directly on charts

---

## 🛠 Libraries Used

| Library     | Purpose                          |
|-------------|----------------------------------|
| `pandas`    | Data loading, cleaning, analysis |
| `numpy`     | Numeric operations               |
| `plotly`    | Interactive visualizations       |
| `random`    | Simulated sentiment values       |
| `datetime`  | Time-based logic for chart access|
| `pytz`      | Timezone handling (IST)          |

---

## 📌 What I Learned

- Real-world data is messy: I practiced cleaning it manually
- Grouping and filtering can extract powerful insights
- Time-based logic adds realism to dashboards
- Creating region-specific features (translations, highlights) improves user experience
- Clear storytelling with visuals is crucial for impactful analysis

---

## 🎓 Internship Outcome

This project was part of the final submission for the NullClass Internship.  
The dashboard and charts created can be integrated into any Python or Streamlit-based reporting system.  
Each task demonstrated professional skills in:

- Data manipulation  
- Insight extraction  
- Visualization logic  
- Real-world readiness (time logic, translations, filtering)

---

## 🙋‍♂️ About Me

**Sumit Agnihotri**  
Data Science Student | Python & Visualization Enthusiast  
[GitHub](https://github.com/Sumit-Agnihotri) | [LinkedIn](https://linkedin.com/sumit-agnihotri)

---

> 📈 *Built for growth. Designed to impress. Ready for real-world challenges.*

## 📊 Technologies Used

| Tool    | Purpose                     |
|---------|-----------------------------|
| Python  | Core programming            |
| Pandas  | Data handling               |
| NumPy   | Numeric operations          |
| Plotly  | Interactive visualizations  |
| datetime / pytz | Time filtering logic |

---
