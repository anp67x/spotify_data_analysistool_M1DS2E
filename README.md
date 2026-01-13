# Spotify Data Analysis Tool (GDPR Export)

## Authors: PACCHIONI Antoine, ROMANENKO German, DIALLO Abdoulaye
- Program: M1 DS2E, University of Strasbourg
- Academic year: 2025–2026


## Overview
This project is a Python data analysis tool that helps analyze personal Spotify data from GDPR exports.
It is implemented as a **Jupyter Notebook (`.ipynb`)**, combining code, explanations, and outputs
(tables/plots) in a single reproducible document.

For privacy reasons, **raw Spotify export files are not included** in this repository. The notebook
contains **precomputed outputs** generated from a personal export so the results can be reviewed
directly on GitHub without running the code.

## How it works 
- The notebook searches Spotify export files using filename patterns
- Loads JSON data into pandas DataFrames
- Cleans and merges datasets (music and podcasts)
- Removes duplicates when exports overlap
- Produces summary tables and visualizations

## Project files
- `Jupyter Notebook code final version.ipynb` : main notebook (code + results)
- `README.md` : documentation
- `.gitignore` : excludes personal data (`data/`, `*.json`, etc.)

## How to reproduce the analysis:

1. Visit the Spotify website (https://www.spotify.com/fr/account/privacy/), log in to your account and request your data under the "Download your data" section at the bottom of the page.

2. After receiving your data via the Spotify email, extract the following three files from the .zip archive:
- StreamingHistory_music_0.json
- StreamingHistory_podcast_0.json
- Inferences.json

Place them either on the Desktop or in a specified `data` folder that is accessible by the software (for example, via the Explorer section in VS Code).

Note: All files can be extracted, but the program will only use the mentioned files.


3. Open the Jupyter Notebook named `Jupyter Notebook code final version.ipynb` using a code editor or a Python distribution.
The code was developed and tested using VS Code and Anaconda.


4. Before running the code, make sure to:
- Have the necessary libraries installed (pandas, matplotlib).
- Choose a Python kernel (top-right in VS Code) where the required libraries are installed.
For reference, the project was developed using Python 3.12.1. When re-running the notebook, the selected kernel should correspond to the Python version where the required libraries are installed. This may vary depending on the user's configuration.


5. You can now run the code using your own exported data, or simply browse the notebook and its precomputed results generated from our dataset.



