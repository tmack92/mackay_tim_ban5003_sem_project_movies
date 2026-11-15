# BAN5003 Final Project: Movie Runtime, Audience Sentiment, and Cast/Directors That Buck the Trend

**BAN 5003: Data Management and Analytics Integration**  
Timothy Mackay

This repository contains the project starter notebook, curated data files, environment files, and output folders for the Movies final project option.

Detailed project instructions, milestone requirements, due dates, rubric, report guide, and presentation guide are provided in Canvas/LMS.

## Disclaimer
> **Note:** Initialized from Dr. Zu's BAN 6003 Movies starter template and adapted for BAN 5003. For brevity, this README will be updated prior to final submission to reflect additions, edits, and removals made across the project notebook.


## Data

The curated CSV files are stored in `data/`:


This project uses movie metadata, user ratings, links, credits, and keywords. A common final ABT is one row per movie.

Important: `ratings.csv` is rating-event-level, not movie-level. Aggregate ratings by `movieId` before merging ratings into a movie-level ABT.

See `data/README.md` for row meaning, expected keys, and join guidance for each file.


## SQL with DuckDB

The starter notebook uses DuckDB to run SQL directly on your pandas DataFrames and on the exported ABT CSV file, for example to check row counts, key uniqueness, and one aggregation against the pandas result. Milestone 2 requires at least one DuckDB query on your own project data. Using a hosted database such as Neon is optional and has no course guide.

Similarly, postgres and DBeaver will be used for quick SQL Queries when doing so in VS Code would be a hinderence on the workflow in the notebook.

## Working Environment

Path Used.

1. Created repository from the starter template on GitHub and cloned locally via GitHub Desktop.
2. Open the repository in VS Code.
3. pip install -r requirements.txt
4. Open the starter notebook.
5. Run cells from top to bottom.


## Expected Repository Organization

Use the existing folders:

- `notebooks/`: your project notebook
- `data/`: provided data files
- `outputs/`: required final ABT (`outputs/movies_final_abt.csv`) and data dictionary (`outputs/movies_data_dictionary.csv`), plus model metrics or other exported outputs
- `reports/`: HTML report exported from your final notebook, and other final report files

## Required Output Files

Your final repository must include these two files with these exact names:

- `outputs/movies_final_abt.csv`: your final ABT
- `outputs/movies_data_dictionary.csv`: the data dictionary for every column in your final ABT


## Project Deliverables (BAN 5003)

This repository contains the analytical artifacts for BAN 5003:

- **Project Notebook:** `notebooks/movies_project_starter.ipynb`
- **Final Analytical Base Table:** `outputs/movies_final_abt.csv`
- **Data Dictionary:** `outputs/movies_data_dictionary.csv`
- **Model Metrics & Outputs:** Saved in `outputs/`
- **AI Prompt Logs:** Saved in `ai/prompts/`
- **Executive Deck & Summary:** Saved in `reports/`


## Academic Integrity and AI Use

- Your commit history will be reviewed. Commit and push regularly as you work. Do not upload everything in one large commit at the end.
- At the end of your final notebook, include a markdown cell titled **AI use disclosure**. State which AI tools you used and what you used them for, or write "None".
- You may be asked to explain any part of your code or analysis.
