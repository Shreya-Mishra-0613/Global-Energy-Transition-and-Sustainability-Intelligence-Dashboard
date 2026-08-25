# 🌍 Global Energy Transition & Climate Impact Dashboard

An interactive **Tableau dashboard project** for analyzing global energy transition, renewable energy adoption, carbon emissions, and climate impact using verified datasets from **Our World in Data (OWID)**.

The project transforms large, multi-year international datasets into two connected analytical dashboards that help users explore relationships between energy consumption, renewable adoption, CO₂ emissions, carbon intensity, and historical climate impact.

---

## 📌 Project Overview

The global transition toward cleaner energy is one of the most important challenges of the modern world. However, energy and climate datasets are often large, complex, and difficult to interpret directly.

This project integrates multiple energy and climate indicators into an interactive Tableau-based analytical solution. The dashboards support exploration of global energy transition patterns and climate-related indicators through interactive visualizations and filters.

### Key Questions Addressed

- Which countries consume the most energy?
- Which countries are leading renewable energy adoption?
- How does renewable energy share relate to CO₂ emissions?
- Which countries have the highest carbon-intensive electricity systems?
- Who are the largest current CO₂ emitters?
- Which countries have contributed most to historical global warming?

---

## 🎯 Problem Statement

Global energy and climate datasets contain large volumes of information across countries and years. Comparing countries across multiple indicators such as renewable energy adoption, energy consumption, carbon emissions, and climate impact can be difficult when working directly with raw data.

The objective of this project is to develop an interactive data visualization dashboard that integrates energy and climate datasets into meaningful visualizations for exploring global energy transition patterns and carbon intelligence.

---

## 🚀 Project Objectives

- Develop an interactive Tableau dashboard for global energy and climate analytics.
- Analyze renewable energy adoption across countries.
- Compare global primary energy consumption and energy mix.
- Study CO₂ emissions and emissions per capita.
- Analyze the relationship between renewable adoption and carbon emissions.
- Compare carbon intensity across countries.
- Visualize historical contributions to global warming.
- Enable interactive exploration through filters and dashboard navigation.

---

# 📊 Dashboards

The project consists of two connected dashboards.

## 1️⃣ Global Energy Transition Dashboard

Focuses on the current global energy landscape and renewable transition.

### Key Areas

- Global energy consumption
- Renewable energy adoption
- Country-level comparisons
- Top energy consumers
- Renewable energy leaders
- Global energy mix
- Energy transition trends

### Interactive Features

- Year filtering
- Country selection
- Cross-chart interactions
- Dynamic KPI updates
- Dashboard navigation

---

## 2️⃣ Climate Impact & Carbon Intelligence

Focuses on the environmental impact associated with global energy systems.

### Key Areas

- Renewable energy share vs CO₂ emissions per capita
- Top CO₂ emitting countries
- Carbon intensity of electricity
- Greenhouse gas emissions
- Historical contributions to global warming

### Analytical Highlight

The dashboard includes a scatter plot exploring the relationship between renewable energy adoption and CO₂ emissions per capita.

- **X-axis:** Renewable Energy Share
- **Y-axis:** CO₂ Emissions per Capita
- **Bubble Size:** Population
- **Bubble Color:** Renewable Energy Category
- **Detail:** Country

Countries are categorized based on renewable energy share:

| Category | Renewable Energy Share |
|----------|------------------------|
| 🟢 High | Greater than 65% |
| 🟡 Medium | Greater than 40% and up to 65% |
| 🔴 Low | 40% or below |

---

# 🗂️ Dataset

## Source

**Our World in Data (OWID)**

The project uses international energy and climate datasets covering approximately:

- 🌍 **220 countries and territories**
- 📅 **25 years (2000–2024)**
- 📊 Multiple energy and climate indicators

### Data Categories

The integrated dataset includes indicators related to:

- Primary energy consumption
- Electricity generation and consumption
- Renewable energy share
- Fossil fuel share
- CO₂ emissions
- CO₂ emissions per capita
- Greenhouse gas emissions
- Carbon intensity of electricity
- Population
- Historical contribution to temperature change

### Integration Keys

The datasets were integrated primarily using:

- `Country / Entity`
- `Year`
- ISO country codes where applicable

