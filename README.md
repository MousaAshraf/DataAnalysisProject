# Economic Growth Prediction: Nighttime Lights and Internet Speeds

## Objective
This project aims to predict economic development by analyzing changes in nighttime lights (VIIRS data) and internet speeds (Ookla Speedtest data). The focus is on understanding the interplay between digital infrastructure and economic activity, with a specific analysis conducted on Egypt, Libya, and Palestine for the year 2021 (Q1 to Q4).

---

## Datasets
### 1. **Ookla Speedtest Data**
   - **Metrics**: Download/upload speeds, latency, and test counts.
   - **Spatial Coverage**: Global, with ~610.8m × 610.8m tiles.
   - **Temporal Coverage**: Quarterly data for 2021 (Q1 to Q4).

### 2. **VIIRS Annual Composites**
   - **Metrics**: Radiance values indicating human activity and economic infrastructure.
   - **Spatial Coverage**: Global, with ~500m resolution.
   - **Temporal Coverage**: Annual data for 2021.

---

## Procedural Details
### Data Preprocessing
1. **VIIRS Data**:
   - Extracted annual radiance data for 2021 at regional or national levels.
   - Calculated percentage changes in radiance over time to represent economic growth.

2. **Ookla Data**:
   - Aggregated quarterly internet speed data for 2021 (Q1 to Q4) into annual averages to align with VIIRS temporal granularity.
   - Focused on download speeds as a key indicator of internet infrastructure performance.

3. **Integration**:
   - Performed spatial joins to align Ookla tiles with VIIRS grids or administrative boundaries (e.g., countries or regions).
   - Created a unified dataset that includes radiance changes, internet speeds, and economic indicators (e.g., GDP growth, if available).

---

## Exploratory Data Analysis (EDA) and Visualizations
1. **Heatmap**:
   - Visualized regional variations in radiance intensity and internet speeds.

2. **Scatter Plot**:
   - Correlated changes in radiance with internet speeds to identify trends.

3. **Bar Chart**:
   - Compared regions with different levels of radiance growth and internet performance.

4. **Geospatial Overlay**:
   - Mapped regions with high radiance growth and fast internet speeds to highlight economic hotspots.

5. **Line Chart**:
   - Displayed time-series trends in radiance and internet speeds for key regions.

6. **Pie Chart**:
   - Visualized the distribution of radiance intensity or internet speed performance across regions (e.g., Egypt, Libya, Palestine).

7. **Donut Pie Chart**:
   - Enhanced the pie chart by adding a central hole to display additional metrics (e.g., percentage of total economic activity or internet usage).

---

## Hypothesis Testing
- **Null Hypothesis**: Changes in nighttime light intensity and internet speeds are not significantly associated with economic development.
- **Alternative Hypothesis**: Changes in nighttime light intensity and internet speeds are significantly associated with economic development.

---

## Prediction Model Objective
- **Objective**: Predict regional economic growth (e.g., GDP growth) using changes in nighttime light intensity and internet speeds as predictors.

---

## Analysis on Egypt, Libya, and Palestine
- Conducted a detailed analysis of the year 2021 (Q1 to Q4) for Egypt, Libya, and Palestine.
- Explored trends in radiance and internet speeds to understand their relationship with economic activity in these regions.
- Included **pie charts** and **donut pie charts** to visualize the distribution of key metrics (e.g., radiance intensity, internet speeds) across these regions.

---

## How to Use
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/economic-growth-prediction.git
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Run the Jupyter notebooks in the `/notebooks` folder to reproduce the analysis.

---

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgments
- **Ookla** for providing global internet speed data.
- **VIIRS** for nighttime light radiance data.
- Open-source tools and libraries used in this project.
