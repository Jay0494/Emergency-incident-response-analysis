# 🚨 Emergency Incident Response Analysis

## 📌 Overview

This project analyses emergency incident data to evaluate **response performance, operational efficiency, and demand patterns**.

The focus is not just on response speed, but on identifying:

> **Where delays occur in the incident lifecycle and how response effectiveness can be improved**

---

## 🎯 Business Question

**Where are delays and inefficiencies occurring in the incident lifecycle, and how can operations be optimised?**

---

## 📊 Dashboard Preview

<img width="1279" height="765" alt="dashboard" src="https://github.com/user-attachments/assets/ddec8abe-3d35-473b-9284-454c84446ce0" />


---

## 🧠 Data Model

This project uses a **star schema** for efficient querying and scalable analysis.

<img width="981" height="645" alt="DATA MODEL" src="https://github.com/user-attachments/assets/c8b596d8-47c0-410a-a4aa-727fcee60ea8" />

### Fact Table

* `fact_incident`

  * Stores all incident-level records
  * Includes timestamps, dispatch details, escalation flags

### Dimension Tables

* `dim_date_table` → Time-based analysis
* `dim_location` → City and region insights
* `dim_incident_type` → Incident classification
* `dim_incident_location` → Location type (home, hospital, etc.)
* `dim_dispatcher` → Response teams and modes
* `dim_intervention_type` → Treatment type

### Modelling Approach

* One-to-many relationships (dimensions → fact)
* Dedicated date table for time intelligence
* Derived lifecycle metrics for delay analysis

---

## 📈 Key Metrics

* Total Incidents
* Average Response Time
* Average Dispatch Delay
* High Priority Incident Rate (%)
* Incidents Resolved On-Site (%)

---

## 🔍 Key Insights

* **55.9% of incidents occur at home**
  → Demand is primarily community-based

* **Mental health incidents are the most common**
  → Significant overlap between emergency response and healthcare

* **Dispatch delay averages 14.8 minutes**
  → Major bottleneck occurs before response begins

* **Only 30.2% of incidents are resolved on-site**
  → High escalation rate increases system pressure

* **36.2% of incidents are high priority**
  → Indicates potential strain on resources

* **57.1% of incidents occur on weekends**
  → Demand is not aligned with typical staffing patterns

* **Seasonal spikes observed (Sep–Oct)**
  → Demand is predictable but underutilised operationally

---

## 💡 Recommendations

* **Optimise dispatch processes** to reduce pre-response delays
* **Introduce specialised mental health response units**
* **Improve on-site resolution capability** to reduce escalations
* **Adopt dynamic resource allocation** based on demand patterns
* **Leverage predictive analytics** for proactive planning

---

## 🛠️ Tools & Technologies

* Power BI
* DAX
* Data Modelling (Star Schema)

---

## 📌 Key Takeaway

This project demonstrates how data can move beyond reporting to:

> **Identify operational bottlenecks and drive real-world performance improvements**

---

## 👤 Author

**Elijah Okpako**
Data Analyst | Power BI | SQL | Operational Analytics

---
