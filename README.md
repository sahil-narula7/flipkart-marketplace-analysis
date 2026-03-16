# Flipkart Marketplace Product & Vendor Opportunity Analysis

![Flipkart Marketplace Opportunity Dashboard]("dashboard.png")

## Project Overview

This project analyzes **~20,000 Flipkart marketplace product listings** to identify **high-demand categories, vendor performance patterns, and pricing opportunities**.

The objective was to simulate how a **startup or marketplace analyst could identify profitable product opportunities using marketplace data.**

The analysis was conducted using **Microsoft Excel with data cleaning, pivot tables, and dashboard visualization.**

---

# Dataset

The dataset contains approximately **19,922 Flipkart marketplace listings** including:

* Product Category
* Vendor / Seller
* Selling Price
* Discount Percentage
* Customer Rating

The dataset represents **Flipkart marketplace product listings across multiple categories.**

---

# Project Objectives

The analysis answers four key business questions:

1. Which product categories show **high demand but lower competition?**
2. Which vendors demonstrate **strong product performance?**
3. What **price segments dominate marketplace demand?**
4. Where are the **potential product opportunity gaps for new sellers?**

---

# Data Preparation

Before analysis, several preprocessing steps were performed.

### Data Cleaning Steps

* Extracted **primary product categories** from messy category strings
* Created **price segments** (Low / Mid / Premium)
* Calculated **discount percentage**
* Created a custom **Demand Score metric**
* Handled **missing ratings using conditional formulas**
* Removed spreadsheet errors such as `#DIV/0`

These steps transformed the raw dataset into a **structured format suitable for pivot analysis.**

---

# Demand Score Metric

To estimate product demand, a custom metric was created.

```
Demand Score = (Rating + Discount) × log(Selling Price)
```

The metric combines:

* Customer satisfaction (ratings)
* Pricing attractiveness (discount)
* Product value perception (price)

This helps approximate **marketplace demand signals even when ratings are missing.**

---

# Analysis Performed

## 1. Category Demand Analysis

Compared:

* Number of product listings
* Average demand score per category

Purpose:

Identify **high-demand categories with relatively lower competition.**

---

## 2. Vendor Performance Analysis

Analyzed vendors based on:

* Number of products listed
* Average demand score

Purpose:

Identify vendors with **strong performing products.**

---

## 3. Demand by Price Segment

Products were grouped into three segments:

* Low Price
* Mid Price
* Premium

Purpose:

Understand which **price ranges dominate marketplace demand.**

---

## 4. Category Distribution by Price Segment

Compared category listings across price segments.

Purpose:

Identify **market gaps and potential product launch opportunities.**

---

# Key Insights

### 1. Clothing category is highly competitive

The **Clothing category has the highest number of listings (~6000+)**, indicating strong competition despite moderate demand scores.

---

### 2. Mid-price products dominate the marketplace

Most listings fall within the **mid-price segment**, suggesting this price range drives the majority of marketplace activity.

---

### 3. Technology categories show strong demand

Categories such as **Computers and Watches** show relatively **higher demand scores with fewer listings**, indicating strong product potential.

---

### 4. Vendor performance differences

Some vendors achieve **higher demand scores with fewer products**, suggesting stronger **product-market fit.**

---

### 5. Premium product opportunity

Several categories have **limited premium offerings**, suggesting potential opportunities for **premium product launches.**

---

# Challenges Faced

### Messy Category Data

Category fields contained complex text strings.

Solution:

Used **Excel text functions** to extract primary categories.

---

### Missing Ratings

Many products lacked ratings.

Solution:

Used **conditional formulas** to estimate demand score using discount and price.

---

### Chart Scale Issues

Product counts were large compared to demand score values.

Solution:

Used **secondary axis combo charts**.

---

### Overcrowded Charts

Too many vendors and categories made charts difficult to read.

Solution:

Applied **Top-N filtering in pivot tables.**

---

# Tools Used

* Microsoft Excel
* Pivot Tables
* Pivot Charts
* Data Cleaning Functions
* Data Visualization

---

# Business Value

This project demonstrates how marketplace data can help businesses:

* Identify **high-demand product categories**
* Evaluate **vendor performance**
* Understand **pricing strategies**
* Detect **product opportunity gaps**

These insights can support **data-driven product launch decisions for startups and marketplace teams.**

---

# Project Structure

```
Flipkart-Marketplace-Analysis
│
├── flipkart_marketplace_analysis.xlsx
├── dashboard.png
└── README.md
```

---

# Interview Explanation (Short Version)

Analyzed ~20K Flipkart marketplace listings using Excel to identify high-demand categories, vendor performance patterns, and pricing opportunities through pivot analysis and a custom demand scoring metric.

---

# Author

**Sahil Narula**

GitHub
https://github.com/sahil-narula7
