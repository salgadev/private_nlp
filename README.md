# private_nlp
Natural Language Processing models using private and secure data. Powered by OpenMined's tools [PySyft](https://github.com/OpenMined/PySyft) and [SyferText](https://github.com/OpenMined/SyferText).

## Getting Started
Follow the instructions to install:
- [PySyft](https://github.com/OpenMined/PySyft)==0.2.5. There is an incompatibility issue with Tensorflow on version 0.2.6) and
- [SyferText](https://github.com/OpenMined/SyferText)

## Data
Dataset compiled for Natural Language Processing using a corpus of medical transcriptions and custom-generated clinical stop words and vocabulary.

### Authors and acknowledgment
- `mtsamples.csv`. Compiled from Kaggle's medical transcriptions dataset by [Tara Boyle](https://github.com/terrah27), scraped from [Transcribed Medical Transcription Sample Reports and Examples](https://www.mtsamples.com/). See [Kaggle repository](https://www.kaggle.com/tboyle10/medicaltranscriptions#mtsamples.csv).

- `clinical-stopwords.txt`. Compiled from [Dr. Kavita Ganesan](https://github.com/kavgan) [clinical-concepts](https://github.com/kavgan/clinical-concepts) repository. See the [Discovering Related Clinical Concepts Using Large Amounts of Clinical Notes
](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5015701/) paper.

- `vocab.txt`. Generated vocabulary text files for Natural Language Processing (NLP) using the [Systematized Nomenclature of Medicine International (SNMI) data](https://bioportal.bioontology.org/ontologies/SNMI). See how to [Generate your own vocab file](https://github.com/socd06/snmi_vocab/blob/master/notebooks/snmi_vocab.ipynb).

## Notebooks
- [Medical text data exploration](https://github.com/socd06/private_nlp/blob/master/notebooks/medical-text-data-exploration.ipynb): An introduction to data exploration of medical text using Pandas, matplotlib and Seaborn.

- [Medical text encrypted training](https://github.com/socd06/private_nlp/blob/master/notebooks/medical-text-encrypted-training.ipynb): Tutorial on how to train an NLP model of data you cannot see using [PySyft](https://github.com/OpenMined/PySyft) and [SyferText](https://github.com/OpenMined/SyferText). Inspired by [Alan Aboudib's](https://twitter.com/alan_aboudib) [Sentiment classification using SyferText use case](https://github.com/OpenMined/SyferText/blob/master/tutorials/usecases/UC01%20-%20Sentiment%20Classifier%20-%20Private%20Datasets%20-%20(Secure%20Training).ipynb).

## Scripts
Holds the script used to download whole datasets using url

## Contributing
Issues and Pull requests welcomed

# License
[GNU GENERAL PUBLIC LICENSE VERSION 3](https://github.com/socd06/medical-nlp/blob/master/LICENSE)
