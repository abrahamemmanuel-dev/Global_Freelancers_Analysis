# 📊 Global Freelancers Analysis: Interactive Excel Dashboard

An interactive Excel dashboard that analyses **1,000 global freelancers** by primary skill, performance (rating), experience, pricing, language, country, and activity status.

### Table of Contents
- [Project Overview](#project-overview)
- [Business Questions](#business-questions)
- [Dataset](#dataset)
- [Data Cleaning & Preparation](#data-cleaning--preparation)
- [Tools & Techniques](#tools--techniques)
- [Dashboard Components](#dashboard-components)
- [Key Insights](#key-insights)
- [How to Use](#how-to-use)
- [Repository Structure](#repository-structure)
- [Recommendations](#recommendations)
- [Author](#author)

<img width="2260" height="1084" alt="Dashboard" src="https://github.com/user-attachments/assets/3130bc85-abc2-482a-9507-0848849f5268" />


---

### 📌 Project Overview

Freelance platforms need to understand who their talent is, where they are, what they charge, and how well they perform. This project cleans a raw freelancer dataset and turns it into a single-page, slicer-driven dashboard that answers those questions at a glance.

### 🎯 Business Questions

- How many freelancers are on the platform, and what is the gender split?
- Which primary skills earn the highest average rating?
- How is experience distributed across the freelancer base?
- What hourly rates are most common?
- Which languages and countries are most represented?
- How do the answers change for **Active** vs **Not Active** freelancers?

### 🗂️ Dataset

| Field | Description |
|---|---|
| `Freelancer_ID` | Unique freelancer identifier |
| `Full Name` | Cleaned name (titles removed) |
| `Gender` | Standardised to Male / Female |
| `Age` | Age of the freelancer |
| `Country` / `Language` | Location and spoken language |
| `Primary Skill` | Main service offered (e.g. DevOps, AI, UI/UX Design) |
| `Years of Experience` | Raw years, grouped into buckets (0-5, 6-10, 11-15, 16-20, 20+) |
| `Hourly Rate` | Rate in USD, cleaned from text such as "USD 100" |
| `Rating` | Platform rating |
| `Status` | Active / Not Active |
| `Client Satisfaction` | Client satisfaction score |

**Records:** 1,000 freelancers

### 🧹 Data Cleaning & Preparation

- Standardised inconsistent gender entries (`f`, `FEMALE`, etc.) into **Male / Female**
- Removed titles and prefixes from names to create a clean `Full Name`
- Stripped the `USD` text from hourly rates and converted them to numbers
- Grouped years of experience into five buckets
- Converted the activity flag into a readable **Active / Not Active** status
- Handled blank values so they are visible and not silently dropped

### 🛠️ Tools & Techniques

- **Microsoft Excel**
- Formulas (`IF`, `LOWER`, `LEFT`, `SUBSTITUTE`)
- **PivotTables** and **PivotCharts**
- **Slicers** for interactive filtering (Primary Skill, Status)
- Dashboard layout and formatting

### 📈 Dashboard Components

| Visual | Purpose |
|---|---|
| **KPI Card** | Total freelancers (1,000) |
| **Pie Chart** | Gender split (51% Male / 49% Female) |
| **Column Chart** | Average rating by primary skill |
| **Column Chart** | Years of experience distribution |
| **Column Chart** | Hourly rate distribution |
| **Bar Chart** | Freelancer count by language |
| **Bar Chart** | Freelancer count by country |
| **Slicers** | Filter everything by Primary Skill and Status |

### 🔍 Key Insights

- **DevOps** has the highest average rating (**2.8**), while **Blockchain Development** is lowest (**2.4**).
- The gender split is nearly even: **51% Male** and **49% Female**.
- **39%** of freelancers have **0-5 years** of experience, the largest group.
- **40 USD/hour** is the most common rate band (**17%**).
- **English (215)** and **Spanish (142)** are the most common languages.
- **South Korea (68)** and **Canada (65)** have the most freelancers; the rest of the countries fall in a narrow 31-52 range.

### 🚀 How to Use

1. Download `Global_Freelancers_Analysis.xlsx` from the `data/` folder.
2. Open it in Microsoft Excel (2013 or later, since slicers are required).
3. Go to the **Dashboard** sheet.
4. Click the **Primary Skill** or **Status** slicers to filter all charts at once.
5. Use the clear-filter icon at the top right of a slicer to reset.

### 📁 Repository Structure

```
global-freelancers-dashboard/
├── README.md
├── data/
│   └── Global_Freelancers_Analysis.xlsx
├── images/
│   └── dashboard.png
└── docs/
    └── data_dictionary.md   (optional)
```

### 💡 Recommendations

- Invest in onboarding and upskilling for the large early-career segment.
- Investigate why lower-rated skills (e.g. Blockchain, AI) underperform.
- Grow talent in under-represented languages and regions.

### 👤 Author

**Abraham Emmanuel**

Mathematician | Data Analyst | Data Scientist | Lead, Creative Designer | Brand Guide Developer |

📧 uchebutone@gmail.com
🔗 [LinkedIn](https://www.linkedin.com/in/abraham-emmanuel-35a746193/) | [GitHub](https://github.com/your-username)

---

⭐ If you found this project useful, please give it a star!
