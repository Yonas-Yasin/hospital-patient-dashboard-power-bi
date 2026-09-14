# Hospital Patient Dashboard (Power BI)

An end-to-end healthcare analytics report built in Microsoft Power BI. The project covers data preparation in Power Query, a star-schema data model with a dedicated date dimension, DAX measures, and a four-page interactive report with a custom mobile layout.

## Project Overview

The report analyses hospital admissions data to answer operational, clinical, and financial questions:

- How many admissions and patients are handled, and how does volume change over time?
- Which hospitals, departments, and doctors carry the highest workload?
- How is revenue split between insurance and out-of-pocket payments?
- How satisfied are patients, and how does satisfaction relate to billing and recovery outcomes?

## Dashboard Pages

| Page | Purpose | Key Visuals |
|---|---|---|
| **Executive Overview** | High-level summary of activity and revenue | KPI cards (Total Admissions, Total Patients, Avg Satisfaction, Total Revenue), admissions per month, admissions by type, hospital ranking; slicers for year, admission type, and hospital |
| **Department Analysis** | Workload and efficiency by department | Admissions by department, average length of stay by department, admissions by doctor, department-versus-hospital matrix; department slicer |
| **Financial Summary** | Revenue composition and insurance coverage | KPI cards, insurance-rate gauge, insurance versus out-of-pocket share by department, revenue by hospital (treemap), revenue by month and year |
| **Quality & Satisfaction** | Patient experience and outcomes | Satisfaction by doctor and by department, bill amount versus satisfaction (scatter), patient status breakdown with recovery rate |

## Mobile-Optimised Layout

Each report page includes a dedicated mobile layout so the dashboard remains readable in the Power BI mobile application.

## Data Model

- **Admissions** – fact table containing admission records (hospital, department, doctor, admission type, status, billing, and satisfaction fields).
- **DimDate** – date dimension used for year and month analysis.
- **_Measures** – a dedicated table holding all DAX measures.

## Key Measures

| Measure | Description |
|---|---|
| Total Admissions | Number of admission records |
| Total Patients | Number of distinct patients |
| Total Revenue | Sum of billed amounts |
| Total Insurance | Portion of revenue covered by insurance |
| Total Out of Pocket | Portion of revenue paid directly by patients |
| Insurance Rate % | Share of revenue covered by insurance |
| Avg Bill | Average bill per admission |
| Avg Length of Stay | Average number of days per admission |
| Avg Satisfaction | Average patient satisfaction score |
| Recovery Rate % | Share of admissions with a recovered status |

## Key Features

- Interactive slicers and cross-filtering between visuals
- KPI cards for headline metrics
- Back button for returning to the previous page
- Consistent, accessible colour theme across all pages
- Separate desktop and mobile layouts

## Tools and Technologies

- Microsoft Power BI Desktop
- Power Query (data transformation)
- DAX (Data Analysis Expressions)
- Power BI Mobile

## Viewing the Project

1. Install [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (Windows).
2. Download `HC_Patient_Dashboard.pbix` from this repository.
3. Open the file in Power BI Desktop and use the page tabs to navigate the report.

## Data Note

The dataset was provided for educational purposes as part of a data analytics training programme. It is not intended for operational or clinical decision-making.

## Author

**Yonas Yasin** – [GitHub](https://github.com/Yonas-Yasin)
