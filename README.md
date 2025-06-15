
# End-to-End-BI-Project-with-Microsoft-Fabric-Sales-Analytics

This repository showcases a complete Business Intelligence (BI) project built using **Microsoft Fabric**, starting from raw data ingestion to building interactive Power BI reports. The project leverages modern data architecture, including Lakehouse, Dataflows, Notebooks, Semantic Modeling, and Pipelines for automation.

---

## 🔍 Project Overview

The goal of this project is to analyze sales data from multiple years using a structured BI pipeline. The project covers:

- Ingesting raw CSV data from Azure
- Transforming data using Fabric Notebooks and Dataflows
- Creating a Lakehouse data model
- Building a Semantic Model with DAX measures
- Designing Power BI reports in Power BI Desktop
- Automating the entire workflow with Fabric Pipelines

---

## 🛠️ Tech Stack

| Layer              | Tool / Feature                 |
|--------------------|-------------------------------|
| Data Storage       | OneLake (Lakehouse)           |
| Data Ingestion     | Fabric Notebooks, Dataflows   |
| Data Modeling      | Semantic Model (Power BI)     |
| Visualization      | Power BI Desktop              |
| Automation         | Fabric Pipelines              |

---

## 🧩 Project Architecture

```

Azure Storage
↓
Lakehouse (Raw Zone)
↓
Fabric Notebook (Data Cleaning)
↓
Dataflow Gen2 (Staging + Transformation)
↓
Lakehouse (Final Tables)
↓
Semantic Model (Relationships + Measures)
↓
Power BI Desktop (Visualization)
↓
Fabric Pipeline (Automation & Scheduling)

```

---

## ✅ Key Highlights

- **Dataflow Gen2** was used to append multiple yearly sales datasets and create `Fact_Sales`.
- A rich **Dim_Date** table was generated with fields like Month Start, Day of Week, etc.
- DAX Measures such as `Total Sales`, `Order Count`, and `Average Order Value` were defined in the Semantic Model.
- **Power BI Desktop** was chosen for better layout, interaction design, and publishing flexibility.
- A **Pipeline** was created to run Notebook → Dataflow → Semantic Model refresh automatically.

![EXEC Dashboard](./images/EXEC%20Dashboard.png)

---

## 📊 Sample Insights

Here are a few sample views from the Power BI report:

### 🔹 Product Details

![Products Details](./images/Products%20Details.png)

---

### 🔹 Customer Details

![Customers Details](./images/Customers%20Details.png)

---

## 🧠 What I Learned

- Practical use of Microsoft Fabric for modern BI pipelines  
- Effective structuring of Lakehouse data  
- Hands-on experience with DAX and semantic modeling  
- Scheduling and automation using Pipelines

---

## 📂 Folder Structure

```

fabric-sales-bi-project/
│
├── notebooks/
│   └── sales\_data\_preparation.ipynb
│
├── dataflow/
│   └── dataflow\_definition.json
│
├── semantic-model/
│   └── model\_description.md
│
├── reports/
│   └── sales\_report.pbix
│
├── docs/
│   ├── project\_overview\.md
│   └── pipeline\_design.md
│
└── README.md

```

---

## 📬 Contact

Created by **Seyed Mojtaba Hosseini**  
[LinkedIn](https://www.linkedin.com/in/mojtaba-hosseini-0b38318b/) | [Email](mailto:hosseiny.mj69@yahoo.com)

؟
