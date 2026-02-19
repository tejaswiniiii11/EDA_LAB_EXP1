# IMPLEMENTATION OF ACADEMIC PERFORMANCE DATA VISUALIZATION USING R

**Name:** Tejaswini M  
**Register Number:** 23BAD121  
**Course:** Exploratory Data Analysis & Visualization

----------------------------------------------

## 📌 Project Overview

This project focuses on designing appropriate data charts to analyze and compare academic performance indicators.

An autonomous engineering college aims to evaluate internal assessment performance of first-year students across five subjects to identify difficult courses and enhance teaching strategies.

This lab demonstrates how bar charts, line graphs, and pie charts can be used to interpret academic trends effectively.

-------------------------------------------------

## 🗂️ Dataset Information

**File Name:** `student_performance.csv`  
**Type:** CSV file containing student academic performance records  

-------------------------------------------------

## 📄 Key Attributes

- **Subject** – Name of subject  
- **Internal_Test1** – Marks obtained in Internal Test 1  
- **Internal_Test2** – Marks obtained in Internal Test 2  
- **Final_Grade** – Final grade assigned to each student  

The dataset represents internal assessment performance across multiple engineering subjects.

-------------------------------------------------

## 🛠️ Tools & Libraries Used

### Software
- R  
- RStudio  

### Libraries
- `ggplot2` – Data visualization  
- `dplyr` – Data manipulation and aggregation  
- `tidyr` – Data reshaping using `pivot_longer()`  

------------------------------------------------

## ⚙️ Implementation Steps

### 1️⃣ Data Loading & Preprocessing

- Imported dataset using `read.csv()`  
- Inspected structure using `str()` and `summary()`  
- Computed average internal marks:  
  `Avg_Internal = (Internal_Test1 + Internal_Test2) / 2`  

------------------------------------------------

### 2️⃣ Bar Chart – Subject-wise Average Marks

- Grouped data by Subject  
- Calculated mean of average internal marks  
- Created bar chart using `geom_bar()`  

📊 **Output:** Subject-wise Average Internal Marks  

------------------------------------------------

### 3️⃣ Line Chart – Performance Trend Across Tests

- Calculated average marks for Internal Test 1 and Internal Test 2  
- Reshaped data using `pivot_longer()`  
- Generated line chart with `geom_line()` and `geom_point()`  

📊 **Output:** Performance Trend Across Tests (Internal 1 vs Internal 2)  

------------------------------------------------

### 4️⃣ Pie Chart – Grade Distribution

- Counted frequency of each Final Grade using `count()`  
- Converted counts to percentages  
- Used `coord_polar()` to create pie chart representation  

📊 **Output:** Final Grade Distribution  

------------------------------------------------

## 📈 Visualizations Generated

- Bar chart of subject-wise average internal marks  
- Line chart showing performance trend across tests  
- Pie chart representing overall grade distribution  

All visualizations were created using `ggplot2`.

------------------------------------------------

## 🎯 Key Insights

- Identifies subjects with lower average marks (indicating higher difficulty)  
- Compares improvement or decline between Internal Test 1 and Test 2  
- Displays overall grade distribution to understand performance balance  

These visualizations support data-driven academic evaluation and teaching strategy improvement.
