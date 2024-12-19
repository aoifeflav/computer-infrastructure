# computer-infrastructure
#### Author: Aoife Flavin

## Weather Data Automation and Analysis Repository

This repository is for the module Computer Infrastrucure in Semester 2 of the Higher Diploma in Data Analytics at ATU. It showcases my ability to automate tasks, process and analyze weather data, and create a structured, reproducible workflow. The repository is designed for automating the collection, storage, and analysis of weather data from the Athenry weather station. 
### Repository Structure

#### Files

1. ###### `now.txt`
   - Contains the date and time of a specific moment when the file was created.

2. ###### `formatted.txt`
   - Contains the date and time of a specific moment when the file was created but the date and time are formatted.

3. ###### `YYYYmmdd_HHMMSS.txt`
   - An empty file named with the current date and time in `YYYYmmdd_HHMMSS` format (e.g., `20231219_101500.txt`).

4. ###### `weather.json`
   - Contains weather data from the [Athenry weather station](https://data.gov.ie/dataset/todays-weather-athenry) in JSON format.

5. ###### `YYYYmmdd_HHMMSS.json`
   - Multiple files in this format are created, each containing weather data from the Athenry weather station at a specific timestamp.

6. ###### weather.sh`
   - A Bash script that automates the creation of new weather data files in the format `YYYYmmdd_HHMMSS.json` by pulling data from the Athenry weather station.

7. ###### `weather.ipynb`
   - A [Jupyter Notebook](https://jupyter.org/) containing a brief report explaining the completion of weekly tasks. It also includes code to:
     - Load weather data using `pandas.read_json()`.
     - Examine and summarize the collected weather data.

8. ###### `.github/workflows/weather.yml`
  - A GitHub Actions workflow that automates the execution of the `weather.sh` script daily at 10 AM and pushes the new data file to the repository.

9. ###### `requirements.txt`
  - A file listing the Python dependencies required to run the notebook and scripts, including:
    - [`pandas`](https://pandas.pydata.org/)
    - [`matplotlib`](https://matplotlib.org/)
    - [`glob`](https://en.wikipedia.org/wiki/Glob_(programming))

### Features

1. **Automated Weather Data Collection**
   - The `weather.sh` script collects weather data from the Athenry weather station and stores it in a timestamped JSON file.

2. **Daily Automation with GitHub Actions**
   - The workflow runs `weather.sh` daily at 10:00 AM, ensuring up-to-date weather data is collected and committed to the repository automatically.

3. **Data Analysis and Reporting**
   - The `weather.ipynb` notebook provides:
     - Insights into the collected weather data.
     - Summaries and potential visualisations using pandas and other Python libraries.

## Usage

### Running the Script Locally
To manually run the weather script and collect data:
1. Ensure you have [Bash](https://en.wikipedia.org/wiki/Bash_(Unix_shell)) installed.
2. Run the script using:
   ```bash
   ./weather.sh
   ```

### Viewing the Notebook
To explore the analysis:
1. Install the required Python libraries using:
   ```bash
   pip install -r requirements.txt
   ```
2. Open the `weather.ipynb` file in a Jupyter Notebook environment.
3. Execute the cells to view the data analysis and results.

### Using the Repository Online
You can also use this repository online with GitHub Codespaces:
1. Open the repository in GitHub.
2. Click on the "Code" button and select "Codespaces".
3. Start a new Codespace to access the scripts and notebook directly in a cloud-based development environment.

## Prerequisites
- Bash (to run `weather.sh` locally)
- Python with the following libraries:
  - [`pandas`](https://pandas.pydata.org/)
  - [`matplotlib`](https://matplotlib.org/)
  - [`glob`](https://en.wikipedia.org/wiki/Glob_(programming))
- GitHub repository with Actions enabled for automation.

## Acknowledgements
- Data source: [Athenry weather station](https://data.gov.ie/dataset/todays-weather-athenry)

## Future Improvements
- Extend data analysis to include predictive modeling of weather trends.
- Integrate additional weather stations for a broader dataset.
- Enhance visualizations with more advanced plotting libraries like [`seaborn`](https://seaborn.pydata.org/).


End
