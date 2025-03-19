# 5240 Project - Addressing the Lack of Public Space for Teenagers  

## 📌 Project Overview  
This project explores the **availability and accessibility of public recreation spaces** for teenagers in North Dallas. Using **data processing and analytics tools**, we aim to provide **insights for better urban planning** and community engagement.  

## 🛠️ Technologies Used  
- **Google Cloud Platform (GCP)** – Data storage and processing  
- **Apache Hive & Spark** – Query execution and analysis  
- **BigQuery** – SQL-based data analysis  
- **OpenRefine** – Data cleaning and transformation  
- **Python & SQL** – Data processing and querying  

## 📊 Datasets Used  
1. **Chicago Park District Facilities Dataset**  
   - Source: [City of Chicago Open Data](https://data.cityofchicago.org/Parks-Recreation/Parks-Chicago-Park-District-Facilities)  
   - Provides details on park locations, amenities, and accessibility.  
2. **Washington, D.C. Open Data - Real-Time Recreation Facilities Dataset**  
   - Source: [DC Open Data](https://opendata.dc.gov/datasets/Recreation-Facilities)  
   - Contains real-time geospatial data on public spaces.  

## 🔍 Key Findings  
✅ **Identified Gaps** – Locations with no or limited public recreational spaces.  
✅ **Utilization Patterns** – Understanding which spaces are underused or overcrowded.  
✅ **Optimization Opportunities** – Recommending ways to improve or repurpose existing spaces.  

## 📂 Project Implementation  
### **Data Processing**  
- **Converted text-based identifiers (e.g., OBJECTID, PARK_NO) into numerical values** for better analysis.  
- **Filled missing data** in key attributes to improve dataset consistency.  
- **Stored and analyzed datasets** in **Google Cloud Storage, BigQuery, Hive, and Spark**.  

### **Query Execution**  
- **BigQuery, Hive, and Spark** were used to analyze recreation facility data.  
- Sample query for identifying **indoor recreational spaces**:  
  ```sql
  SELECT PARK, FACILITY_N, FACILITY_T  
  FROM adta5240project-443220.CDPFacilities.CPDFacilities  
  WHERE FACILITY_T = 'Indoor';
