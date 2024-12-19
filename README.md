# computer-infrastructure

## Weather Data Automation and Analysis Repository

This repository is designed for automating the collection, storage, and analysis of weather data from the Athenry weather station. Below is an overview of the structure, purpose, and usage of the repository's files and scripts.

### Repository Structure

#### Files

1. **`now.txt`**
   - Contains the date and time of a specific moment when it was last updated.

2. **`formatted.txt`**
   - Contains the same date and time as `now.txt`, but formatted for readability.

3. **`YYYYmmdd_HHMMSS.txt`**
   - An empty file named with the current date and time in `YYYYmmdd_HHMMSS` format (e.g., `20231219_101500.txt`).

4. **`weather.json`**
   - Contains weather data from the Athenry weather station in JSON format.

5. **`YYYYmmdd_HHMMSS.json`**
   - Multiple files in this format are created, each containing weather data from the Athenry weather station at a specific timestamp.

6. **`weather.sh`**
   - A Bash script that automates the creation of new weather data files in the format `YYYYmmdd_HHMMSS.json` by pulling data from the Athenry weather station.

7. **`weather.ipynb`**
   - A Jupyter Notebook containing a brief report explaining the completion of weekly tasks. It also includes code to:
     - Load weather data using `pandas.read_json()`.
     - Examine and summarize the collected weather data.

8. **GitHub Actions Workflow**
   - A CI/CD workflow to automate the execution of `weather.sh` daily at 10:00 AM. This workflow also pushes the newly created weather data file to the repository.

### Features

1. **Automated Weather Data Collection**
   - The `weather.sh` script collects weather data from the Athenry weather station and stores it in a timestamped JSON file.

2. **Daily Automation with GitHub Actions**
   - The workflow runs `weather.sh` daily at 10:00 AM, ensuring up-to-date weather data is collected and committed to the repository automatically.

3. **Data Analysis and Reporting**
   - The `weather.ipynb` notebook provides:
     - Insights into the collected weather data.
     - Summaries and potential visualizations using pandas and other Python libraries.

### Usage

#### Setting Up

1. Clone the repository to your local machine:
   ```bash
   git clone <repository-url>
   ```

2. Ensure you have the following installed:
   - Bash
   - Python (with Jupyter Notebook and pandas)

3. Verify that the GitHub Actions workflow is active in your repository.

#### Running the Script

To manually run the weather data collection script:
```bash
./weather.sh
```

#### Viewing and Analyzing Data

1. Open the Jupyter Notebook:
   ```bash
   jupyter notebook weather.ipynb
   ```
2. Follow the instructions in the notebook to load and analyze the weather data.

### GitHub Actions Workflow

The workflow automatically:
1. Runs the `weather.sh` script daily at 10:00 AM.
2. Commits and pushes the newly generated JSON file to the repository.

#### Enabling the Workflow

Ensure the workflow file is located in `.github/workflows/` and GitHub Actions are enabled for the repository.



### Acknowledgments

Data sourced from the Athenry weather station.

---# Weather Data Automation and Analysis Repository

This repository is designed for automating the collection, storage, and analysis of weather data from the Athenry weather station. Below is an overview of the structure, purpose, and usage of the repository's files and scripts.

## Repository Structure

### Files

1. **`now.txt`**
   - Contains the date and time of a specific moment when it was last updated.

2. **`formatted.txt`**
   - Contains the same date and time as `now.txt`, but formatted for readability.

3. **`YYYYmmdd_HHMMSS.txt`**
   - An empty file named with the current date and time in `YYYYmmdd_HHMMSS` format (e.g., `20231219_101500.txt`).

4. **`weather.json`**
   - Contains weather data from the Athenry weather station in JSON format.

5. **`YYYYmmdd_HHMMSS.json`**
   - Multiple files in this format are created, each containing weather data from the Athenry weather station at a specific timestamp.

6. **`weather.sh`**
   - A Bash script that automates the creation of new weather data files in the format `YYYYmmdd_HHMMSS.json` by pulling data from the Athenry weather station.

7. **`weather.ipynb`**
   - A Jupyter Notebook containing a brief report explaining the completion of weekly tasks. It also includes code to:
     - Load weather data using `pandas.read_json()`.
     - Examine and summarize the collected weather data.

8. **GitHub Actions Workflow**
   - A CI/CD workflow to automate the execution of `weather.sh` daily at 10:00 AM. This workflow also pushes the newly created weather data file to the repository.

## Features

1. **Automated Weather Data Collection**
   - The `weather.sh` script collects weather data from the Athenry weather station and stores it in a timestamped JSON file.

2. **Daily Automation with GitHub Actions**
   - The workflow runs `weather.sh` daily at 10:00 AM, ensuring up-to-date weather data is collected and committed to the repository automatically.

3. **Data Analysis and Reporting**
   - The `weather.ipynb` notebook provides:
     - Insights into the collected weather data.
     - Summaries and potential visualizations using pandas and other Python libraries.

## Usage

### Setting Up

1. Clone the repository to your local machine:
   ```bash
   git clone <repository-url>
   ```

2. Ensure you have the following installed:
   - Bash
   - Python (with Jupyter Notebook and pandas)

3. Verify that the GitHub Actions workflow is active in your repository.

### Running the Script

To manually run the weather data collection script:
```bash
./weather.sh
```

### Viewing and Analyzing Data

1. Open the Jupyter Notebook:
   ```bash
   jupyter notebook weather.ipynb
   ```
2. Follow the instructions in the notebook to load and analyze the weather data.

## GitHub Actions Workflow

The workflow automatically:
1. Runs the `weather.sh` script daily at 10:00 AM.
2. Commits and pushes the newly generated JSON file to the repository.

### Enabling the Workflow

Ensure the workflow file is located in `.github/workflows/` and GitHub Actions are enabled for the repository.

## Contributions

Contributions are welcome! Please open an issue or submit a pull request for improvements or feature additions.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Acknowledgments

Data sourced from the Athenry weather station.

---

For any questions or feedback, feel free to reach out via the repository's issue tracker.