---

# 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| Tableau Public | Interactive dashboard development |
| Microsoft Excel | Data cleaning and preparation |
| Our World in Data | Verified energy and climate datasets |
| Business Intelligence | Analytical storytelling and decision support |

---

# 🔄 Data Preparation

The data preparation process included:

1. Selecting relevant OWID datasets and indicators.
2. Removing unnecessary columns.
3. Checking data types and units.
4. Handling missing values where required.
5. Standardizing percentage fields.
6. Integrating datasets using country and year-based keys.
7. Creating calculated fields in Tableau.
8. Validating values to avoid aggregation and unit inconsistencies.

---

# 🧮 Key Calculated Fields

## Renewable Category

Countries are categorized based on renewable energy share:

```tableau
IF [Renewables Share Energy] > 65 THEN "High"
ELSEIF [Renewables Share Energy] > 40 THEN "Medium"
ELSE "Low"
END
```

## Latest Year Indicator

Used to identify the most recent available year dynamically:

```tableau
[Year] = { FIXED : MAX([Year]) }
```

This allows current-state visualizations to automatically reflect the latest available data.

---

# 💡 Key Insights

## ⚡ Energy Transition

- Renewable energy contributes approximately **12.1% of global primary energy consumption**.
- **China** is the world's largest energy consumer.
- **Iceland and Norway** are among the leading countries in renewable energy adoption.
- Fossil fuels continue to dominate the global energy system.

## 🌍 Climate Intelligence

- Higher renewable adoption generally corresponds with lower CO₂ emissions per capita across many countries.
- **China** is the largest current CO₂ emitter.
- The **United States** has the highest historical contribution to global warming.
- Several countries continue to rely on highly carbon-intensive electricity generation.

---

# 🎨 Dashboard Design

The dashboards use a consistent sustainability-focused visual system.

### Color Theme

- 🟢 **Green:** Renewable energy and sustainability
- 🔵 **Blue:** Energy systems and global analytics
- 🟠 **Amber:** Energy transition and intermediate conditions
- 🔴 **Red:** Carbon emissions and climate risk

### Design Principles

- Minimal visual clutter
- Clear visual hierarchy
- Consistent typography
- Interactive exploration
- Analytical storytelling
- Cross-dashboard navigation

---

# 🔗 Interactive Features

The dashboards include:

- Year filters
- Country filters
- Interactive chart selections
- Cross-chart filtering
- Dynamic KPI updates
- Navigation buttons between dashboards
- Detailed tooltips with country-level information

These interactions allow users to move from a global overview toward more detailed country-level exploration.

---

# 🌐 Live Dashboard

The interactive dashboard is published on Tableau Public.

🔗 **Tableau Public Dashboard:**  
[https://public.tableau.com/app/profile/shreya.mishra1905/viz/Global_Energy_Transition_Dashboard/GlobalEnergyTransitionDashboard?publish=yes]

---

# 📸 Dashboard Preview

## Global Energy Transition Dashboard

![Global Energy Transition Dashboard](images/dashboard1.png)

## Climate Impact & Carbon Intelligence

![Climate Impact & Carbon Intelligence](images/dashboard2.png)

---

# 🔮 Future Improvements

Possible future enhancements include:

- Adding more recent energy and climate data.
- Incorporating predictive analytics for future emissions.
- Adding regional-level comparisons.
- Introducing year-over-year change indicators.
- Creating scenario-based renewable energy transition analysis.
- Adding forecasting and machine learning models.
- Expanding the project into a web-based sustainability intelligence platform.

---

# 👩‍💻 Author

**Shreya Mishra**  
B.Tech CSE – Data Science  
Ajay Kumar Garg Engineering College

---

# 📄 Data Source & Attribution

This project uses datasets published by **Our World in Data (OWID)**.

Appropriate dataset attribution and licensing requirements should be retained according to the respective OWID dataset documentation.

---

# ⭐ Project Purpose

This project demonstrates practical skills in:

- Data Cleaning
- Data Integration
- Business Intelligence
- Data Visualization
- Tableau Dashboard Development
- Analytical Storytelling
- Sustainability and Climate Data Analysis

---

⭐ If you found this project interesting, consider giving the repository a star!
