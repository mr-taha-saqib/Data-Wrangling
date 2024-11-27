# Exploratory Data Analysis (EDA) on Adult Dataset

## Overview  
This project involves performing Exploratory Data Analysis (EDA) using **NumPy** and **Pandas** on the `adult.data` dataset. The tasks include data wrangling, answering specific analytical questions, and visualizing the findings.

---

## 1.1 Data Wrangling (20 Marks)  
Apply the following processes to clean and prepare the dataset:  
- **Noisy Data**: Remove or handle noisy data points.  
- **Outliers**: Detect and address outliers using statistical methods or visualizations.  
- **Missing Values**: Handle missing values appropriately (impute or drop).  
- **Redundant Features**: Identify and remove redundant or irrelevant features.  
- **Correlation and Covariance**: Analyze relationships between features.

### Visualization  
Provide visual evidence (e.g., histograms, scatter plots, box plots, and heatmaps) for each process. Explain the rationale behind each visualization.

---

## Analytical Questions  

### 1. Count the number of men and women in the dataset.  
- Use `value_counts()` on the gender column.  
- Visualize the gender distribution using a **bar plot**.

---

### 2. Find the average age of women in the dataset.  
- Filter the dataset by gender (`"Female"`) and calculate the average age using `mean()`.  
- Display the age distribution of women using a **box plot**.

---

### 3. Count the number of United States citizens.  
- Filter the dataset where `native-country == "United-States"` and count the rows.  
- Use a **pie chart** to compare the number of U.S. citizens to other countries.

---

### 4. Analyze salary groups (>50K and <=50K):  
- **Find mean and standard deviation of age** for both salary groups.  
- Visualize age distributions using **histograms** for each salary group.

---

### 5. High School Education and High Salary:  
- Check if individuals earning more than 50K have at least high school education.  
  (High school education includes `Bachelors`, `Prof-school`, `Assoc-acdm`, `Assoc-voc`, `Masters`, and `Doctorate`.)  
- Answer using a **Yes/No** format.  
- Visualize the distribution of education levels using a **bar chart**.

---

### 6. Race and Gender Statistics:  
- Use `groupby()` and `describe()` to generate statistics for `age` grouped by `race` and `gender`.  
- Find the **maximum age** of men in the `Amer-Indian-Eskimo` race.  
- Display age statistics using **box plots** for each gender and race.

---

### 7. Proportion of High Earners: Married vs. Single Men:  
- Define married individuals as those whose `marital-status` starts with `"Married"`.  
- Compare the proportion of high earners (>50K) among married and single men.  
- Visualize proportions using a **stacked bar chart**.

---

### 8. Maximum Hours Worked Per Week:  
- Identify the **maximum hours-per-week** value.  
- Count how many people work such hours and calculate the percentage of those earning >50K.  
- Visualize the number of people working maximum hours using a **bar chart**.

---

### 9. Average Working Hours by Country:  
- Use `groupby(["native-country", "salary"])` to calculate the average working hours for each salary group (`<=50K` and `>50K`).  
- Visualize the data using a **heatmap** to compare working hours across countries.

---
