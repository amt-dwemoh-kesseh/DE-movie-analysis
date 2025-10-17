# TMDB Movie Data Analysis

This project analyzes movie data sourced from The Movie Database (TMDB) API. It fetches detailed information for a curated list of movies, cleans and preprocesses the data, computes key performance indicators (KPIs), and generates visualizations to uncover insights about movie franchises, genres, budgets, revenues, and more.

## Features

- **Data Fetching**: Retrieves movie data including credits, genres, production details, and financial metrics from TMDB API.
- **Data Cleaning**: Processes raw API responses to extract and normalize key fields, handle missing values, and remove duplicates.
- **KPI Analysis**: Computes rankings for highest/lowest revenue, budget, profit, ROI, ratings, popularity, and more.
- **Advanced Queries**: Performs targeted searches based on complex criteria (e.g., genre-director-actor combinations).
- **Comparative Analysis**: Compares franchise vs. standalone movies, identifies top franchises and directors.
- **Visualizations**: Generates scatter plots, bar charts, and line graphs to illustrate relationships and trends.
- **Export**: Saves cleaned data to CSV for further analysis.

## Requirements

- Python 3.7+
- Libraries: `pandas`, `numpy`, `matplotlib`, `requests`, `python-dotenv`
- TMDB API Key (free account required from [TMDB](https://www.themoviedb.org/settings/api))

## Installation

1. Clone or download this repository.
2. Install required Python packages:
   ```
   pip install pandas numpy matplotlib requests python-dotenv
   ```
3. Obtain a TMDB API key:
   - Sign up for a free account at [TMDB](https://www.themoviedb.org/account/signup).
   - Go to your account settings and generate an API key under the "API" section.
4. Create a `.env` file in the project root and add your API key:
   ```
   TMDB_API_KEY=your_api_key_here
   ```

## Usage

1. Open `TMDB_Movie_Data_Analysis.ipynb` in Jupyter Notebook or JupyterLab.
2. Run the cells sequentially:
   - **Cell 1**: Project title and overview.
   - **Cell 2**: Import libraries and load environment variables.
   - **Cell 3**: Fetch movie data from TMDB API.
   - **Cells 4-6**: Data cleaning and preprocessing.
   - **Cell 8**: KPI computations and rankings.
   - **Cell 9**: Advanced filtering and search queries.
   - **Cell 10**: Franchise vs. standalone analysis.
   - **Cell 11**: Top franchises and directors.
   - **Cells 12-16**: Visualizations.
   - **Cell 17**: Conclusions.
   - **Cell 18**: Export cleaned data to `tmdb_cleaned.csv`.
3. View results, plots, and the exported CSV file.

## Data

- **Input**: Movie IDs are hardcoded in the notebook for demonstration. Modify `MOVIE_IDS` to analyze different movies.
- **Output**: `tmdb_cleaned.csv` contains the processed dataset with columns like title, budget, revenue, genres, director, etc.
- **Source**: TMDB API (v3). Note: API calls may fail for invalid IDs or rate limits; the notebook handles errors gracefully.

## Project Structure

- `TMDB_Movie_Data_Analysis.ipynb`: Main Jupyter notebook with analysis code.
- `notebook_explanation.md`: Detailed cell-by-cell breakdown of the notebook.
- `tmdb_cleaned.csv`: Exported cleaned dataset.
- `.env`: Environment file for API key (not included in repository).
- `.ipynb_checkpoints/`: Jupyter auto-save directory.

## Key Insights (Sample)

- Franchise movies tend to have higher average revenue and budgets compared to standalone films.
- Certain genres (e.g., Animation, Adventure) show higher ROI.
- Revenue has trended upward over recent decades.
- Top directors and franchises are ranked by total revenue and average ratings.

## License

This project is for educational purposes. TMDB data is subject to their terms of use. Ensure compliance with API usage policies.

## Contributing

Feel free to fork and enhance the analysis. Suggestions for additional KPIs or visualizations are welcome.