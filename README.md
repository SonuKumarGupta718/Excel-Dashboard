# Re-create the README.md file after code execution environment reset

readme_content = """
# 🌍 Air Pollution Analysis Dashboard

An interactive Excel dashboard created using pivot tables, slicers, and visual charts to analyze and compare pollution data across different cities, states, and monitoring stations.

---

## 📁 Dataset Overview

The dataset contains pollution monitoring data with the following key fields:

- `country`, `state`, `city`, `station`: Location information
- `pollutant_id`: Type of pollutant (e.g., PM10, NO2, CO)
- `pollutant_min`, `pollutant_max`, `pollutant_avg`: Pollution readings
- `latitude`, `longitude`: Geographic coordinates
- `last_update`: Date/time of the data capture

---

## 📊 Pivot Tables Included

| # | Pivot Table Description | Chart Type | Slicers Used |
|---|--------------------------|------------|---------------|
| 1 | Average Pollutant by State | Clustered Bar Chart | `pollutant_id`, `city` |
| 2 | Max Pollutant by Station | Stacked Column Chart | `state`, `pollutant_id`, `last_update` |
| 3 | Min Pollutant by City | Stacked Bar Chart | `state`, `pollutant_id`, `station`, `last_update` |
| 4 | Pollutant Trend Over Time | Line Chart | `pollutant_id`, `state` |
| 5 | Pollutant Distribution by Country | 100% Stacked Column Chart | `pollutant_id`, `last_update` |
| 6 | Pollution by Latitude | Filled Map / Scatter Plot | `pollutant_id`, `state`, `last_update` |
| 7 | Monitoring Stations Count per State | Column Chart | `state` |
| 8 | Overall Pollution Comparison | Combo Chart / Radar Chart | `state`, `city`, `last_update` |

---

## 🧩 Interactivity

The dashboard is enhanced with slicers for:
- Pollutant type (`pollutant_id`)
- State and City filters
- Monitoring Station selection
- Time-based filtering (`last_update`)

All slicers are linked across pivot tables for seamless, responsive filtering.

---

## 📌 Requirements

- Microsoft Excel 2016 or later (for Pivot Charts, Slicers & Maps)

---

## 🧠 Insights You Can Gain

- Which state or city has the highest or lowest pollution levels
- Time trends of specific pollutants
- Comparative analysis between different regions or stations
- Identification of pollution hotspots

---

## 🛠️ How to Use

1. Open the `Dashboard.xlsx` file.
2. Use slicers at the top/side to filter data.
3. Hover over charts for exact values.
4. Explore all pivot tables for detailed insights.

---

## 📜 License

This project is open-source and free to use under the MIT License.

---

## 🤝 Contributing

Feel free to fork this project, improve it, or expand it with other datasets like AQI levels, weather conditions, etc.

---

## 📬 Contact

For suggestions, feel free to reach out via GitHub issues or open a pull request.
"""

# Save the README to a file
readme_path = "/mnt/data/README.md"
with open(readme_path, "w") as file:
    file.write(readme_content)

readme_path

