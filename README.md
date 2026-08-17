# 🌊 Interactive Ocean Microbiome Data Visualization Dashboard

An interactive data visualization project for exploring **ocean microbiome abundance, geographic distribution, temporal patterns, sampling depth, and uncertainty** across marine environments.

The dashboard combines multiple coordinated visualizations built with **Python, Pandas, Altair, Vega/Vega-Lite, and Jupyter Notebook**, enabling users to explore complex ocean microbiome datasets through interactive filtering, geographic mapping, statistical summaries, and uncertainty-aware visual analysis.

---

## 📌 Project Overview

Ocean microbiome datasets contain complex relationships across microbial taxonomy, geographic sampling locations, sampling depth, time, and abundance.

This project transforms those multidimensional datasets into an **interactive visual analytics dashboard** designed to make those relationships easier to explore and interpret.

The system provides multiple coordinated views so that users can investigate questions such as:

* How does microbial abundance vary geographically?
* Which microbial classes are most abundant?
* How does microbial abundance change across different years?
* Is microbial abundance related to sampling depth?
* Which ocean regions contain higher concentrations of particular microbial groups?
* How much variability or uncertainty exists within the observations?

Rather than relying on a single chart, the project combines several complementary visualizations that provide both a **high-level overview** and the ability to investigate individual observations.

---

## 🎯 Objectives

The main objectives of the project were to:

* Build an interactive dashboard for exploring ocean microbiome data.
* Visualize geographic distributions of microbial populations.
* Analyse microbial abundance across taxonomic classes and ocean regions.
* Investigate temporal trends in microbial abundance.
* Explore relationships between sampling depth and abundance.
* Represent uncertainty and variability within the data.
* Provide coordinated filtering across multiple visualizations.
* Apply visualization design principles to improve clarity and interpretability.
* Support both overview-level exploration and detailed investigation.

---

## ✨ Key Features

### 🗺️ Interactive Geographic Map

The geographic visualization displays microbiome sampling locations across the world's oceans.

Users can explore:

* sampling coordinates,
* microbial abundance,
* microbial classes,
* geographic distribution patterns,
* and selected temporal subsets.

The map provides geographic context that makes it easier to identify spatial patterns in microbiome observations.

---

### 📊 Microbial Abundance Bar Chart

The bar chart provides a comparative view of microbial abundance across categories.

It enables users to quickly identify:

* highly abundant microbial groups,
* differences between categories,
* dominant classes,
* and patterns within filtered subsets.

---

### 🥧 Microbial Distribution Pie Chart

The pie chart provides a proportional representation of microbial classes.

It gives users a quick overview of the relative contribution of different microbial groups within the selected data.

---

### 📈 Temporal Trend Analysis

The line chart visualizes changes in microbial abundance over time.

This helps users investigate:

* temporal patterns,
* changes between sampling years,
* long-term abundance trends,
* and possible fluctuations within microbial populations.

---

### 🔬 Sampling Depth vs Microbial Abundance

The scatter plot explores the relationship between **sampling depth** and **microbial abundance**.

Individual observations can be inspected interactively, allowing users to identify:

* possible correlations,
* clusters,
* unusual observations,
* depth-dependent patterns,
* and variability within microbial measurements.

---

### 🌡️ Uncertainty Visualization

Environmental and biological datasets naturally contain uncertainty arising from sampling methods, environmental variability, measurement error, and incomplete observations.

This project incorporates uncertainty into the visual analysis through techniques including:

* error bars,
* standard deviation,
* variability measures,
* heatmaps,
* color gradients,
* and interactive contextual information.

These visual elements help users distinguish between stable trends and observations that may require more cautious interpretation.

---

### 🔄 Multiple Coordinated Views

One of the core features of the project is the use of **multiple coordinated visualizations**.

The dashboard combines:

* geographic maps,
* bar charts,
* pie charts,
* scatter plots,
* line charts,
* legends,
* dropdown filters,
* and uncertainty visualizations.

These complementary views allow users to analyse the same dataset from several perspectives.

---

### 🎛️ Interactive Filtering

Interactive controls enable users to narrow the dataset according to their analytical interests.

Filters include dimensions such as:

* microbial class,
* sampling year,
* and visualization selections.

Filtering helps users move from a high-level overview to focused investigation of particular subsets.

---

### 💬 Interactive Tooltips

Hover-based tooltips provide contextual information without overcrowding the visualizations.

Depending on the chart, users can inspect information such as:

* microbial class,
* abundance,
* sampling depth,
* geographic location,
* year,
* and individual observation values.

---

## 🧠 Visualization Design Principles

The dashboard was designed using established information visualization principles.

### Gestalt Principles

The interface applies concepts such as:

* **Proximity** — related visual elements are positioned together.
* **Similarity** — consistent visual encoding helps users recognise related categories.
* **Continuity** — charts and dashboard components are arranged to support natural visual exploration.

