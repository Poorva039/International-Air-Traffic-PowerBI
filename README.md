# ✈️ International Air Traffic Analysis – Power BI Dashboard  
*Interactive Data Visualization of Passenger and Freight Traffic (2015–2017)*

![Dashboard Preview](Images/Air%20Traffic%20first%20Dashboard.png)

---

## 🧭 Project Overview

This Power BI project analyzes international air traffic to and from India from 2015 to 2017. It uses multiple datasets to uncover trends in passenger volume, freight movement, and airline performance across cities and countries.

---

## 🔍 Project Objectives

- Identify peak air traffic quarters and top-performing airlines  
- Analyze passenger and freight trends over time  
- Visualize city-to-city and country-to-country travel flows  
- Forecast future travel volumes  
- Identify key influencers behind traffic changes

---

## 📊 Key Visualizations

### 📈 1. Forecasting Passenger Trends  
![Forecast](Images/Forecast.png)

### 💡 2. Key Influencers for Freight Drop  
![Key Influencers](Images/Key%20Influencers.png)

### 🧩 3. Decomposition Tree  
![Decomposition Tree](Images/Decomposition%20tree.png)

### 🗺️ 4. Flow Map of Travel Routes  
![Flow Map](Images/Flow%20map.png)

### 🌍 5. Country-Wise Passenger Traffic  
![Country-Wise Passengers](Images/Country%20wise%20Passengers%20Air%20Traffic.png)

### 📦 6. Country-Wise Freight Movement  
![Freight by Country](Images/Country%20wise%20Freight%20Air%20Traffic.png)

### 🏙️ 7. City-Level Air Traffic Overview  
![City Traffic](Images/City%20wise%20Air%20Traffic.png)

### 🛫 8. Top 10 Airlines by Passenger Volume  
![Top 10 Airlines](Images/Top%2010%20Airline%20for%20Passenger%20travel.png)

### 📅 9. Monthly Trends of Passenger & Freight  
![Monthly Traffic](Images/Comparison%20of%20Passenger%20and%20Freight%20Traffic.png)

---

## 🧰 Tools & Techniques Used

- **Power BI Desktop**
- **Power Query Editor (M Language)**
- **DAX (Data Analysis Expressions)**
- **Star Schema data modeling**
- **AI Visuals & Forecasting**
- **Interactive dashboard design** with slicers, bookmarks, and drilldowns

---

## 💡 DAX Usage Highlights

Also used to:
- Rank top airlines  
- Create filters by year, month, quarter  
- Define forecast series using time intelligence functions

Example DAX:
```DAX
Total Passengers = [Passengers From India] + [Passengers To India]
Freight Difference = [Freight From India] - [Freight To India]
---

### 💡 Additional DAX Applications

Also used to:
- Rank top airlines  
- Create filters by year/month/quarter  
- Define forecast series with time intelligence  

---

### 🔄 Power Query (M Language)

Used for data cleaning and transformation:
- Removed nulls, blanks, and duplicates  
- Merged `Year` and `Month` to form a `Date` column  
- Changed data types using M syntax like:
```m
Table.TransformColumnTypes(Source,{{"Passengers From India", Int64.Type}})
