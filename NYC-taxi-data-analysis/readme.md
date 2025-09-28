# 🚕 NYC Taxi Data Analysis with Apache Spark

Welcome! This project is a beginner-friendly, end-to-end example of using **Apache Spark** to analyze real-world **NYC Yellow Taxi trip data**. Even if you're new to Spark or big data tools, this project will guide you step-by-step through loading, cleaning, analyzing, and saving insights from millions of taxi trip records.

---

## 📘 What is Apache Spark?

Apache Spark is a powerful open-source engine used to process large datasets very quickly. Unlike traditional tools that may slow down with big files, Spark is designed to handle **big data efficiently**, either on your computer or across many machines.

In this project, we use **PySpark** — the Python interface to Spark.

---

## 🧠 What You'll Learn

- What Spark is and how to use it with Python
- How to load and explore a large real-world dataset
- How to clean and transform raw data using Spark
- How to analyze trip patterns (duration, distance, zones, demand)
- How to identify inefficiencies (e.g., long trip times for short distances)
- How to save processed data and analysis results

---

## 📂 Dataset Used

- **NYC Yellow Taxi Trip Data (January 2023)**  
  📁 File: `yellow_tripdata_2025-08.parquet`  
  📎 Source: [NYC Taxi & Limousine Commission](https://www.nyc.gov/site/tlc/about/tlc-trip-record-data.page)

- **Taxi Zone Lookup Table**  
  📁 File: `taxi_zone_lookup.csv`  
  📎 Maps location IDs to readable zone names.

---

## 📊 Project Workflow

1. **Load** the taxi trip and zone data
2. **Clean** the data (remove invalid trips)
3. **Enhance** the data by calculating trip duration and joining with zone names
4. **Analyze**:
   - Top pickup zones
   - Average trip duration by hour
   - Find trips with high duration but low distance
5. **Save** the results to CSV or Parquet

---

## ▶️ How to Run This Project

### 🔧 Requirements

- Python 3.x
- PySpark
- Jupyter Notebook (or run in Google Colab / Databricks)

### 📦 Install Dependencies

If you're running locally, install PySpark:

```bash
pip install pyspark
````

You may also need:

```bash
pip install jupyter pandas matplotlib
```

### 🖥️ Run the Notebook

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/nyc-taxi-spark.git
   cd nyc-taxi-spark
   ```

2. Launch the notebook:

   ```bash
   jupyter notebook
   ```

3. Open `nyc_taxi_analysis.ipynb` and follow the cells.

---

## 📁 Project Structure

```
nyc-taxi-spark/
│
├── yellow_tripdata_2025-08.parquet       # Main trip data (downloaded)
├── taxi_zone_lookup.csv                  # Location ID to Zone name mapping
├── nyc_taxi_analysis.ipynb               # Main notebook
└── README.md                             # This file
```

---

## 📈 Sample Outputs

* **Top Pickup Zones**: Shows which parts of NYC have the highest demand.
* **Trip Duration by Hour**: Reveals traffic patterns over the day.
* **Long Wait, Short Distance**: Highlights inefficiencies — possibly traffic jams or poor routing.

---

## 🙋 FAQ

**Q: Do I need a cluster or Spark installed?**
A: No! This project runs fine on a regular laptop using PySpark locally.

**Q: Is this project beginner-friendly?**
A: Absolutely. The code is well-commented, and each step is explained.

**Q: Can I use Google Colab or Databricks?**
A: Yes. You can upload the notebook to either platform and run it there (just make sure the data files are available).
