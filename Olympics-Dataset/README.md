# Olympics-Dataset

This repository contains a comprehensive dataset on Summer and Winter Olympic athletes and their results from 1896 to 2022. The dataset will be updated with the results from the 2024 Paris Games.

![Olympic Flame](./assets/olympic_flame.jpeg)

---

## Dataset Information

This dataset was sourced from [olympedia.org](https://www.olympedia.org/) and web scraped using Python's Beautiful Soup library by [Keith Galli](https://github.com/KeithGalli).

- **[athletes/bios.csv](./athletes/bios.csv):** Contains raw biographical information on each athlete.
- **[results/results.csv](./results/results.csv):** Provides a detailed breakdown of each event athletes competed in and their results.

---

## Clean Data

Easier-to-analyze data can be found in the [clean-data/](./clean-data/) folder. In addition to the results and bios information, this folder includes:
- Latitude/longitude location data for athletes
- NOC region codes
- Historical population data of countries over time

---

## Insights 

1. **Top Medal-Winning Country:**
   - The United States athletes secured the highest number of medals overall, dominating both the total medal count and the number of gold medals won.

2. **Gold Medal Dominance:**
   - The analysis highlighted that the United States not only led in total medals but also had a significant lead in gold medals, reflecting their dominance across multiple Olympic events.

3. **Medal Distribution Across Countries:**
   - Other countries, such as Russia and China, were also identified as top performers, consistently winning a large share of the medals, particularly in specific sports or events.

4. **Emerging Medalists:**
   - Some countries showed improvement over the years, with nations like Japan and Great Britain increasing their medal counts in recent Olympic Games.

5. **Countries Without Medals:**
   - The analysis identified a number of countries that have never won an Olympic medal, emphasizing the disparity in athletic success across different nations.

---

## Acknowledgment

Special thanks to [Keith Galli](https://github.com/KeithGalli/Olympics-Dataset) for the inspiration for this project.