# Persian SnappFood Review Sentiment Analysis

## Overview

This project analyses Persian customer reviews from SnappFood to identify the
words and two-word phrases most strongly associated with positive (`HAPPY`)
and negative (`SAD`) comments.

The project focuses on descriptive text analysis rather than sentiment
prediction. It examines word frequency, statistical association, phrase
context, and differences in comment length between the two sentiment groups.

## Research Question

Which Persian words and two-word phrases are most strongly associated with
positive and negative SnappFood reviews?

## Dataset

The dataset contains 70,000 Persian SnappFood customer comments with the
following columns:

- `comment`: the original Persian review
- `label`: sentiment label (`HAPPY` or `SAD`)
- `label_id`: numerical sentiment label (`0` or `1`)

Although the file has a `.csv` extension, its columns are separated by tab
characters. Therefore, it is loaded with:

```python
pd.read_csv(DATA_PATH, sep="\t")

Download the SnappFood Persian Sentiment Analysis dataset from Kaggle.

Place the CSV file here with the following name:

snappfood_comments.csv


And:

````markdown
Install the libraries with:

```bash
pip install -r requirements.txt
```