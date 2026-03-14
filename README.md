## Context

Business communities in the United States face a high demand for skilled human resources. One of the biggest challenges for organizations is identifying and attracting the right talent, which is essential to remain competitive. Companies in the United States actively seek talented and qualified individuals both locally and internationally.

The **Immigration and Nationality Act (INA)** allows foreign workers to come to the United States for work on either a temporary or permanent basis. At the same time, the act protects U.S. workers from adverse impacts on wages and working conditions by ensuring that employers comply with statutory requirements when hiring foreign workers.

These immigration programs are administered by the **Office of Foreign Labor Certification (OFLC)**.

The OFLC processes job certification applications for employers seeking to hire foreign workers. Certifications are granted only when employers can demonstrate that:

- There are **not enough qualified U.S. workers** available for the job.
- The wages offered **meet or exceed the prevailing wage** for the occupation in the intended employment area.

---

## Objective

In **FY 2016**, the OFLC processed **775,979 employer applications** for **1,699,957 positions** for temporary and permanent labor certifications. This represented a **9% increase** in the total number of processed applications compared to the previous year.

As the number of applicants continues to grow each year, manually reviewing every application is becoming increasingly **time-consuming and inefficient**.

This situation calls for a **Machine Learning–based solution** that can help shortlist candidates who have a **higher probability of visa approval**.

The OFLC has hired **EasyVisa** to develop a **data-driven solution**. As a **Data Scientist at EasyVisa**, the goal is to analyze the data and build a **classification model** that can:

- Facilitate the **visa approval decision-making process**.
- Recommend **which applications should be certified or denied** based on the factors that significantly influence visa approval.

---

## Data Description

The dataset contains various attributes related to the **employee and employer involved in the visa application process**.

---

## Data Dictionary

| Feature | Description |
|-------|-------------|
| **case_id** | Unique ID of each visa application |
| **continent** | Continent of the employee |
| **education_of_employee** | Education level of the employee |
| **has_job_experience** | Whether the employee has job experience (Y = Yes, N = No) |
| **requires_job_training** | Whether the employee requires job training (Y = Yes, N = No) |
| **no_of_employees** | Number of employees in the employer's company |
| **yr_of_estab** | Year in which the employer's company was established |
| **region_of_employment** | Intended region of employment in the U.S. |
| **prevailing_wage** | Average wage paid to similarly employed workers in the same occupation and location |
| **unit_of_wage** | Unit of prevailing wage (Hourly, Weekly, Monthly, Yearly) |
| **full_time_position** | Whether the position is full-time (Y = Full-Time, N = Part-Time) |
| **case_status** | Target variable indicating whether the visa was **certified or denied** |


## Key Highlights

- Addressed **class imbalance** using **over-sampling and under-sampling techniques**.
- Built and compared multiple classification models:
  - Decision Tree
  - Bagging
  - Random Forest
  - AdaBoost
  - Gradient Boosting
- Applied **Grid Search and Randomized Search** for **hyperparameter tuning**.
- Selected **Gradient Boosting (Grid Search tuned)** as the **final model** with a strong **F1-score (~0.82)** on test data.
- Identified key drivers influencing visa approval:
  - **Education Level**
  - **Job Experience**
  - **Prevailing Wage**
  - **Employment Type**

---

## Business Impact

The final model provides a **data-driven framework** to help prioritize **high-probability visa applications** while maintaining a **balanced trade-off between precision and recall**.

This approach can assist immigration authorities and organizations in **improving efficiency and decision-making during the visa approval process**.

---

## Skills Demonstrated

- Exploratory Data Analysis (EDA)
- Data Preprocessing
- Handling Class Imbalance
- Classification Modeling
- Hyperparameter Tuning
- Model Evaluation (F1-score, Precision, Recall)
- Business Insights from Machine Learning Models
