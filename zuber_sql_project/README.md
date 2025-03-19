README: Zuber SQL Project

Project Overview:
-----------------
This project is an analytical case study for Zuber, a new ride-sharing company launching in Chicago. The objective is to analyze taxi ride data and weather records to uncover patterns in ride frequency, understand passenger preferences, and assess the impact of weather conditions on ride performance.

Project Components:
-------------------
1. **Data Files:**
   - **neighborhoods.csv:** Contains data on Chicago neighborhoods with fields such as `name` and `neighborhood_id`.
   - **cabs.csv:** Contains taxi information including `cab_id`, `vehicle_id`, and `company_name`.
   - **trips.csv:** Contains ride details with fields like `trip_id`, `cab_id`, `start_ts`, `end_ts`, `duration_seconds`, `distance_miles`, `pickup_location_id`, and `dropoff_location_id`.
   - **weather_records.csv:** Contains weather data with fields such as `record_id`, `ts`, `temperature`, and `description`.
   - *Note: The tables are joined by matching the ride start time (`trips.start_ts`) with the weather record time (`weather_records.ts`), despite the absence of a direct foreign key relationship.*

2. **SQL Queries:**
   - **Exploratory Data Analysis:**
     - Count taxi rides per company for November 15-16, 2017, and sort the results in descending order.
     - Filter and count rides for taxi companies whose names contain "Yellow" or "Blue" for November 1-7, 2017.
     - Aggregate rides for the top companies (Flash Cab and Taxi Affiliation Services) and group other companies under "Other" for November 1-7, 2017.
   - **Weather and Ride Analysis:**
     - Retrieve neighborhood identifiers for Loop and O'Hare.
     - Categorize weather conditions hourly using the CASE operator (labeling hours as "Bad" for rain/storm and "Good" otherwise).
     - Analyze ride durations on Saturdays for trips from Loop (pickup_location_id: 50) to O'Hare (dropoff_location_id: 63), incorporating weather conditions.

3. **Documentation:**
   - This README file.
   - Inline comments within the SQL scripts (e.g., `queries.sql`) explaining each step of the analysis.
   - Additional documentation detailing table relationships and analysis workflow.

Methodology:
------------
1. **Data Cleaning and Preparation:**
   - Validated data types, handled missing values, and standardized text fields.
   - Established temporal links between the `trips` and `weather_records` tables by matching `start_ts` with `ts`.

2. **Exploratory Analysis:**
   - Performed detailed analysis on ride frequencies and company performance for specified date ranges.
   - Applied filtering and grouping to identify top-performing taxi companies and aggregate smaller groups.
   - Used JOINs and CASE expressions to merge ride data with weather records, enabling an analysis of weather impact on ride duration.

Key Findings & Recommendations:
-------------------------------
- **Patterns in Ride Frequency:** Analysis identified distinct patterns in ride frequencies tied to specific dates and taxi companies.
- **Weather Impact:** Preliminary results indicate that adverse weather conditions (rain or storms) may influence ride duration and frequency.
- **Strategic Recommendations:** 
  - Further refine scheduling and resource allocation during adverse weather.
  - Consider targeted marketing strategies for taxi companies based on performance trends under different weather conditions.

How to Use the Project Files:
-----------------------------
- Open and view files. This project was completed successfully on the TripleTen platform.

Contact Information:
--------------------
Project Lead: Quinisha Cockheran  
LinkedIn: [Quinisha Cockheran](https://www.linkedin.com/in/quinisha-cockheran)

=============================================
End of README
=============================================
