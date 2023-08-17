# Canada_Political_Analysis

## Table of Contents

- [Description](#description)
- [Questions Answered](#questions-answered)
- [Project Structure](#project-structure)
- [Requirements](#requirements)
- [Usage](#usage)

## Questions Answered

This project aims to answer the following questions:

1. What are the main topics discussed between 1900 and 1939?
2. What topics are the Prime Minister and the opposition talking about?
3. Is there a correlation between electoral performance and the most frequently discussed topic of each Parliamentarian?

## Project Structure

The project is structured as follows:

- `analysis` folder: Contains Jupyter notebooks and data files.
  - `main.ipynb`: Main Jupyter notebook containing the analysis code.
  - `helper.ipynb`: Helper Jupyter notebook for web scraping.
  - `speeches` folder: Supposed to contain individual CSV files for each year's speeches, unfortunately all csv folders are nearly 5gb, so please add all the csv's 1900-2010 manually to here.
  - `cleaned_df_nlp.csv`: Preprocessed speech data with cleaned text for NLP.
  - `removed_stopwords.csv`: Speech data with stopwords removed.
  - `sampled_df.csv`: Sampled speech data for sentiment analysis.
  - `frequency_df.csv`: Frequency of most used words in speech data.
  - `electoral_data.csv`: Electoral data coming from webscrapping

## Requirements

Make sure you have the following dependencies installed:

- Python (>=3.6)
- Jupyter Notebook
- pandas
- seaborn
- matplotlib
- tqdm
- nltk
- selenium
- chromedriver (for web scraping)

You can install the required packages using the following command:

pip install pandas seaborn matplotlib tqdm nltk selenium

Additionally, you need to download the NLTK stopwords and punkt tokenizer resources. In a Python environment, run the following commands:

```python
import nltk
nltk.download('stopwords')
nltk.download('punkt')
```

## Usage

Run the Jupyter notebooks in the analysis folder:

- `main.ipynb`: Analysis code for answering the questions.
- `helper.ipynb`: Web scraping helper code (if needed). For Question 3, this workbook needs to be run to collect electoral data.

Make sure you have the necessary CSV files in the project directory.

Modify the paths in the code to match your directory structure if needed.

Run the notebooks cell by cell to perform the analysis.
