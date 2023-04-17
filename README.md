# Project Title: UdacityPost - A Quick German Electrical Power Market Overview from 2019 to 2022
# Motivation:
  Learning how to deal with public excess able data sets and outline findings.

# Project Description: 
  To gather insights into German electrical power market a appropriate data source had to be identified. 
  Therefore https://transparency.entsoe.eu/dashboard/show was used. 
  The business aim is to get general insight, from a human perspective visual data is better processed. 
  Therefore, the it was necessary to deal with categorical and missing data. Data was wrapped to get best visualizations. 

# Libraries:
  numby, datetime from datetime, pandas, matplotlib.pyplot, matplotlib.cm, display from IPython

# Files in repo:
  The Data:
            Total Load - Day Ahead _ Actual_201901010000-202001010000.csv -- Total and Day Ahead Load every 15 minutes
            Total Load - Day Ahead _ Actual_202001010000-202101010000.csv 
            Total Load - Day Ahead _ Actual_202101010000-202201010000.csv 
            Total Load - Day Ahead _ Actual_202201010000-202301010000.csv 
            Total Load - Day Ahead _ Actual_202301010000-202401010000.csv 

            Day-ahead Prices_201901010000-202001010000.csv -- Prices per MW/h day ahead every 15 minutes
            Day-ahead Prices_202001010000-202101010000.csv
            Day-ahead Prices_202101010000-202201010000.csv
            Day-ahead Prices_202201010000-202301010000.csv
            Day-ahead Prices_202301010000-202401010000.csv

            Actual Generation per Production Type_201901010000-202001010000.csv -- Actual Generation per Production Type every 15 minutes
            Actual Generation per Production Type_202001010000-202101010000.csv
            Actual Generation per Production Type_202101010000-202201010000.csv
            Actual Generation per Production Type_202201010000-202301010000.csv
            Actual Generation per Production Type_202301010000-202401010000.csv
  The code:
            GEM_2019_2023.ipynb -- joins the data above, unifies data, drops empty rows, handles NaN values, align datatypes, plot data, subset data, 
                                   check data consistency, ensure data consistency, visualize data 
          
# Results summary: 
  -The overall load over the last years 2019 to 2022 was almost constant around 500 TW.
  -The price for a MW/h jumped from an average of 37.94 EUR in 2019 to 237.54 EUR in 2022.
  -The biggest German electrical power sources are fossil Brown Coal/Lignite (19.6%-2019 / 20.4%-2022) and Wind Onshore (19.1%-2019 / 19.9%-2022).
  -The third major source in 2019 nuclear power (13.5%-2019) become the 7th in 2022 (6.5%). 3rd in 2022 is solar (11.0%).
  -Three sources changed over 10 TW Solar and Fossil Hard Coal increased and Nuclear decreased by almost 40TW. 
  -A load pattern can be identified over time, for every year with peaks in winter and saddle in summer,
    for every week with a plateaus on weekdays and dips on weekends, for every day with dips at night and peaks at lunch time. 
  -The general yearly trend is also mirrored in daily peaks and dips.
