# 🏙️ Quarterly Homelessness Trends: Hackney vs Neighbouring Local Authorities  

> **A data-driven project comparing homelessness patterns across Hackney and its nine neighbouring councils, using a fully automated Python–SQL–Power BI pipeline.**  
> Enables real-time KPI tracking and supports data-informed prevention strategies.

---

## 🎯 Aim  
Provide actionable insights into quarterly homelessness trends to help shape effective prevention policies across local authorities.

---

## 📊 Data  
Public datasets sourced from [GOV.UK](https://www.gov.uk/).

---

## 🧰 Tools & Technologies  

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?logo=postgresql&logoColor=white" alt="PostgreSQL"/>
  <img src="https://img.shields.io/badge/Power%20BI-F2C811?logo=powerbi&logoColor=black" alt="Power BI"/>
  <img src="https://img.shields.io/badge/Power%20Query-107C10?logo=microsoftpowerquery&logoColor=white" alt="Power Query"/>
  <img src="https://img.shields.io/badge/OneDrive-0078D4?logo=microsoftonedrive&logoColor=white" alt="OneDrive"/>
  <img src="https://img.shields.io/badge/PowerPoint-B7472A?logo=microsoftpowerpoint&logoColor=white" alt="PowerPoint"/>
</p>

---

## ⚙️ Process Overview  

![ETL Flow Diagram](flow_diagram_for_dashboard_project.png)

---

## 🧩 ETL Workflow Summary  

### 🐍 **Python (Data Preparation)**
- Extracted data from multiple Excel sources into pandas DataFrames  
- Cleaned, deduplicated, and standardised columns  
- Engineered `quarter_indicator`, `is_neighbouring_la`, and `delta` fields  
- Synced schemas between source and warehouse tables  
- Implemented delta comparison to load only new or updated records  
- Exported refined outputs to cloud-stored CSVs  

### 🗄️ **SQL (Transformation & Aggregation)**
- Filtered nine neighbouring local authorities: *Southwark, Islington, Haringey, Lambeth, Tower Hamlets, Camden, Waltham Forest, Hammersmith & Fulham, Newham*  
- Computed aggregates and merged results with Hackney data  
- Engineered time-sorting field `year_qtr`  
- Unpivoted/pivoted metrics for visualisation  
- Published final dataset as a SQL view for Power BI  

### 📊 **Power BI (Visualisation)**
- Connected to the cloud dataset via Power Query  
- Cleaned column headers and metric labels  
- Built DAX measures and interactive visuals  
- Published a live dashboard to Power BI Service  

---

## 📈 Dashboard Snapshots  

| Report Type | Preview |
|--------------|----------|
| 🏘️ Households & Initial Assessment | [View PDF](https://github.com/Beegie01/Comparing-Homelessness-Trends-in-Hackney-and-Neighbouring-Local-Authorities/blob/main/initial_assessment_report.pdf) |
| 🧾 Owed Prevention Duty | [View PDF](https://github.com/Beegie01/Comparing-Homelessness-Trends-in-Hackney-and-Neighbouring-Local-Authorities/blob/main/prevention_duty_report.pdf) |
| 🔁 Prevention Duty Ended | [View PDF](https://github.com/Beegie01/Comparing-Homelessness-Trends-in-Hackney-and-Neighbouring-Local-Authorities/blob/main/prevention_duty_ending_report.pdf) |
| 🚨 Owed Relief Duty | [View PDF](https://github.com/Beegie01/Comparing-Homelessness-Trends-in-Hackney-and-Neighbouring-Local-Authorities/blob/main/relief_duty_report.pdf) |
| ✅ Relief Duty Ended | [View PDF](https://github.com/Beegie01/Comparing-Homelessness-Trends-in-Hackney-and-Neighbouring-Local-Authorities/blob/main/relief_duty_ending_report.pdf) |
| 🏠 Households in Temporary Accommodation | [View PDF](https://githu)

---

## ✅ RECOMMENDATIONS<br>
1. Educate households on importance of encouraging friends or family members to apply early for their own housing options while relationships are still positive.
2. Encourage household members to report early signs of domestic abuse to help identify potential risks of homelessness and enable timely preventive measures.
3. Strengthen the council’s capacity to secure accommodation and expand its use of LA/HA stock to reduce reliance on more expensive alternatives.
4. Direct greater investment towards reducing the length of time families spend in temporary accommodation, in order to minimize the negative impact on growing children.
5. Investigate the root causes of unexpectedly high use of temporary accommodation by  single adult males.

---

### REPORT SUMMARY
Full version of this report is available [here](https://github.com/Beegie01/Comparing-Homelessness-Trends-in-Hackney-and-Neighbouring-Local-Authorities/blob/main/Hackney%20Quarterly%20Report%20-%20MAR2025.pdf).<br>
