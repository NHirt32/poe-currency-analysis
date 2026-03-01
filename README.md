# Path of Exile Currency & Market Analysis Tool

## Project Overview
This repository contains a Jupyter Notebook designed to interface with the PoE Ninja API to retrieve, document, and analyze real-time currency market data within Path of Exile. While the tool provides financial insights, its primary technical purpose is to perform API discovery and validate the consistency of dynamic data returns in a high-frequency environment.

## Key Features
* **Automated Data Retrieval:** Interfaces with the PoE Ninja API to pull live currency exchange rates and historical price trends.
* **API Schema Documentation:** Maps and documents unique API return structures to ensure data ingestion remains stable across game expansions and API updates.
* **Statistical Validation:** Implements statistical models to identify "outlier" data points—isolating instances of market manipulation, API lag, or corrupted data entries.
* **Dynamic Visualizations:** Utilizes Matplotlib and Seaborn to transform raw JSON responses into readable trend analyses, facilitating better communication of economic "health" metrics.

## Technical Stack
* **Language:** Python
* **Environment:** Jupyter Notebook
* **Libraries:** Pandas, Requests, Matplotlib, Seaborn, NumPy

## Configuration
The notebook is currently configured to analyze the **Keepers** league by default. To analyze a different league (e.g., Standard, Hardcore, or a new Challenge League):

1. Locate the `league` string variable in the first configuration cell.
2. Update the string to the desired league name exactly as it appears on the official PoE trade site or API documentation.
3. Re-run the data ingestion cells to fetch the updated dataset.

## How to Use
1. **Clone the repository**
2. **Install dependencies**
3. **Configure League:** Ensure the league string matches your target analysis (see Configuration above).
4. **Execute:** Run the `currency-analysis.ipynb` notebook to generate real-time visualizations.
