# 📱 GPlay Store Analysis – Full Project

A professional-level Data Analysis & Visualization project using **Python**, **Pandas**, **NumPy**, and **Plotly**  
> Built as part of the **NullClass Placement Program**

---

## 📌 Project Overview

This project analyzes and visualizes Google Play Store app data, focusing on sentiment distribution, ratings, reviews, installs, and category-level patterns.  
It includes **three main tasks** with applied business logic, data filtering, and real-world dashboard constraints.

---

## 📂 Tasks Breakdown

---

### ✅ Task 1 – Sentiment Distribution (Stacked Bar Chart)

**Objective:**  
Visualize the sentiment distribution (Positive, Neutral, Negative) of user reviews segmented by rating groups and limited to top 5 app categories.

**Chart:**  
- Stacked bar chart
- X-axis: Category  
- Y-axis: Review Count  
- Color: Sentiment  
- Split into 3 charts for rating groups: 1–2 ⭐, 3–4 ⭐, 4–5 ⭐

**Filters Applied:**  
- Reviews > 1000  
- Top 5 categories  
- Rating grouped via `pd.cut()`  
- Sentiment column already present

---

### ✅ Task 2 – Avg Rating & Total Reviews by Installs (Grouped Bar Chart)

**Objective:**  
Compare average rating and total review count for the top 10 app categories based on number of installs.

**Chart:**  
- Grouped bar chart  
- Bars show average rating and total reviews side-by-side for each category

**Filters Applied:**  
- Exclude categories where:
  - Average rating < 4.0  
  - App size < 10 MB  
  - Last update not in January  
- Visible only between **3 PM to 5 PM IST**  
- Uses `datetime` and `pytz` to control time-based rendering

---

### ✅ Task 3 – Size vs Rating (Bubble Chart)

**Objective:**  
Analyze the relationship between app size and average rating using a bubble chart where bubble size represents number of installs.

**Chart:**  
- X-axis: App Size (MB)  
- Y-axis: Average Rating  
- Bubble Size: Installs  
- Bubble Color: Category  

**Filters Applied:**  
- Rating > 3.5  
- Categories: Game, Beauty, Business, Comics, Communication, Dating, Entertainment, Social, Event  
- Reviews > 500  
- App name must **not contain letter 'S'**  
- Sentiment subjectivity > 0.5  
- Installs > 50K  
- Visible only between **5 PM to 7 PM IST**

**Special Features:**  
- Game category bubbles are **highlighted in pink**  
- Category labels translated:
  - Beauty → Hindi  
  - Business → Tamil  
  - Dating → German

---

## 🚀 Features

- ✅ Clean, filtered visualizations using Pandas + Plotly  
- ✅ Time-restricted charts using `datetime` and `pytz`  
- ✅ Real-world dashboard behavior (hides charts outside allowed hours)  
- ✅ Custom visual tweaks & multi-language category display  
- ✅ Ready to integrate into Streamlit or HTML dashboards

---

## 📊 Technologies Used

| Tool    | Purpose                     |
|---------|-----------------------------|
| Python  | Core programming            |
| Pandas  | Data handling               |
| NumPy   | Numeric operations          |
| Plotly  | Interactive visualizations  |
| datetime / pytz | Time filtering logic |

---