# Executive Summary
Understanding how social services are distributed in New York City is essential for addressing the ongoing crisis of poverty and homelessness. Using R, this project analyzes publicly available data to evaluate whether the allocation of key resources aligns with the borough-specific needs of NYC’s population.

Findings show that The Bronx and Brooklyn have the highest levels of need, yet resource allocation does not fully match this demand, particularly in The Bronx. In contrast, Staten Island has the lowest need and the fewest services, reflecting a more proportional distribution.

Future recommendations include closer monitoring of borough-specific needs over time and exploring additional data sources to assess service accessibility beyond location, such as capacity and wait times.

# Problem Statement

Homelessness and poverty continue to impact a significant portion of New York City’s population, with 17% of residents living below the poverty line (U.S. Census Bureau). How can we better understand and optimize the availability of services for New Yorkers living in poverty or at risk of homelessness?

# Methodology
1. Import and merge NYC Open Data JSON files (70K+ rows) in R.
2. Clean data and handle missing values.
3. Create three data frames: population (2020 Census), poverty indicators (evictions, SNAP), and resource distribution (e.g., shelters, employment programs).
4. Calculate summary statistics (min, max, mean, median, SD).
5. Perform ANOVA to assess differences in resource allocation by borough.
6. Visualize data using tables and bar graphs to compare population, need, and available resources across boroughs.

# Skills
- R
  - Data import (JSON)
  - Merging large datasets
  - Handling NAs
  - Data wrangling (Tidyverse: dplyr, tidyr)
  - Data visualization (Tidyverse: ggplot2)
  - Statistical analysis
  - ANOVA (Supernova)
  - Table formatting (KableExtra)

# Results & Recommendation

A key insight from this analysis is that The Bronx and Brooklyn have the highest levels of risk indicators, as shown by the high amount of residential evictions and SNAP recipients. However, in The Bronx, access to resources does not always increase proportionately to match the need, particularly for shelters, employment programs, and community centers, as it does in Brooklyn. Additionally, Queens shows moderate need but does not receive proportionate support for employment or shelter services.

Due to these findings, I recommend focusing efforts on increasing targeted resources to better match the higher need. Specifically, re-allocating or expanding employment programs, shelters, and community centers, where need is high. Also, reassessing service distribution in Queens to ensure it reflects the needs of the communities in that borough.

These adjustments could increase the effectiveness of these resources in meeting the actual needs of New Yorkers in poverty across all boroughs.

# Next Steps

- Monitor borough trends over time to identify changes in population, and any service that may appear as a result.
- Incorporate additional data sources that capture service accessibility metrics, such as program capacity, utilization rates, and wait times.
- Conduct geospatial analysis to identify high-need neighborhoods within each borough, and evaluate their accessibility to services.
- Partner with community stakeholders to validate findings and gain further insights that may not be present in the data.
