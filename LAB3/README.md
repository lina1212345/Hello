Key Outcomes and Descriptions

• Data Ingestion & Formatting

 Action: Loaded the global_cars_enhanced.xlsx file and corrected the structure.
Outcome: The first row of the raw file was incorrectly identified as data; the notebook manually reassigned this row as column headers and reset the index to create a clean table of 300 cars.

• Data Integrity Verification

Action: Checked for missing values (isna) and duplicate records.
Outcome: Confirmed the dataset is complete with 0 missing values across all 16 columns and contains no duplicate entries.

• Feature Type Conversion

Action: Converted data types from generic objects to numeric formats (int64 and float64).
Outcome: Key variables like Price_USD, Horsepower, and Efficiency_Score are now computationally accessible for statistical calculations and plotting.

• Descriptive Statistical Profiling

Action: Generated a summary of the dataset's central tendencies and ranges.
Outcome: Established a baseline for the market: the average car price is approximately $60,848, with engines averaging 3052 CC and an average car age of roughly 11 years.

• Univariate Distribution Analysis

Action: Created a visual distribution (histogram) of car prices.
Outcome: Provided a visual representation of how car prices are spread across the dataset, identifying common price brackets for the inventory.
