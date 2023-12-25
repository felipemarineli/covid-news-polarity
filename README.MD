# Covid-19 Pandemic and Polarity in Editorial News: A BBC case study

This project seeks to understand whether there is a relationship between the Covid-19 pandemic in the United Kingdom (through the official metrics) and the `polarity` (a feature offered by the SpaCy library in order to determine the positivity or negativity of a statement) of the editorial news from the British Broadcasting Corporation (BBC). Our null hypothesis states that there is no relationship. A sitemap web crawler is employed in other to collect data from the BBC archive, which is then processed using the `spaCy` library. We perform significance tests (t-tests) using the extracted polarity (by date) and various pandemic metrics, such as new infections and daily vaccinations.


### Prerequisites

- [Python 3.8.2](https://www.python.org/downloads/release/python-382/)
- [Anaconda](https://www.anaconda.com/products/individual)

### Installing

Make sure conda-forge is in your list of Anaconda channels

```
conda config --append channels conda-forge
```

Create a new Anaconda environment from requirements.txt
```
conda create --name data_programming --file requirements.txt
```

Activate the environment
```
conda activate data_programming
```

Instal spaCyTextBlob using pip
```
pip install spacytextblob
```

Download data for TextBlob
```
python -m textblob.download_corpora
```

Download spaCy model for English
```
python -m spacy download en_core_web_sm
```

### Usage:

Launch the application and follow the instruction in the notebook
```
jupyter notebook
```
