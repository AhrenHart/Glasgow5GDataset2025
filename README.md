# Glasgow5GDataset2025

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg)](LICENSE.md)
[![Data Date](https://img.shields.io/badge/Date-April%202025-blue.svg)](https://github.com/AhrenHart/Glasgow5GDataset2025)
[![Locations](https://img.shields.io/badge/Locations-15-orange.svg)](https://github.com/AhrenHart/Glasgow5GDataset2025)

A comprehensive dataset capturing real-world 5G network performance across Glasgow, Scotland, collected in April 2025. This includes speed tests from major UK providers in urban and suburban locations, tested on flagship Android devices.

## 📊 Overview
This dataset provides insights into 5G connectivity in Glasgow, focusing on key metrics like download/upload speeds, ping latency, and signal strength. Data was gathered over three consecutive days (April 6–8, 2025) using automated speed tests in 15 diverse neighborhoods. It's ideal for researchers, network engineers, or urban planners studying mobile broadband performance, coverage disparities, or 5G rollout effectiveness.

### Key Highlights
- **Total Tests**: ~1,200+ individual measurements (4 providers × 2 devices × 15 locations × 3 days).
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
 
**Download Speed Distribution per Network Provider**
<img width="2970" height="1765" alt="download_speed_distribution" src="https://github.com/user-attachments/assets/17b71fda-9a8d-4eae-a9cf-64333d796cb5" />
Box plot showing download speed distributions (Mbps) across providers. EE and Vodafone show higher variability, while O2 and Sky Mobile are more consistent.

**Signal Strength by Provider**
<img width="2970" height="1765" alt="signal_strength_by_provider" src="https://github.com/user-attachments/assets/2ad6c60c-cd94-4a0f-9554-29a0f43955b8" />
Box plot of signal strength (dBm; lower = stronger). Sky Mobile exhibits the strongest average signal, followed closely by Vodafone.

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

**5G Average Download Speeds Across Glasgow**
<img width="1536" height="754" alt="HeatMap2" src="https://github.com/user-attachments/assets/41dd5a89-dc23-43f8-aca4-042996d88579" />
Choropleth map of average 5G download speeds (Mbps) across Glasgow neighborhoods. Warmer colors indicate higher speeds.

**Average Upload Speed by Area**
<img width="2969" height="1765" alt="avg_upload_by_area" src="https://github.com/user-attachments/assets/26f431f9-ca39-4bcb-8243-1f213e7396a2" />
Bar chart of average upload speeds (Mbps) across Glasgow neighborhoods. Shawlands and Pollok lead in upload performance.

**Average Ping by Area**
<img width="2969" height="1765" alt="avg_ping_by_area" src="https://github.com/user-attachments/assets/a9c5f432-7cc4-46d2-aa54-9cb68b818a24" />
Bar chart of average ping latency (ms). Partick and Maryhill show the lowest (best) latency, ideal for gaming or video calls.

**Average Download Speed by Area**
<img width="2969" height="1765" alt="avg_download_by_area" src="https://github.com/user-attachments/assets/fa23dda5-6bc6-42f9-a06e-ba3c904444dd" />
Bar chart of average download speeds (Mbps). Easterhouse and Govan top the list for peak throughput.

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

**Avg Download Speed: Area vs Network Provider**
<img width="3392" height="2365" alt="avg_download_heatmap" src="https://github.com/user-attachments/assets/d6297677-2806-42b6-91b5-6e4f3a569a13" />
Heatmap of average download speeds (Mbps) by location and provider. O2 shines in central areas like Glasgow City Centre, while EE dominates in suburbs like Cathcart.

## 📁 Dataset Structure
The repository includes:
- **`Glasgow5GDataSet.xlsx`**: Processed and compiled raw data in Excel format for easy reading and use.
  - **Sheets 0–2**: Daily raw measurements (timestamps as Excel serial dates; convert via `pd.to_datetime` in Python).
  - **Sheet 3**: Pre-computed averages (locations, providers, days).

### Sample Data Row
| Timestamp          | Location          | Provider | Device                | Signal (dBm) | Download (Mbps) | Upload (Mbps) | Ping (ms) |
|--------------------|-------------------|----------|-----------------------|--------------|-----------------|---------------|-----------|
| 2025-04-06 08:30  | Glasgow City Centre | EE      | Google Pixel 9 Pro   | -86         | 907.32         | 192.95       | 29.75    |

## 🤝 Contributing

* Fork the repo and submit a PR for additions (e.g., more dates, analysis scripts).

* Report issues for data anomalies or suggestions.

* Cite this dataset in your work: @misc{glasgow5g2025, author = {Hart, Ahren}, title = {Glasgow 5G Performance Dataset}, year = {2025}, url = {https://github.com/AhrenHart/Glasgow5GDataset2025} }

## 📄 License
License: CC BY 4.0  
This dataset is licensed under the [Creative Commons Attribution 4.0 International License](LICENSE.md).  

You are free to:  
* Share — copy and redistribute the material in any medium or format  
* Adapt — remix, transform, and build upon the material for any purpose, including commercially  

Under the following terms:  
* Attribution — You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.  

Suggested Citation: Hart, A. (2025). Glasgow 5G Performance Dataset [Data set]. University of the West of Scotland, Paisley, UK. https://github.com/AhrenHart/Glasgow5GDataset2025  
For questions, contact Ahren Hart at Ahren.hart@uws.ac.uk.

## 👤 Author
Ahren Hart – Researcher at University of the West of Scotland, focused on Holographic Communication Networks Enhanced By 5G/6G Networks and AI. 
Collected with open-source tools like Speedtest CLI. All data is anonymized and for public research use.2.8s

