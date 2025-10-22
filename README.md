# Udemy Data Analysis Project

## Project Overview

* The **Udemy Data Analysis Project** aims to explore and analyze the Udemy courses dataset to gain insights into **subjects, pricing, popularity, and trends**.
* The project answers key business and analytical questions about courses, including which subjects perform best, pricing patterns, and audience engagement.
* It focuses on **data cleaning, exploration, and visualization** using Python.

🔗 View the Project

---

## Objective

* To perform **exploratory data analysis (EDA)** on Udemy course data.
* To answer analytical questions related to:

  * Course subjects
  * Pricing
  * Popularity
  * Yearly trends
  * Subscriber levels

---

## Tools and Libraries Used

* **Python**
* **Pandas** – for data cleaning and analysis
* **NumPy** – for numerical operations
* **Matplotlib** – for data visualization
* **Seaborn** – for advanced plots

---

## Steps and Tasks Performed

### ## Data Preprocessing

* Imported Udemy dataset into Python using Pandas.
* Performed initial inspection using:

  * `.head()`, `.info()`, `.describe()`, `.shape()`
* Checked and handled:

  * **Null values**
  * **Duplicate records**
  * **Data types of each column**

---

### ## Exploratory Data Analysis (EDA)

Performed detailed analysis to answer the following questions:

1. **What are all the different subjects for which courses are offered?**

   * Extracted all unique subjects using `.unique()` on the **subject** column.

2. **Which subject has the maximum number of courses?**

   * Counted number of courses per subject using `.value_counts()`.
   * Visualized using a **bar plot** for better comparison.

3. **Show all the courses which are free of cost.**

   * Filtered dataset where `is_paid == False`.

4. **Show all the courses which are paid.**

   * Filtered dataset where `is_paid == True`.

5. **Which is the top-selling course?**

   * Found the course with the **maximum number of subscribers** using `.max()` on `num_subscribers`.

6. **Which is the least selling course?**

   * Found the course with the **minimum number of subscribers** using `.min()`.

7. **Show all the Graphic Design courses where the price is less than 100.**

   * Filtered where `subject == 'Graphic Design'` and `price < 100`.

8. **List out all the courses related to Python.**

   * Used string matching on course titles using:

     ```python
     df[df['course_title'].str.contains('Python', case=False)]
     ```

9. **What are the courses published in the year 2015?**

   * Extracted courses where `published_timestamp` contains year `2015`.

10. **What is the maximum number of subscribers for each level of courses?**

    * Grouped data by `level` and found `max(num_subscribers)` for each.
    * Displayed results in a tabular format.

---

## Visualizations

* Created **bar charts**, **count plots**, and **histograms** using Seaborn and Matplotlib to:

  * Compare subjects
  * Analyze free vs paid courses
  * Visualize price distributions
  * Show subscribers by level

---

## Insights Gained

* Identified the **most popular subjects** on Udemy.
* Discovered trends in **pricing and subscription** patterns.
* Found that **Python-related courses** have high engagement.
* Observed course publication trends over the years.
* Understood the relationship between **course level** and **subscriber count**.

---

## Conclusion

* This analysis provides clear insights into Udemy’s course patterns, audience preferences, and pricing strategies.
* The project demonstrates a complete **data analysis workflow**, from **data cleaning** to **visual insights**.
* The same workflow can be used to analyze other e-learning platforms or educational datasets.

---

🔗 [View the Project](https://github.com/Dharani1202/Udemy-Data-Analysis)

---

