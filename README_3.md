# Descriptive Statistics Primer – Titanic Dataset

**Task 9 – Descriptive Statistics Primer**
Veda Technology | Data Analytics Track | Level 1, Day 9

## About
I calculated the main descriptive statistics (mean, median, mode, standard deviation, percentiles and skew) for four numeric columns of the Titanic dataset using Python and Pandas. I used the raw data (891 passengers) and let Pandas skip the missing ages.

## Summary statistics table
| Column | Count | Mean | Median | Mode | Std | Min | 25% | 75% | Max | Skew |
|--------|-------|------|--------|------|-----|-----|-----|-----|-----|------|
| Age | 714 | 29.70 | 28.00 | 24 | 14.53 | 0.42 | 20.1 | 38.0 | 80.0 | 0.39 |
| Fare | 891 | 32.20 | 14.45 | 8.05 | 49.69 | 0.00 | 7.91 | 31.00 | 512.33 | 4.79 |
| SibSp | 891 | 0.52 | 0 | 0 | 1.10 | 0 | 0 | 1 | 8 | 3.70 |
| Parch | 891 | 0.38 | 0 | 0 | 0.81 | 0 | 0 | 0 | 6 | 2.75 |

## What the numbers reveal about skew and spread
**Age** is fairly symmetrical. The mean (29.7) is very close to the median (28), and the skew is small (0.39). The standard deviation is 14.5 years, so passengers' ages are spread widely, but the middle 50% are between about 20 and 38 years old.

**Fare** is strongly right-skewed. The mean (32.2) is more than double the median (14.45), and the skew is 4.79. A few very expensive tickets (the maximum is 512.33) pull the mean up. The standard deviation (49.7) is larger than the mean, which means fares vary a lot. The median describes a typical passenger better than the mean.

**SibSp and Parch** are also right-skewed, but for a different reason. Most passengers travelled without siblings, spouses, parents or children, so the median and mode are both 0, while a few large families push the mean and the maximum up. For counts like these, the median and mode tell more than the mean.

**Main takeaway:** always compare the mean with the median to spot skew, and read the standard deviation together with the mean. The Fare column shows why: the mean alone would give a wrong idea of what a typical passenger paid.

## Files
- `Descriptive_Statistics_Titanic.ipynb` – notebook with the code and output
- `summary_statistics.csv` – the summary table
- `fare_age_histograms.png` – histograms of Age and Fare
- `README.md`

## Tools used
Python, Pandas, Matplotlib (Google Colab)

## Author
Rabia
