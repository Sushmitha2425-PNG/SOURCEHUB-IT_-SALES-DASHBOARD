🎓 Student Performance Dashboard — Power BI Project"A" Task 2

## 📌 Project Overview
The **Student Performance Dashboard** visualizes and analyzes student performance across departments and demographics.  
It tracks **total scores**, **attendance**, **pass/fail ratios**, and **top performers** to help educators identify trends, correlations, and areas for improvement.

---

## 🧩 Data Preparation Process

### 1. Data Cleaning
- Imported dataset with columns:  
  `Student_ID, First_Name, Gender, Department, Attendance (%), Midterm_Score, Final_Score, Assignments_Avg, Quizzes_Avg, Participation_Score, Projects_Score, Total_Score, Grade`
- Removed duplicates and blanks from `Student_ID`.
- Converted numeric fields (`Total_Score`, `Attendance (%)`) to **decimal number** type.
- Verified that there were no missing or invalid entries.

### 2. Calculated Columns & Measures

#### ✅ Pass/Fail Classification
```DAX
PassFail = 
IF(VALUE([Total_Score]) >= 400, "Pass", "Fail")
````

> Used to classify students based on performance threshold of 400.

#### ✅ Ranking Students

```DAX
Rank_Students = 
RANKX(
    ALL('Table1'[Student_ID]), 
    CALCULATE(SUM('Table1'[Total_Score])),
    ,
    DESC,
    Dense
)
```

> Used to rank students based on total score in descending order.

#### ✅ Average Measures

* **Average of Total_Score**
* **Average of Attendance (%)**

---

## 📊 Dashboard Components

### 🟣 1. Title: *Student Performance Dashboard*

A clear title defining the report’s purpose.

---

### 🟣 2. Student Distribution by Total Score

**Visual Type:** Area/Column Chart
**Axis:** `Total_Score`
**Values:** `Count of Student_ID`

**Purpose:** Displays the score distribution pattern across all students.
**Tooltip Suggestion:**

* Total_Score
* Count of Students
* % of total students

**Insight:** Most students scored between **350–450**, indicating moderate performance spread.

---

### 🟣 3. KPIs — Average Total Score & Attendance (%)

**Visual Type:** Card
**Measures Used:**

* `Average of Total_Score` → 414.62
* `Average of Attendance (%)` → 75.36

**Insight:** Students have an **average total score** of 415/600 and an **average attendance** of 75%, reflecting overall strong engagement.

---

### 🟣 4. Pass/Fail Ratio

**Visual Type:** Bar Chart
**Axis:** `PassFail`
**Value:** Count of Student_ID

**Purpose:** Visualize how many students passed or failed.
**Insight:** A majority of students **passed**, indicating good academic outcomes.

---

### 🟣 5. Attendance vs Total Score

**Visual Type:** Scatter Plot
**Axis:**

* X: Average of Attendance (%)
* Y: Average of Total_Score

**Purpose:** To explore the correlation between attendance and performance.
**Insight:** There is a **positive relationship** — higher attendance corresponds to higher scores.

---

### 🟣 6. Top Performers

**Visual Type:** Horizontal Bar Chart
**Axis:**

* Y: First_Name
* X: Sum of Total_Score
  **Measure:** `Rank_Students`

**Purpose:** Highlight top-ranked students by total score.
**Insight:** **Maria**, **Ahmed**, and **Ali** are the highest scorers, showcasing consistent performance.

---

### 🟣 7. Slicers — Gender & Department

**Fields:** `Gender`, `Department`
**Purpose:** Enable interactivity for filtering insights by demographics.

**Tooltip Suggestion:** “Click to filter by gender or department.”

---

## 🧠 Tooltips Added

| Visual               | Tooltip Details                            |
| -------------------- | ------------------------------------------ |
| Student Distribution | Total Score, Student Count, % of Total     |
| KPI Cards            | Average vs Previous Period (if applicable) |
| Pass/Fail Ratio      | % of total students                        |
| Attendance vs Score  | Student Name, Total Score, Attendance      |
| Top Performers       | Rank, Total Score, Department              |

---

## 📈 Key Insights

1. **Average Performance:** Overall average score of ~415/600 with 75% attendance indicates good engagement and learning outcomes.
2. **Pass Rate:** Most students score above 400 — a strong overall pass rate.
3. **Correlation:** Higher attendance leads to better performance.
4. **Top Performers:** A few students (Maria, Ahmed, Ali) stand out as consistent high achievers.
5. **Score Distribution:** Most students fall within a mid-score range (350–450).

---

## 🖼️ Dashboard Preview

*("C:\Users\Sushmitha D Shetty\Pictures\Screenshots\Screenshot 2025-10-14 211619.png")*


---

## 🧾 Summary

This Power BI dashboard efficiently showcases how attendance, performance, and departmental variations affect overall student outcomes.
It demonstrates the power of DAX measures, interactivity through slicers, and insightful data visualization.

---

**Created and Analyzed by:** *Sushmitha D*
📅 *October 2025*
🧠 *Tools Used: Power BI, DAX, Excel (for preprocessing)*