### Consistent Visual Encoding

Microbial classes are represented consistently across coordinated visualizations, helping users maintain context while moving between different charts.

### Overview + Detail

The dashboard supports both:

* high-level exploration through aggregated charts and maps,
* and detailed inspection through filtering, selections, and tooltips.

### Accessible Colour Schemes

Colour palettes such as **Viridis** and categorical schemes are used to improve readability and support interpretation across a range of users.

---

## 🛠️ Technology Stack

| Technology           | Purpose                                                      |
| -------------------- | ------------------------------------------------------------ |
| **Python**           | Data processing and visualization development                |
| **Pandas**           | Data cleaning, transformation, aggregation and analysis      |
| **NumPy**            | Numerical and statistical processing                         |
| **Altair**           | Declarative interactive data visualizations                  |
| **Vega / Vega-Lite** | Rendering interactive visualization specifications           |
| **Vega Datasets**    | Geographic visualization data                                |
| **Jupyter Notebook** | Interactive development and data analysis                    |
| **HTML**             | Exported interactive dashboard and individual visualizations |
| **CSV**              | Ocean microbiome datasets                                    |

---

## 📂 Repository Structure

```text
ocean-microbiome-data-visualization/
│
├── visualization.ipynb
│
├── dashboard.html
├── map_chart.html
├── bar_chart.html
├── scatter_chart.html
├── line_chart.html
├── pie_chart.html
├── legend.html
├── year_dropdown.html
│
├── Tara_Cleaned_Data.csv
├── Tara_GenusTableTax_80CAb.csv
├── Tara_OTUtableTax_80CAb.csv
├── Tara_OTUtableTax_Full.csv
├── Tara_OTUtable_80CAb_transp.csv
├── Tara_SampleMeta.csv
│
├── .gitignore
└── README.md
```

---

## 📊 Dataset

The project uses ocean microbiome data associated with the **Tara Oceans** research domain.

The repository contains several datasets representing microbial taxonomy, operational taxonomic units, sample metadata, and cleaned data used by the visualization workflow.

### Main Dataset Files

#### `Tara_Cleaned_Data.csv`

Processed dataset used for visualization and analysis.

#### `Tara_SampleMeta.csv`

Contains metadata associated with ocean sampling locations and observations.

#### `Tara_GenusTableTax_80CAb.csv`

Contains genus-level taxonomic information.

#### `Tara_OTUtableTax_80CAb.csv`

Contains taxonomic information associated with operational taxonomic units.

#### `Tara_OTUtableTax_Full.csv`

Contains the larger OTU taxonomy dataset used during analysis.

#### `Tara_OTUtable_80CAb_transp.csv`

Contains transformed OTU abundance information used during preprocessing and analysis.

---

## 🔄 Data Analysis Workflow

The project follows a general analytical pipeline:

```text
Raw Ocean Microbiome Data
          │
          ▼
   Data Preprocessing
          │
          ▼
 Cleaning & Transformation
          │
          ▼
 Statistical Aggregation
          │
          ▼
 Interactive Visualization
          │
          ▼
 Coordinated Dashboard
          │
          ▼
 Exploration & Interpretation
```

The data preparation process includes operations such as:

