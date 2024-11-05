# SunspotDataScraper

SunspotDataScraper is a Python-based tool designed to scrape, analyze, and visualize historical sunspot group data from observatories. This project aims to provide insights into solar activity trends by collecting sunspot appearance data across specified years, calculating the average lifespans of sunspot groups, and generating visual representations of these patterns over time. It’s ideal for researchers, students, and anyone interested in exploring long-term solar cycle trends and the impact of sunspot activity on space weather.

## Project Goals
The primary objectives of SunspotDataScraper are:

To retrieve historical sunspot data from multiple observatory databases.
Analyzing and calculating sunspot groups' average lifespan shows how long groups remain visible.
To generate time-series visualizations of sunspot data, allowing users to observe solar cycle patterns and trends.
To enable customizable data collection ranges, users can specify particular years or periods of interest in the list_of_years data structure.
This project can help provide context for studies of solar behavior, potential impacts on Earth's geomagnetic environment, and historical solar cycle analysis.

## Features

- **Data Retrieval**: Automatically scrapes sunspot data from multiple observatories.
- **Data Processing**: Cleans and organizes raw data into structured formats for easy analysis.
- **Visualization**: Generates plots for average sunspot lifespan and trends across specific timeframes.
- **Customizable**: Easily modify the years or range of data being retrieved for tailored analysis.

## Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/daxpatel2/SunspotDataScraper.git
   cd SunspotDataScraper
   ```

2. **Install dependencies**:
   This project uses Python libraries including `requests`, `pandas`, and `matplotlib`. Install them with:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Set the Desired Years**: In the scripts, you can modify the `list_of_years` to specify the years you want to retrieve data for.
2. **Run the Scrapers**:
   - **Specola Database Scraper**:
     ```bash
     python Specola_Database_Scrapper.ipynb
     ```
   - **Fenyi Scraper**:
     ```bash
     python Fenyi_Scrapper.ipynb
     ```
3. **View Data**: The scripts will output data in the console and optionally save results to `.csv` files.
4. **Generate Visualizations**: After running the scrapers, the `SunspotDataScraper` will generate plots to show sunspot lifespans and activity trends.

## Example

Here’s an example of how to retrieve data for sunspot groups and calculate their average lifespans by year:

```python
# Import the scraper functions
from Specola_Database_Scrapper import retrieve_and_process_data, calculate_group_durations

# Retrieve and process data for a specific year
data = retrieve_and_process_data('1974')

# Calculate average group durations
durations = calculate_group_durations(data)
print(durations)
```

## Files

- **`Specola_Database_Scrapper.ipynb`**: Scrapes sunspot data from the Specola Observatory database.
- **`Fenyi_Scrapper.ipynb`**: Scrapes data from the Fenyi Observatory database.
- **`sunspot_data_excel.csv`**: Example output data file for sunspot group appearances and lifespans.

## Contributing

Contributions are welcome! Please submit an issue or pull request if you have suggestions for improvements or bug fixes.

1. Fork the repository
2. Create a feature branch (`git checkout -b feature-branch`)
3. Commit your changes (`git commit -m 'Add feature'`)
4. Push to the branch (`git push origin feature-branch`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

Created by [daxpatel2](https://github.com/daxpatel2) – feel free to reach out with questions or feedback!
