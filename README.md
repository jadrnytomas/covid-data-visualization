
# COVID-19 Data Analysis & Interactive Dashboards (Python, Plotly & Dash)

This project focuses on visualizing global COVID-19 pandemic data using Python's scientific and interactive visualization libraries, specifically **Seaborn**, **Plotly**, and **Dash**. This project was done for my Data Analyst course.

## 📋 Project Overview
- **Problem Statement:** Analyze the global development, impact, and vaccination rates of the COVID-19 pandemic using data-driven insights.
- **Data Source:** Sourced from the GitHub of *Our World In Data*, modified to include simplified columns and geographical coordinates (`latitude`, `longitude`).
- **Environment:** Google Colab / Python Jupyter Notebooks.
- **Key Technologies:** `pandas`, `seaborn`, `matplotlib`, `plotly.express`, `dash`, and `threading`.

---

## 📊 Features & Task Breakdown

### 1. Country Population Ranking (Seaborn)
- **Task:** Generate a ranking of the top 10 most populated countries in the dataset.
- **Highlights:** Styled using `whitegrid` with an adjusted figure size and rotated X-axis tick labels to prevent overlapping.
- **Key Insight:** Easily contrast the massive demographic sizes of countries like China and India against the remaining top countries.

### 2. Population vs. Life Expectancy Correlation (Plotly)
- **Task:** Interactive scatter plot evaluating the relationship between a country's population size and life expectancy.
- **Highlights:** Features a logarithmic X-axis for population, customized trace color mapping via `continent_colors`, and interactive dropdown filters by continent.
- **Key Insight:** A larger population does not correlate with longer life expectancy; however, regional trends (such as lower average life expectancies in Africa) are visible.

### 3. COVID-19 Timeline Comparison (Plotly)
- **Task:** A timeline comparison showing the distribution of daily new COVID-19 cases over time for chosen countries (**Czechia** and **Slovakia**).
- **Highlights:** Dynamic line charts with formatted dates and hover menus.

### 4. Global COVID-19 Map (Plotly Mapbox)
- **Task:** Display cumulative global cases represented dynamically as markers on a global dark-themed map projection.
- **Highlights:** Marker sizes scale according to the total cases, color-coded by continent, with a custom hover tooltip using `carto-darkmatter` style.

### 5. Dashboard 1: Country-Level Trend Explorer (Dash)
- **Task:** Dynamic interactive side-by-side dashboard containing line charts representing cumulative cases and cumulative deaths.
- **Highlights:**
  - Interactive country-selector dropdown menu.
  - The main page title adapts dynamically to the selected country.
  - Runs inside Colab environment on port `8050` using thread execution.

### 6. Dashboard 2: Regional Metrics Map Viewer (Dash)
- **Task:** An interactive Mapbox scatter map showcasing various selectable metrics from the pandemic's last recorded day.
- **Highlights:**
  - Interactive continent selection filter.
  - Metric selection dropdown (`Total cases`, `Total deaths`, `Total tests`, `Total vaccinations`, `People vaccinated`).
  - Displays coordinates and values cleanly on hover. Running on port `8051`.

### 7. Dashboard 3: Global Vaccination Analysis (Dash)
- **Task:** Interactive column charts showing absolute total vaccinations vs. population vaccination ratio.
- **Highlights:**
  - Slider allowing users to change the number of displayed countries ($n$) between $5$ and $20$.
  - Displays both absolute numbers and population ratios side-by-side. Running on port `8052`.

---

## 🛠️ How to Run locally

1. **Open the nothebook in Google Colab**
2. **Upload the project_1_pythong.csv dataset into the Colab working environmnet files**
3. **Run the Notebook:**
   Run all cells sequentially to spin up local Dash servers on ports `8050`, `8051`, and `8052` respectively.
