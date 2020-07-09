# private_nlp
Natural Language Processing models using private and secure data. Powered by OpenMined's tools [PySyft](https://github.com/OpenMined/PySyft) and [SyferText](https://github.com/OpenMined/SyferText).

## blog post
The contents of this repo were featured in a [blog post](https://blog.openmined.org/encrypted-training-medical-text-syfertext/) at [OpenMined's blog](https://blog.openmined.org/)

## Disclaimer
This is an ongoing work in progress. Be prepared to tackle coding errors and/or typos.

## Getting Started
Follow the instructions to install:
- [PySyft](https://github.com/OpenMined/PySyft)==0.2.5. There is an incompatibility issue with Tensorflow on version 0.2.6
- [SyferText](https://github.com/OpenMined/SyferText)

## Data
Dataset compiled for Natural Language Processing using a corpus of medical transcriptions and custom-generated clinical stop words and vocabulary.

- [`X.csv`](https://github.com/socd06/private_nlp/blob/master/data/X.csv). Fully processed dataset obtained from running the [Data Modelling](https://github.com/socd06/private_nlp/blob/master/notebooks/medical-text-data-modelling.ipynb) notebook.
- [`classes.txt`](https://github.com/socd06/private_nlp/blob/master/data/classes.txt). Text file describing the dataset's classes: `Surgery`, `Medical Records`, `Internal Medicine` and `Other`
- [`train.csv`](https://github.com/socd06/private_nlp/blob/master/data/train.csv). Training data subset. Contains 90% of the `X.csv` processed file.
- [`test.csv`](https://github.com/socd06/private_nlp/blob/master/data/test.csv). Test data subset. Contains 10% of the `X.csv` processed file.

### Authors and acknowledgment
- `mtsamples.csv`. Compiled from Kaggle's medical transcriptions dataset by [Tara Boyle](https://github.com/terrah27), scraped from [Transcribed Medical Transcription Sample Reports and Examples](https://www.mtsamples.com/). See [Kaggle repository](https://www.kaggle.com/tboyle10/medicaltranscriptions#mtsamples.csv).

- `clinical-stopwords.txt`. Compiled from [Dr. Kavita Ganesan](https://github.com/kavgan) [clinical-concepts](https://github.com/kavgan/clinical-concepts) repository. See the [Discovering Related Clinical Concepts Using Large Amounts of Clinical Notes
](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5015701/) paper.

- `vocab.txt`. Generated vocabulary text files for Natural Language Processing (NLP) using the [Systematized Nomenclature of Medicine International (SNMI) data](https://bioportal.bioontology.org/ontologies/SNMI). See how to [Generate your own vocab file](https://github.com/socd06/snmi_vocab/blob/master/notebooks/snmi_vocab.ipynb).

## Notebooks
- [Data Modelling](https://github.com/socd06/private_nlp/blob/master/notebooks/medical-text-data-modelling.ipynb): Data exploration and feature engineering using Pandas, matplotlib and Seaborn and consolidation of dataset using scikit-learn.

- [Medical text data exploration](https://github.com/socd06/private_nlp/blob/master/notebooks/medical-text-data-exploration.ipynb): An introduction to data exploration of medical text using Pandas, matplotlib and Seaborn. **NOTE**: Deprecated. See [Data Modelling](https://github.com/socd06/private_nlp/blob/master/notebooks/medical-text-data-modelling.ipynb) instead.

- [Medical text encrypted training](https://github.com/socd06/private_nlp/blob/master/notebooks/medical-text-encrypted-training.ipynb): Tutorial on how to train an NLP model of data you cannot see using [PySyft](https://github.com/OpenMined/PySyft) and [SyferText](https://github.com/OpenMined/SyferText). Heavily inspired by [Alan Aboudib's](https://twitter.com/alan_aboudib) [Sentiment classification using SyferText use case](https://github.com/OpenMined/SyferText/blob/master/tutorials/usecases/UC01%20-%20Sentiment%20Classifier%20-%20Private%20Datasets%20-%20(Secure%20Training).ipynb). **WARNING**: This is an ongoing project, be wary of errors.

## Scripts
Holds the script used to download whole datasets using url

## Contributing
Issues and Pull requests welcomed

# License
[GNU GENERAL PUBLIC LICENSE VERSION 3](https://github.com/socd06/medical-nlp/blob/master/LICENSE)
