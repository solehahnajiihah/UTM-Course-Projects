# Change in Mean Sea Level

## Introduction
**Change in mean sea level** refers to long-term rises or falls in the average ocean height, defined as the midpoint between average high and low tides, and is a crucial indicator in climate and environmental studies. Rising mean sea levels, driven mainly by global warming through glacier and ice sheet melting, thermal expansion of seawater, and increased greenhouse gas concentrations, pose serious environmental and socio-economic risks. These include coastal erosion, damage to infrastructure, increased flooding and storm severity, saltwater intrusion into freshwater sources, loss of coastal habitats such as mangroves and salt marshes, threats to marine biodiversity, and displacement of coastal and island communities. Mean sea level trends are monitored using tide gauges, satellite altimetry, and climate models to assess past changes and predict future scenarios. Understanding these changes is essential for informing climate policies and adaptation strategies, such as coastal defenses and managed retreat, to protect vulnerable ecosystems and human populations.

## Problem Background
Global mean sea level is an important indicator of the warming climate. However when assessing potential impacts at the coastal areas, it is the change in regional mean sea level that is most important. The threat of rising sea level can results to the vulnerability of coastal communities to increased flooding, high tides, erosion and displacement. In order to cope with this rising sea level matter, governments must make adaptation or mitigation strategies such as building sea walls, flooding flood defense and managed retreat. By analyzing the trends of regional mean sea level, the governments of the respective areas can be alert about the dangers and take preventive measures.

## Dataset:
The dataset provides insights into the change in mean sea level over time. This dataset is obtained from the National Oceanic and Atmospheric Administration (NOAA) and includes measurements in millimeters for various regions worldwide. The data spans from 1992 to 2023, offering a comprehensive view of sea-level fluctuations over this period. The dataset consists of 35604 rows and 13 columns.

## Dataset Description :
The dataset contains the following columns relevant to our analysis:

Measure: The area where measure are taken (e.g., Andaman Sea, Arabian Sea).
Date: The date of the measurement (from December 17, 1992, to December 16, 2023).
Value: The change in mean sea level in millimeters compared to a reference point.

## Research Question
This study seeks to analyse the variations in the average height of the ocean's surface over time. Mean sea level is a vital metric in oceanography, climate science, and environmental studies, representing the midpoint between the mean high and low tides at a particular regions. This measure is crucial for understanding a variety of environmental and socio-economic impacts.

1. What is the mean values for different regions.
2. What is the overall trend in mean sea level rise for each region over the past years?
3. How can we predict future sea levels based on historical data?

## Data Cleaning and Preparation
The dataset detailing changes in mean sea levels includes various attributes such as ObjectId, Country, ISO2, ISO3, Indicator, Unit, Source, CTS_Code, CTS_Name, CTS_Full_Descriptor, Measure, Date, and Value. Before conducting any analysis, it is essential to ensure the data is clean and well-prepared. Here are the steps undertaken for data cleaning and preparation:

### Handling Missing Values
Missing values can significantly affect the accuracy and reliability of our analysis. In this dataset, we focused on critical columns such as Value and Date. The Value column represents the measured change in sea level, and any missing entries here would lead to incomplete or misleading analysis results. Similarly, the Date column is crucial for any time-series analysis, and missing dates would disrupt the continuity of our data. Therefore, any rows containing missing values in these columns were removed to ensure data integrity.

### Data Type Conversion
Next, data type conversion was performed, particularly for the Date column. Initially stored as a string, the Date column was extracted and converted into a datetime format to facilitate time-series analysis. Converting the date strings into a datetime object allows for accurate date-related operations, such as grouping data by year or month and plotting time-series graphs. This step is vital for ensuring that the temporal aspects of the data are correctly interpreted and handled.


### Removing Unnecessary Columns
To streamline the dataset and focus on the most relevant information, unnecessary columns were removed. The initial dataset contained several columns that were not directly needed for our analysis, such as ObjectId, ISO2, ISO3, Indicator, Unit, Source, CTS_Code, CTS_Name, and CTS_Full_Descriptor. These columns, while potentially useful for other types of analysis, were not essential for our specific goal of examining sea level changes over time. By removing these columns, we reduced the dataset to the essential attributes: Country, Measure, Date, and Value.

### Adding a New Column
To provide additional context and facilitate broader analysis, we can map each body of water (Measure) to its corresponding ocean. This step involves creating a new column Ocean based on a predefined mapping dictionary, sea_to_ocean, which contains mappings of various seas to their respective oceans.


### Final Cleaned Dataset
After these steps, the cleaned dataset is now ready for further analysis and visualization.These steps ensure that our data is accurate, consistent, and relevant for the subsequent analysis. The cleaned dataset provides a solid foundation for exploring trends in sea level changes, performing aggregations, and applying machine learning models to predict future changes.


<img width="1226" height="1337" alt="image" src="https://github.com/user-attachments/assets/d87beb7b-ca9e-49d9-bb66-dd8ba80f888a" />

<img width="1206" height="953" alt="image" src="https://github.com/user-attachments/assets/20c15006-e6e3-4731-92b3-b6807c629c4b" />