* loading CSV datasets,
* cleaning records,
* handling missing values,
* transforming data structures,
* aggregating abundance measurements,
* calculating statistical measures,
* joining sample metadata,
* and preparing visualization-specific datasets.

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/Karthikeyan010/ocean-microbiome-data-visualization.git
```

Move into the project directory:

```bash
cd ocean-microbiome-data-visualization
```

---

## 🐍 Create a Python Virtual Environment

### Windows

```bash
python -m venv .venv
```

Activate it:

```bash
.venv\Scripts\activate
```

### macOS / Linux

```bash
python3 -m venv .venv
```

Activate it:

```bash
source .venv/bin/activate
```

---

## 📦 Install Dependencies

Install the main Python libraries:

```bash
pip install pandas numpy altair vega_datasets jupyter
```

Depending on your Jupyter environment, you may also use:

```bash
pip install notebook
```

---

## ▶️ Run the Project

Start Jupyter Notebook:

```bash
jupyter notebook
```

Then open:

```text
visualization.ipynb
```

Run the notebook cells sequentially to:

1. load the datasets,
2. preprocess the microbiome data,
3. generate the visualizations,
4. construct the coordinated dashboard,
5. export the resulting HTML visualizations.

---

## 🌐 View the Interactive Dashboard

The generated dashboard is available as:

```text
dashboard.html
```

Open it locally using a web browser.

You can also inspect individual visualization outputs:

```text
map_chart.html
bar_chart.html
scatter_chart.html
line_chart.html
pie_chart.html
legend.html
year_dropdown.html
```

These files contain interactive Vega/Vega-Lite visualizations exported from the Python workflow.

---

## 🔍 Example Analytical Questions

The dashboard can be used to explore questions including:

### Geographic Analysis

> How does microbial abundance vary across different ocean regions?

### Taxonomic Analysis

> Which microbial classes dominate particular samples or regions?

### Temporal Analysis

> How does microbial abundance change between sampling years?

### Depth Analysis

> Is there a relationship between sampling depth and microbial abundance?

### Uncertainty Analysis

> Which observations demonstrate greater variability or uncertainty?

These questions demonstrate how coordinated visual analytics can support exploratory investigation of multidimensional environmental datasets.

---

## ⚠️ Sources of Data Uncertainty

Several factors can introduce uncertainty into ocean microbiome analysis.

### Sampling Methodology

Differences in sampling depth, equipment, calibration, and collection methods can influence recorded abundance.

### Temporal Variability

Microbial populations can change because of seasonal conditions, ocean currents, ecological events, and other environmental processes.

### Geographic Coverage

Uneven sampling coverage may result in some regions being represented more heavily than others.

### Measurement Error

Sensors and laboratory instruments may introduce measurement inaccuracies.

### Data Processing

Cleaning, aggregation, transformation, and missing-value handling can influence downstream interpretation.

### Environmental Complexity

Factors such as nutrient availability, salinity, temperature, and interactions between marine organisms may affect microbial populations.

### Outliers

Anomalous observations may result from either genuine environmental conditions or measurement issues.

The visualization therefore aims not only to show patterns, but also to communicate variability where possible.

---

## 🎨 Visualization Design

The dashboard combines several visualization types because each addresses a different analytical task.

| Visualization          | Analytical Purpose                         |
| ---------------------- | ------------------------------------------ |
| **Map**                | Geographic distribution                    |
| **Bar Chart**          | Category comparison                        |
| **Pie Chart**          | Relative distribution                      |
| **Scatter Plot**       | Relationships between continuous variables |
| **Line Chart**         | Temporal trends                            |
| **Heatmap**            | Patterns, density and variability          |
| **Error Bars**         | Statistical uncertainty                    |
| **Interactive Legend** | Category identification and exploration    |
| **Dropdown Filters**   | Focused subset analysis                    |

Together, these components create a **multiple coordinated views** environment for exploratory data analysis.

---

## 💡 Potential Future Improvements

The project could be extended with several features.

### Search and Query Interface

Allow users to search directly for ocean regions, microbial classes, or specific analytical questions.

### Summary Statistics

Add dashboard cards displaying:

* total observations,
* mean abundance,
* dominant microbial class,
* number of sampling regions,
* and average sampling depth.

### Confidence Intervals

Add shaded uncertainty bands to temporal visualizations.

### Improved Data Quality Indicators

Explicitly highlight incomplete, missing, or potentially unreliable observations.

### Storytelling Mode

Provide a guided analytical workflow that walks users through important findings.

### Hierarchical Visualization

Introduce tree maps or hierarchical charts for exploring microbial taxonomy.

### Web Deployment

Deploy the dashboard as an interactive web application using technologies such as:

* Streamlit,
* Dash,
* Flask,
* or a static GitHub Pages deployment.

---

## 📚 References & Resources

The project was informed by resources covering data visualization, scientific computing, ocean microbiome research, and uncertainty visualization.

* Altair Visualization Library — declarative statistical visualization for Python
* Vega and Vega-Lite — grammar-based interactive visualization
* Pandas — data manipulation and preprocessing
* NumPy — numerical computing
* Tara Oceans / Ocean Microbiome datasets
* Wall, E., Blaha, L. M., & Bertini, E. — research on heuristics for evaluating uncertainty in data visualizations
* VanderPlas, J. — *Python Data Science Handbook*
* Steele, J. & Iliinsky, N. — *Designing Data Visualizations*

---

## 🎓 Academic Context

This project was originally developed as part of **CSC8636 – Complex Data Visualization** at **Newcastle University**.

The repository has been organised as a portfolio project to demonstrate practical skills in:

* data visualization,
* exploratory data analysis,
* Python development,
* interactive dashboard design,
* multidimensional data analysis,
* data preprocessing,
* uncertainty visualization,
* and visual analytics.

---

## 👨‍💻 Author

**Karthikeyan Karuppaiah**

MSc Advanced Computer Science
Newcastle University, United Kingdom

GitHub: [@Karthikeyan010](https://github.com/Karthikeyan010)

---

## ⭐ Project Highlights

This project demonstrates practical experience with:

* **Python-based data analytics**
* **Pandas and NumPy data processing**
* **Interactive Altair visualizations**
* **Vega/Vega-Lite**
* **Multiple coordinated views**
* **Geospatial data visualization**
* **Temporal data analysis**
* **Multidimensional environmental datasets**
* **Interactive filtering and tooltips**
* **Statistical uncertainty visualization**
* **Scientific data communication**
* **Dashboard design**

---

If you find the project useful or interesting, feel free to explore the repository and the interactive visualizations.
