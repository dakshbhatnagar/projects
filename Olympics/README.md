# Olympics-Dataset

This repository contains a comprehensive dataset on Summer and Winter Olympic athletes and their results from 1896 to 2022. The dataset will be updated with the results from the 2024 Paris Games.

![Olympic Flame](./assets/olympic_flame.jpeg)

---

## Dataset Information

This dataset was sourced from [olympedia.org](https://www.olympedia.org/) and web scraped using Python's Beautiful Soup library by [Keith Galli](https://github.com/KeithGalli). 

Special thanks to him for inspiring this project. You can check out the one he did [here](https://github.com/KeithGalli/Olympics-Dataset)

- **[athletes/bios.csv](./athletes/bios.csv):** Contains raw biographical information on each athlete.
- **[results/results.csv](./results/results.csv):** Provides a detailed breakdown of each event athletes competed in and their results.

---

## Clean Data

Easier-to-analyze data can be found in the [clean-data/](./clean-data/) folder. In addition to the results and bios information, this folder includes:
1. Latitude/longitude [location](./clean-data/bios_locs.csv) data for athletes
2. [NOC region](./clean-data/noc_regions.csv) codes
3. Historical [population](./clean-data/populations.csv) data of countries over time

---

## INSIGHTS

Below are some of the insights that have been derived from the data while performing analysis on it:-

1. **Top Medal-Winning Country:** The United States secured the highest number of medals overall, dominating both the total medal count and the number of gold medals won.

2. **Gold Medal Dominance:** The United States not only led in total medals but also had a significant lead in gold medals, reflecting their dominance across multiple Olympic events.

3. **Medal Distribution Across Countries:** 
   - Countries like Russia and China were identified as consistent top performers, winning a large share of medals, particularly in specific sports or events.
   - Visual trends show that nations like Japan and Great Britain have significantly increased their medal counts in recent Olympic Games.

4. **Countries Without Medals:** A total of 220 countries were identified as never having won an Olympic medal, highlighting the disparity in athletic success across nations.

5. **No Significant Impact of Height and Weight:** Statistical analysis showed no significant difference in the average height and weight between gold medalists and non-gold medalists, indicating that these physical attributes alone do not guarantee Olympic success.

6. **Yearly Medal Trends:**
   - **Top Performers:** Countries like the United States, Russia (formerly Soviet Union), and China consistently dominate the Olympics, leading in medal counts year after year.
   - **Emerging Nations:** Certain countries have shown marked improvement over time, emerging as new competitors in the global Olympic arena.

7. **Medal Distribution by Sport:**
   - **Dominant Disciplines:** The United States excels in track and field, while Russia has a stronghold in gymnastics.
   - **Specialization:** Countries like Kenya have specialized in long-distance running, consistently winning medals in these events.

8. **Historical Performance:** The performance of countries fluctuates across different Olympic Games, possibly due to political, social, or economic factors, as visualized through trend lines over time.

9. **Impact of Host Country:** There is a noticeable increase in the number of medals won by host countries in certain years, suggesting a possible home-field advantage during the Olympics.

## Installation

To run the project locally, open up the code editor of your choice and move to the terminal. Then follow the instructions below:-

1. Clone the repository:

   ```bash
   git clone https://github.com/dakshbhatnagar/projects/Olympics.git
   ```

2. Switch to the directory:
   ```bash
   cd Olympics
   ```

You can now start browsing files and exploring data locally on your machine.
   
---
## Usage

Navigate to and open the Jupyter Notebook files to view detailed analysis, code, and visualizations.
