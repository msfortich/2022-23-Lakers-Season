Welcome to my Final Project!

Please read the following instructions and run the following in this order.

I am using Python 3.11.5

**requirements.txt** - Contains all the external libraries I used for this project, that you need to install in order to run the following files. I used:

matplotlib==3.8.1
nba_api==1.4.1
numpy==1.26.1
pandas==2.1.2
requests==2.31.0
seaborn==0.13.0
Note I use nba_api which requires Python 3.7+ along with the requests and numpy packages.

To install requirements, run:
    pip install -r requirements.txt

**Fortich DSCI 510 Final Project Report.pdf** - Contains my research question, analysis, and reults in full.
    
**Folders:**

**data** - contains 2 subfolders raw and processed each with one jupyter notebook and 2 data files

data/raw - contains raw data and 1 jupyter notebook

File a. get_data.ipynb - This is a jupyter notebook that extracts the raw data from balldontlie API and NBA API library. This file uses the requests library, pandas library, json library, and the nba_api library in python. It creates two different files: one JSON file and one CSV file and imports it into this subfolder. Run this file using 'Run All'.

raw data a. lakergames2022.json - contains Lakers 2022-23 Information for each game they played

raw data b. lakers_2022_stats.csv - contains all Lakers 2022-23 Game Logs

data/processed - contains cleaned data and 1 jupyter notebook

File a. clean_data.ipynb - This is a jupyter notebook that reads/opens the raw data from the Data/Raw folder and cleans it for later analysis. This file uses the pandas and json libraries. Since the data is in another subfolder within the same folder, the path to read/open these files is "../raw/lakergames2022.json" and "../raw/lakers_2022_stats.csv". It creates two new csv files that is stored into this subfolder. Run this file using 'Run All'

processed data a. clean_lakers_games.csv - cleaned up data from 'lakergames2022.json'

processed data b. clean_lakers_stats.csv - cleaned up data from 'lakers_2022_stats.csv'

**analysis and visuals** - contains jupyter notebook for analysis and visualization

File a. run_analysis_and_visualize_results.ipynb - This is a jupyter notebook that reads the 2 processed csv files and opens them as 2 pandas dataframes and also merges them. This file uses the pandas, numpy, seaborn, and matplotlib.pyplot libraries. Since the data we want to read is in the data/processed folder, the path to read the csv files is '../data/processed/clean_lakers_stats.csv' and '../data/processed/clean_lakers_games.csv'. This is where the data will be analyzed and visualized. Run this file using 'Run All'.
results
