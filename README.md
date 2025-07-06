# Accident Prediction Dataset README

## Overview
This dataset contains detailed records of traffic accidents across various states and cities in India, spanning multiple years.
It is designed to support analysis and predictive modeling of accident occurrences, severity, and contributing factors such as weather, road conditions, and driver characteristics.
The dataset includes a variety of attributes related to each accident, making it suitable for statistical analysis, machine learning, and research purposes.

## Dataset Details
- Source: Unknown (synthetic or anonymized data assumed)
- Time Period: 2018–2023
- Geographical Scope: Multiple states and cities in India
- Format: Comma-Separated Values (CSV)
- Size: 300+ records

## Columns Description
The dataset consists of 22 columns, each representing a specific attribute of an accident. Below is a detailed description of each column:

1. State Name: The state in India where the accident occurred (e.g., Uttar Pradesh, Rajasthan).
2. City Name: The city where the accident occurred (e.g., Lucknow, Jodhpur). Often listed as "Unknown" if unspecified.
3. Year: The year the accident took place (e.g., 2018, 2023).
4. Month: The month of the accident (e.g., January, May).
5. Day of Week: The day of the week when the accident occurred (e.g., Monday, Saturday).
6. Time of Day: The time of the accident in 24-hour format (e.g., 1:46, 23:22).
7. Accident Severity: Severity level of the accident (e.g., Minor, Serious, Fatal).
8. Number of Vehicles Involved: Number of vehicles involved in the accident (e.g., 1, 5).
9. Vehicle Type Involved: Primary type of vehicle involved (e.g., Car, Truck, Cycle, Pedestrian).
10. Number of Casualties: Total number of individuals injured or killed (e.g., 0, 10).
11. Number of Fatalities: Number of deaths resulting from the accident (e.g., 0, 5).
12. Weather Conditions: Weather at the time of the accident (e.g., Clear, Rainy, Foggy, Hazy, Stormy).
13. Road Type: Type of road where the accident occurred (e.g., National Highway, Urban Road, Village Road).
14. Road Condition: Condition of the road (e.g., Dry, Wet, Damaged, Under Construction).
15. Lighting Conditions: Lighting at the time of the accident (e.g., Daylight, Dusk, Dawn, Dark).
16. Traffic Control Presence: Presence of traffic control measures (e.g., Signs, Signals, Police Checkpost, None).
17. Speed Limit (km/h): Posted speed limit at the accident location (e.g., 30, 120).
18. Driver Age: Age of the primary driver involved (e.g., 20, 70).
19. Driver Gender: Gender of the primary driver (e.g., Male, Female).
20. Driver License Status: License status of the driver (e.g., Valid, Expired, None).
21. Alcohol Involvement: Whether alcohol was involved (e.g., Yes, No).
22. Accident Location Details: Specific location feature of the accident (e.g., Straight Road, Curve, Bridge, Intersection).

## Data Characteristics
- Missing Values: The "City Name" column frequently contains "Unknown," indicating missing or unspecified data.
- Categorical Variables: Many columns (e.g., Weather Conditions, Road Type, Accident Severity) are categorical and suitable for encoding in predictive models.
- Numerical Variables: Columns like Number of Casualties, Number of Fatalities, Speed Limit, and Driver Age are numerical and can be used for statistical analysis.
- Temporal Data: Year, Month, Day of Week, and Time of Day provide a temporal context for trend analysis.
- Potential Anomalies: Some entries (e.g., high casualty counts with zero fatalities) may require validation or cleaning depending on use case.

## Usage Notes
1. Preprocessing:
   - Handle "Unknown" values in the City Name column (e.g., impute, exclude, or treat as a separate category).
   - Convert categorical variables (e.g., Weather Conditions, Driver Gender) into numerical encodings (e.g., one-hot encoding) for machine learning models.
   - Parse the Time of Day column into a consistent format (e.g., convert "8:4" to "08:04") for time-based analysis.
   - Check for inconsistencies (e.g., Number of Casualties vs. Number of Fatalities) and resolve as needed.

2. Potential Applications:
   - Predictive Modeling: Use features like Weather Conditions, Road Type, and Driver Age to predict Accident Severity or Number of Fatalities.
   - Trend Analysis: Analyze accident patterns by Year, Month, or Day of Week to identify seasonal or temporal trends.
   - Risk Assessment: Assess risk factors such as Alcohol Involvement, Speed Limit, or Road Condition for safety interventions.

3. Limitations:
   - The dataset lacks specific coordinates or detailed location data beyond State Name and City Name.
   - Some fields (e.g., Driver License Status) may not fully capture nuanced legal statuses.
   - The sample size may not be representative of all accident scenarios across India.

## Example Analysis Questions
- What are the most common weather conditions associated with fatal accidents?
- How does accident severity vary by road type or lighting conditions?
- Is there a correlation between driver age and alcohol involvement in accidents?
