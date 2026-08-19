# ImmunoDefender Dataset

This repository contains the cleaned datasets used in the experiments
reported in the research article:

**ImmunoDefender: A Bio-Inspired Multi-Layer System for Detecting
Social Engineering Attacks**

The repository contains two independent datasets:

- `phishing_cleaned.csv` — phishing and legitimate email messages
- `smishing_cleaned.csv` — smishing and legitimate SMS messages

The datasets provided here are the **cleaned and standardized versions**
used in the ImmunoDefender experiments. They are derived from multiple
publicly available third-party sources.

---

## Dataset Overview

| Dataset | Original Sources | Final Samples |
|---|---|---:|
| Phishing | MillerSmiles + Enron Email Dataset | 57,080 |
| Smishing | Mendeley Data + SmishTank + Combined Labeled Smishing Dataset | 76,798 |

---

## 1. Phishing Dataset

The phishing corpus was constructed by combining phishing reports
collected from the MillerSmiles repository with legitimate email
communications from the Enron Email Dataset.

The MillerSmiles source consists of real-world phishing and social
engineering reports collected from individual web pages. The required
information was extracted and standardized using an automated data
collection pipeline.

The Enron Email Dataset was used as the legitimate (ham) email source.

The two corpora were standardized to a common schema and subsequently
merged.

The original integrated corpus contained:

- 23,364 phishing emails
- 33,716 legitimate emails
- 57,080 emails in total

The dataset was subsequently subjected to the preprocessing procedures
described in the associated research article.

### Original Sources

1. **MillerSmiles — Phishing and Spoof Email Archive**

   https://millersmiles.co.uk/

   MillerSmiles maintains an archive of phishing and identity-theft
   email scam reports.

2. **Enron Email Dataset**

   Cohen, W. W. (2015). *Enron Email Dataset*. Carnegie Mellon University.

   https://www.cs.cmu.edu/~enron/

   The dataset was originally released in connection with the Federal
   Energy Regulatory Commission investigation of Enron.

---

## 2. Smishing Dataset

The smishing corpus was constructed by aggregating multiple publicly
available SMS phishing sources:

- Mendeley Data SMS phishing dataset
- SmishTank real-world smishing reports
- Combined Labeled Smishing Dataset

The original merged corpus contained 96,116 SMS messages.

After removing duplicate records, incomplete records, inconsistent
labels, and other invalid entries, the resulting cleaned corpus
contained:

**76,798 SMS messages.**

The final dataset was standardized to the following structure:

```text
Label, Text

Original Sources

Mishra, S., & Soni, D. (2022).
SMS PHISHING DATASET FOR MACHINE LEARNING AND PATTERN RECOGNITION.

Mendeley Data, Version 1.

DOI: 10.17632/f45bkkt8pr.1

Munoz, M., & Islam, M. (2025).
A Balanced Dataset for Spam and Smishing Detection using Large
Language Models (LLMs).

Mendeley Data, Version 1.

DOI: 10.17632/vmg875v4xs.1

SmishTank

Real-world smishing reports collected from the SmishTank source.

Combined Labeled Smishing Dataset

Publicly available GitHub dataset used as one of the sources for
constructing the unified smishing corpus.

Data Processing

The original datasets were not used directly.

The following preprocessing operations were applied where applicable:

Removal of duplicate records
Removal of records with missing or invalid labels
Removal of unusable records
Text normalization
Label normalization
Schema standardization
Integration of heterogeneous sources
Final consistency checks

The resulting datasets correspond to the data used in the
ImmunoDefender experiments.

Attribution and Licensing

The datasets in this repository are derived from third-party
datasets and publicly available sources.

The original datasets remain subject to their respective licenses,
terms of use, and attribution requirements.

This repository does not claim ownership of the underlying
third-party data and does not relicense those original datasets.

Users who access or use the datasets provided here are responsible
for complying with the licensing conditions and attribution
requirements of the original sources.

Where a source requires attribution, the original authors and/or
dataset providers must be appropriately cited.

For research and academic use, please cite both the original datasets
and the ImmunoDefender research article.
