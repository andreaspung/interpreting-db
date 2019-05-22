# interpreting-db

This is the Python code used in my Bachelor's Thesis "[Interpreting a Convolutional Text Classification Neural Network on a Clinical Dataset](https://comserv.cs.ut.ee/ati_thesis/datasheet.php?id=66544&year=2019)". The main Jupyter notebook file is based on Ben Trevett's [PyTorch sentiment analysis tutorial](https://github.com/bentrevett/pytorch-sentiment-analysis). The base code of the interpretation methods was given by my supervisor. The [DementiaBank](https://dementia.talkbank.org/) dataset is used in this analysis which cannot be shared publically.

## Abstract

In this Bachelor’s Thesis, a convolutional text classification neural network is interpreted to find out why the neural network makes such predictions. To perform the analysis, the clinical DementiaBank dataset was used in which people with Alzheimer’s disease describe the Boston cookie theft image. The task of the binary classification was to identify based on the given text whether a person has Alzheimer’s or not. Interpretation methods described in [Jacovi et al. (2018)](https://arxiv.org/abs/1809.08037) were implemented. In addition to that, concrete examples of texts are interpreted in this thesis. Out of all the analyses performed, informative and uninformative ngrams and slot activation vectors with their clustering yield good results. Negative ngrams analysis results were substandard because of the specificity of the dataset.

## Running the notebook

Open Anaconda prompt as an administrator from this project's root directory. Run the following commands:

`conda create --name interpreting-db --file env.txt` (64-bit Windows environment file)

`activate interpreting-db`

`python -m spacy download en` 

`jupyter notebook`

from Jupyter notebook's user interface, you can just click on `interpreting-db.ipynb` file to open it.
