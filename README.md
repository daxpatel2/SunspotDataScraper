# SunspotDataScraper

SunspotDataScraper is a Python Jupyter Notebook-based tool designed to scrape, analyze, and visualize historical sunspot group data from observatories. This project aims to provide insights into solar activity trends by collecting sunspot data across specified years, calculating the average lifespans of sunspot groups, and generating visual representations of these patterns over time. It’s ideal for researchers, students, and anyone interested in exploring long-term solar cycle trends and the impact of sunspot activity on space weather.

## Project Goals
The primary objectives of SunspotDataScraper are:

To retrieve historical sunspot data from multiple observatory databases.
Analyzing and calculating sunspot groups' average lifespan shows how long groups remain visible.
Analyze and predict Zurich Classification of sunspots to determine patterns in lifespan.
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
     Simply run each cell in the Jupyter Notebook
   - **Fenyi Scraper**:
     Automatically ran inside Specola Database Scraper. However, there is a separate file in case you want to run just the web scrapper code
3. **View Data**: All graphs will be outputted inside of Jupyter Notebook cells
4. **Generate Visualizations**: After running the scrapers, the `SunspotDataScraper` will generate plots to show sunspot lifespans and activity trends and get saved as png using the plt.savefig() method


## Files

- **`Specola_Database_Scrapper.ipynb`**: Scrapes sunspot data from the Specola Observatory database.
- **`Fenyi_Scrapper.ipynb`**: Scrapes data from the Fenyi Observatory database(Already implemented inside of Specola Database Scraper).
- **`sunspot_data_excel.csv`**: Example output data file for sunspot group appearances and lifespans downloaded from Specola Database Archive.
- **`Find_sunspots_switching_zurich_classifications.ipynb`**: Example output data file for sunspot group appearances and lifespans downloaded from Specola Database Archive.

## Contributing

Contributions are welcome! Please submit an issue or pull request if you have suggestions.

1. Fork the repository
2. Create a feature branch (`git checkout -b feature-branch`)
3. Commit your changes (`git commit -m 'Add feature'`)
4. Push to the branch (`git push origin feature-branch`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

Created by [daxpatel2](https://github.com/daxpatel2) – feel free to reach out with questions or feedback!

## Thank You

Big thank you to my research advisors Dr.Asif Ud-Doula and Dr. Gillian Pearce for their guidance in this research.
