# Capital Bikeshare Usage Prediction

## Project Overview

This project aims to predict the usage of Capital Bikeshare services in Washington, DC, by analyzing historical bike usage data along with external factors like weather conditions and public holidays. The goal is to forecast bike demand by date, station, and month to optimize bike station locations and rack capacities, ultimately improving the business's efficiency and user experience.

## Data Sources

The analysis was conducted using data from three key sources:
- **Capital Bikeshare Data**: This dataset spans from October 2010 to March 2023, providing detailed records of bike trips, including start and end stations, trip durations, and timestamps.
- **Weather Data**: Collected from Visual Crossing, this data includes weather conditions specific to Washington, DC, filtered for the same time period to ensure consistency.
- **US Holidays Data**: Sourced from Time and Date, this dataset includes public holidays, which were manually transferred to an Excel sheet and filtered to match the timeline of the bike share data.

## Techniques and Technologies

### Data Processing
- **Data Cleaning and Filtering**: Removed unnecessary columns and ensured consistency across datasets using R and Excel.
- **Data Integration**: Merged the three datasets into a single CSV file, ensuring a comprehensive and relevant dataset for analysis.

### Analytical Techniques
- **Time Series Analysis**: Analyzed trends and patterns over time to understand the factors affecting bike usage.
- **Predictive Modeling**:
  - **Random Forest**: Used to predict bike usage based on historical data, weather conditions, and holiday effects.
  - **Decision Trees (rpart)**: Built interpretable models to understand the decision-making process.
- **Impact Analysis**: Assessed the influence of the COVID-19 pandemic on bike trip demand and model accuracy.

### Visualization and Reporting
- **Geospatial Analysis**: Visualized bike station usage and potential locations using `ggmap` and `ggplot2`.
- **Interactive Dashboards**: Created using `shiny` and `plotly` to allow users to explore the data and predictions interactively.
- **Correlation Analysis**: Used `corrplot` to visualize the relationship between different variables.

### Tools and Libraries
- **R Programming**: The primary language used for data analysis and modeling.
- **Key Libraries**:
  - `dplyr`, `tidyr`, `tidyverse`: For data manipulation and wrangling.
  - `ggmap`, `ggplot2`, `highcharter`: For data visualization.
  - `caret`, `randomForest`, `rpart`: For machine learning and predictive modeling.
  - `shiny`, `plotly`: For interactive visualizations.

## Project Structure

- **Data**: https://drive.google.com/drive/folders/1hsBH2zBBF7BECkSZDbTIfyq9prG-ukV4?usp=sharing .
- **Scripts**: R scripts used for data processing, modeling, and visualization.
- **README.md**: Overview of the project.

## Conclusion

The predictive models developed in this project provide valuable insights into bike usage patterns, helping to optimize the placement and capacity of bike stations in Washington, DC. The project also highlights the importance of considering external factors like weather and public holidays and the need for regular model updates to maintain accuracy, especially during unforeseen events like the COVID-19 pandemic.

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/mohiddin7/Final_project_DATS6101_SIM.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Final_project_DATS6101_SIM
   ```
3. Install the required R packages:
   ```r
   install.packages(c("dplyr", "ggmap", "ggplot2", "tidyverse", "highcharter", "corrplot", "caret", "rpart", "randomForest", "shiny", "plotly"))
   ```
4. Run the R scripts or R Markdown files in the `Scripts` directory.

## Future Work

Future enhancements could include:
- Incorporating real-time data feeds for more accurate and dynamic predictions.
- Expanding the model to include additional external factors, such as major events or public transport disruptions.
- Developing a more sophisticated model to better account on bike usage patterns.


## Acknowledgments

- [Capital Bikeshare for providing the bike usage data](https://www.capitalbikeshare.com/system-data).
- [Visual Crossing for weather data](https://www.visualcrossing.com/weather/weather-data-services).
- [Time and Date for holiday data](https://www.timeanddate.com/holidays/us/%5Byear%5D/).