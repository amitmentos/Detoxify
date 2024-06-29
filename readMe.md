```markdown
# Detoxify Data Analysis

This repository contains data and analysis related to toxic language detection, organized into four main directories: `1000-All`, `400-train`, `600-test`, and `nonToxic`. The `1000-All` directory combines training and test data, while the `400-train` and `600-test` directories contain separate data for training and testing, respectively. The `nonToxic` directory contains data and analysis related to non-toxic language. All analyses are divided by languages.

## Directory Structure

```plaintext
.
├── 1000-All
│   ├── all prompt output
│   │   ├── AM-analyze-final.csv
│   │   ├── AR-analyze-final.csv
│   │   ├── DE-analyze-final.csv
│   │   ├── EN-analyze-final.csv
│   │   ├── ES-analyze-final.csv
│   │   ├── HI-analyze-final.csv
│   │   ├── RU-analyze-final.csv
│   │   ├── UK-analyze-final.csv
│   │   └── ZH-analyze-final.csv
│   ├── clustering files
│   │   ├── AM-analyze-cluster.csv
│   │   ├── AR-analyze-cluster.csv
│   │   ├── DE-analyze-cluster.csv
│   │   ├── EN-analyze-cluster.csv
│   │   ├── ES-analyze-cluster.csv
│   │   ├── HI-analyze-cluster.csv
│   │   ├── RU-analyze-cluster.csv
│   │   ├── UK-analyze-cluster.csv
│   │   └── ZH-analyze-cluster.csv
│   ├── extract words
│   │   ├── unique_words_AM.csv
│   │   ├── unique_words_AR.csv
│   │   ├── unique_words_DE.csv
│   │   ├── unique_words_EN.csv
│   │   ├── unique_words_ES.csv
│   │   ├── unique_words_HI.csv
│   │   ├── unique_words_RU.csv
│   │   ├── unique_words_UK.csv
│   │   └── unique_words_ZH.csv
│   └── plot all
│       ├── Plot-AM.ipynb
│       ├── Plot-AR.ipynb
│       ├── Plot-DE.ipynb
│       ├── Plot-EN.ipynb
│       ├── Plot-ES.ipynb
│       ├── Plot-HI.ipynb
│       ├── Plot-RU.ipynb
│       ├── Plot-UK.ipynb
│       ├── Plot-ZH.ipynb
│       └── plot-ALL.ipynb
├── 400-train
│   ├── extract words
│   │   ├── unique_words_AM.csv
│   │   ├── unique_words_AR.csv
│   │   ├── unique_words_DE.csv
│   │   ├── unique_words_EN.csv
│   │   ├── unique_words_ES.csv
│   │   ├── unique_words_HI.csv
│   │   ├── unique_words_RU.csv
│   │   ├── unique_words_UK.csv
│   │   └── unique_words_ZH.csv
│   ├── plot train
│   │   ├── Plot-AM.ipynb
│   │   ├── Plot-AR.ipynb
│   │   ├── Plot-DE.ipynb
│   │   ├── Plot-EN.ipynb
│   │   ├── Plot-ES.ipynb
│   │   ├── Plot-HI.ipynb
│   │   ├── Plot-RU.ipynb
│   │   ├── Plot-UK.ipynb
│   │   ├── Plot-ZH.ipynb
│   │   └── plot-ALL.ipynb
│   ├── prompt output
│   │   ├── AM-analyze.csv
│   │   ├── AR-analyze.csv
│   │   ├── DE-analyze.csv
│   │   ├── EN-analyze.csv
│   │   ├── ES-analyze.csv
│   │   ├── HI-analyze.csv
│   │   ├── RU-analyze.csv
│   │   ├── UK-analyze.csv
│   │   └── ZH-analyze.csv
│   └── train datasets
│       ├── am-00000-of-00001.parquet
│       ├── ar-00000-of-00001.parquet
│       ├── de-00000-of-00001.parquet
│       ├── en-00000-of-00001.parquet
│       ├── es-00000-of-00001.parquet
│       ├── hi-00000-of-00001.parquet
│       ├── ru-00000-of-00001.parquet
│       ├── uk-00000-of-00001.parquet
│       └── zh-00000-of-00001.parquet
├── 600-test
│   ├── test datasets
│   │   ├── am-00000-of-00001-656e19a6f1cc2383.parquet
│   │   ├── ar-00000-of-00001-2338057ce0eeaf0d.parquet
│   │   ├── de-00000-of-00001-00ccec8d5e81dbf1.parquet
│   │   ├── en-00000-of-00001-c54cbb5edf21dd23.parquet
│   │   ├── es-00000-of-00001-723005ac428f80c9.parquet
│   │   ├── hi-00000-of-00001-35f39f96bd50e4e4.parquet
│   │   ├── ru-00000-of-00001-6818d57069197d03.parquet
│   │   ├── uk-00000-of-00001-86a756a5ad8b3340.parquet
│   │   └── zh-00000-of-00001-21350981874ac4f4.parquet
│   ├── test prompt output
│   │   ├── AM-analyze-test.csv
│   │   ├── AR-analyze-test.csv
│   │   ├── DE-analyze-test.csv
│   │   ├── EN-analyze-test.csv
│   │   ├── ES-analyze-test.csv
│   │   ├── HI-analyze-test.csv
│   │   ├── RU-analyze-test.csv
│   │   ├── UK-analyze-test.csv
│   │   └── ZH-analyze-test.csv
│   └── toxic words
│       ├── AM-toxic.csv
│       ├── AR-toxic.csv
│       ├── DE-toxic.csv
│       ├── EN-toxic.csv
│       ├── ES-toxic.csv
│       ├── HI-toxic.csv
│       ├── RU-toxic.csv
│       ├── UK-toxic.csv
│       └── ZH-toxic.csv
├── nonToxic
│   ├── extract words
│   │   └── EN-analyze-nontoxicWordsList.csv
│   ├── nonToxic dataset
│   │   └── EN-nonToxic.csv
│   ├── plot nonToxic
│   │   └── Plot-EN-nonToxic.ipynb
│   └── prompt output
│       └── EN-analyze-nonToxic.csv
└── readMe.md
```

## Overview

The repository is divided into four main directories:

- **1000-All**: Contains combined data and analysis from both training and test datasets.
  - **all prompt output**: Contains the final analysis CSV files for each language.
  - **clustering files**: Contains clustered analysis CSV files for each language.
  - **extract words**: Contains unique words extracted from the datasets for each language.
  - **plot all**: Contains Jupyter notebooks for plotting and visualizing the analysis.

- **400-train**: Contains data and analysis specific to the training datasets.
  - **extract words**: Contains unique words extracted from the training datasets for each language.
  - **plot train**: Contains Jupyter notebooks for plotting and visualizing the training data analysis.
  - **prompt output**: Contains the analysis CSV files for each language from the training data.
  - **train datasets**: Contains the parquet files for each language used in training.

- **600-test**: Contains data and analysis specific to the test datasets.
  - **test datasets**: Contains the parquet files for each language used in testing.
  - **test prompt output**: Contains the analysis CSV files for each language from the test data.
  - **toxic words**: Contains

 CSV files of toxic words for each language.

- **nonToxic**: Contains data and analysis related to non-toxic language.
  - **extract words**: Contains the list of non-toxic words extracted from the datasets.
  - **nonToxic dataset**: Contains the non-toxic dataset.
  - **plot nonToxic**: Contains Jupyter notebooks for plotting and visualizing the non-toxic data analysis.
  - **prompt output**: Contains the analysis CSV file for non-toxic data.

## Analysis

- **all prompt output**: Contains the analysis results after running prompts through GPT-4.
- **clustering files**: Contains clustered analysis to visualize data points in space using one-hot vectors and clustering algorithms.
- **extract words**: Contains unique words extracted from each column for analysis of their frequencies and occurrences.
- **plot**: Contains visualizations of the analysis, including the top 10 most frequent words in each column (tone, language, sentiment), combined columns, and percentage appearances of words relative to sentence counts. It also includes visualizations of the most offensive words and their frequency, as well as clustering visualizations showing data points colored by cluster, with tooltips displaying words from each column (tone, language, sentiment).

The analyses are divided by language to provide detailed insights into toxic and non-toxic language detection across different linguistic contexts.
```