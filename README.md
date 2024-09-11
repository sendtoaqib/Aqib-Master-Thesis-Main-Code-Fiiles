# Eye Gaze and GSR Analysis Project


This project involves analyzing eye gaze data (saccades, fixations) and Galvanic Skin Response (GSR) data collected from participants using Cargo Bikes and Normal Bikes under various conditions. The project includes data cleaning, analysis, visualization, and correlation analysis between eye gaze metrics and GSR data.
Note: Please download the data files from this link to run the project and get correct results : https://1drv.ms/f/s!AkMVUg1WxxiWgfs3MGyaiUrTqdQdHQ?e=wkVLq8

## Table of Contents

- [Project Structure](#project-structure)
- [Data Collection](#data-collection)
- [Data Cleaning](#data-cleaning)
- [Analysis](#analysis)
- [Visualization](#visualization)
- [Correlation Analysis](#correlation-analysis)
- [Output Files](#output-files)
- [Dependencies](#dependencies)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Project Structure

- **`data_storage/`**: Contains the cleaned data after processing.
- **`output_csv_files/`**: Contains CSV files with the results of various analyses.
- **`scripts/`**: Contains the Python scripts used for data processing and analysis.
- **`README.md`**: This file, providing an overview of the project.

## Data Collection

The data was collected under different conditions:
- **Route Types**: Short Route (Experiment 1), Long Route (Experiment 2)
- **Bike Types**: Cargo Bike, Normal Bike
- **Load Conditions**: With Load, No Load
- **Speed Conditions**: High Speed, Low Speed

## Data Cleaning

### Functions

- **`clean_eye_data()`**: Cleans the eye data by filtering out low-confidence data and removing rows with missing values.
- **`clean_gsr_data()`**: Cleans the GSR data by ensuring relevant columns are valid and non-empty.

### Procedure

1. **Loading**: CSV files are loaded into a data structure.
2. **Cleaning**: Data is cleaned to ensure it is suitable for analysis.

## Analysis

### Average Gaze Positions

Calculated for different conditions based on bike type, load, and speed.

### Average Saccades and Fixations

Calculated for different conditions and compared between Cargo Bike and Normal Bike.

### Average GSR

Analyzed for different conditions, comparing Cargo Bike and Normal Bike, and considering factors like speed and load.

## Visualization

Various bar graphs are generated to visualize the data:
- **Gaze Positions**: Compared across different conditions.
- **Saccades and Fixations**: Magnitude of saccades and duration of fixations.
- **GSR**: Average GSR values compared across conditions.

### Heatmap

A heatmap was created to visualize the correlation between eye saccades and GSR SCR data.

## Correlation Analysis

Performed to explore the relationship between eye gaze metrics (saccades) and GSR data (SCR). The results are saved in both raw data format and as a correlation matrix CSV file.

## Output Files

- **`average_gaze_positions.csv`**: Average gaze positions for various conditions.
- **`average_saccades.csv`**: Average saccades magnitude.
- **`average_fixations.csv`**: Average fixation duration.
- **`average_gsr.csv`**: Average GSR values.
- **`saccades_scr_correlation.csv`**: Correlation matrix between saccades and SCR.
- **`saccades_scr_raw_data.csv`**: Raw data for saccades and SCR.

## Dependencies

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## Usage

1. Clone the repository.
2. Ensure the required dependencies are installed.
3. Run the Python scripts in sequence to process the data, perform the analysis, and generate visualizations.
4. Check the `output_csv_files` directory for the resulting CSV files.

## Contributing

Contributions are welcome! Please submit a pull request or open an issue to discuss any changes.

## License

This project is licensed under the MIT License. See the LICENSE file for details.
