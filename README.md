# Glasgow5GDataset2025

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![Data Date](https://img.shields.io/badge/Date-April%202025-blue.svg)](https://github.com/AhrenHart/Glasgow5GDataset2025)
[![Locations](https://img.shields.io/badge/Locations-16-orange.svg)](https://github.com/AhrenHart/Glasgow5GDataset2025)

A comprehensive dataset capturing real-world 5G network performance across Glasgow, Scotland, collected in April 2025. This includes speed tests from major UK providers in urban and suburban locations, tested on flagship Android devices.

## 📊 Overview
This dataset provides insights into 5G connectivity in Glasgow, focusing on key metrics like download/upload speeds, ping latency, and signal strength. Data was gathered over three consecutive days (April 6–8, 2025) using automated speed tests in 16 diverse neighborhoods. It's ideal for researchers, network engineers, or urban planners studying mobile broadband performance, coverage disparities, or 5G rollout effectiveness.

### Key Highlights
- **Total Tests**: ~1,200+ individual measurements (4 providers × 2 devices × 16 locations × 3 days).
- **Providers**: EE, O2, Vodafone, Sky Mobile.
- **Devices**: Google Pixel 9 Pro, Samsung Galaxy S24 Ultra.
- **Metrics**:
  - Signal Strength (dBm): Lower (more negative) values indicate weaker signal.
  - Download Speed (Mbps): Peak and average throughput.
  - Upload Speed (Mbps): Upstream performance.
  - Ping (ms): Latency for real-time applications.
- **Overall Averages** (across all data):
  - Download: 670.63 Mbps
  - Upload: 165.05 Mbps
  - Ping: 21.62 ms
  - Signal: -77.85 dBm

## 🗺️ Locations Covered
Tests were conducted in a mix of central, residential, and peripheral areas to represent Glasgow's urban fabric.

| Location          | Download Mean (Mbps) | Upload Mean (Mbps) | Ping Mean (ms) | Signal Mean (dBm) |
|-------------------|----------------------|--------------------|----------------|-------------------|
| Bearsden         | 633.88              | 161.43            | 20.62         | -77.62           |
| Cathcart         | 681.34              | 164.10            | 20.79         | -77.81           |
| Dennistoun       | 648.51              | 156.63            | 23.87         | -77.06           |
| Drumchapel       | 682.05              | 154.82            | 22.47         | -78.31           |
| Easterhouse      | 707.79              | 173.77            | 21.88         | -77.94           |
| Glasgow City Centre | 638.76           | 174.35            | 20.99         | -76.31           |
| Govan            | 704.00              | 166.20            | 21.95         | -79.38           |
| Govanhill        | 680.19              | 161.16            | 22.28         | -78.44           |
| Hillhead         | 600.23              | 157.31            | 22.44         | -78.00           |
| Maryhill         | 631.37              | 171.87            | 20.53         | -76.75           |
| Merchant City    | 688.23              | 156.06            | 21.19         | -78.62           |
| Partick          | 677.89              | 165.23            | 19.73         | -77.88           |
| Pollok           | 699.40              | 176.15            | 22.42         | -77.62           |
| Shawlands        | 684.28              | 180.90            | 21.16         | -77.88           |
| Springburn       | 701.56              | 155.71            | 21.99         | -78.19           |

*Glasgow-wide average*: 670.63 Mbps download, 165.05 Mbps upload, 21.62 ms ping, -77.85 dBm signal.

## 📈 Provider Performance
Averages by network provider, highlighting strengths in speed vs. consistency.

| Provider     | Download Mean (Mbps) | Upload Mean (Mbps) | Ping Mean (ms) | Signal Mean (dBm) |
|--------------|----------------------|--------------------|----------------|-------------------|
| EE          | 660.72              | 168.65            | 21.96         | -78.07           |
| O2          | 695.38              | 167.61            | 22.13         | -78.51           |
| Sky Mobile  | 668.58              | 165.26            | 21.21         | -77.13           |
| Vodafone    | 657.86              | 158.66            | 21.18         | -77.71           |

### Day-by-Day Trends
| Date       | Download Mean (Mbps) | Upload Mean (Mbps) | Ping Mean (ms) | Signal Mean (dBm) |
|------------|----------------------|--------------------|----------------|-------------------|
| 2025-04-06 | 694.18              | 163.45            | 21.36         | -78.39           |
| 2025-04-07 | 680.77              | 162.88            | 21.64         | -77.56           |
| 2025-04-08 | 636.94              | 168.81            | 21.87         | -77.61           |

## 📁 Dataset Structure
The repository includes:
- **`Glasgow5GDataSet.xlsx`**: Raw data in Excel format.
  - **Sheets 0–2**: Daily raw measurements (timestamps as Excel serial dates; convert via `pd.to_datetime` in Python).
  - **Sheet 3**: Pre-computed averages (locations, providers, days).

### Sample Data Row
| Timestamp          | Location          | Provider | Device                | Signal (dBm) | Download (Mbps) | Upload (Mbps) | Ping (ms) |
|--------------------|-------------------|----------|-----------------------|--------------|-----------------|---------------|-----------|
| 2025-04-06 08:30  | Glasgow City Centre | EE      | Google Pixel 9 Pro   | -86         | 907.32         | 192.95       | 29.75    |

## 🔧 Usage
### Loading the Data
```python
import pandas as pd

# Load raw sheet (e.g., April 6)
df = pd.read_excel('Glasgow5GDataSet.xlsx', sheet_name=0)

# Convert timestamp
df['Timestamp'] = pd.to_datetime(df['Timestamp'], unit='D', origin='1899-12-30')
```python

##🤝 Contributing

Fork the repo and submit a PR for additions (e.g., more dates, analysis scripts).
Report issues for data anomalies or suggestions.
Cite this dataset in your work: @misc{glasgow5g2025, author = {Hart, Ahren}, title = {Glasgow 5G Performance Dataset}, year = {2025}, url = {https://github.com/AhrenHart/Glasgow5GDataset2025} }

# Basic stats
print(df.groupby('Network Provider')['Download Speed (Mbps)'].mean())

##📄 License
License: CC BY 4.0
This dataset is licensed under the Creative Commons Attribution 4.0 International License.
You are free to:

Share — copy and redistribute the material in any medium or format
Adapt — remix, transform, and build upon the material for any purpose, including commercially

Under the following terms:

Attribution — You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.

Suggested Citation:
Hart, A. (2025). Glasgow 5G Performance Dataset [Data set]. University of the West of Scotland, Paisley, UK. https://github.com/AhrenHart/Glasgow5GDataset2025
For questions, contact Ahren Hart at Ahren.hart@uws.ac.uk.
