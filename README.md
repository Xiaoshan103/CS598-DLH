## Statistical-supervised-meta-ensemble-algorithm-for-medical-record-linkage

This repository is the official implementation of [Statistical-supervised-meta-ensemble-algorithm-for-medical-record-linkage](https://github.com/ePBRN/Medical-Record-Linkage-Ensemble). 

## Requirements

To install requirements:

```setup
pip install numpy
pip install pandas
pip install sklearn
pip install recordlinkage
pip install matplotlib
```

+ Download the github repository and use Python 3.6 or higher wto run the code. All the necessary datasets are in the current repository.

## Training and Evaluation

To train and evaluate the model(s) in the paper:

+ run `FEBRL_UNSW_Linkage.ipynb` to reproduce results for FEBRL dataset.

+ run `ePBRN_UNSW_Linkage.ipynb` to reproduce results for ePBRN dataset.

## Results

Our model achieves the following performance on medical record linkage:

### FEBRL dataset

| Model name         | precision(%)  | recall(%) | f1-score(%) | false counts |
| ------------------ |---------------- | -------------- | -------------- | -------------- |
| Support Vector Machine                |     94.28         |      99.73       |      96.93        |      309       |
| Support Vector Machine with Bagging   |     94.94         |      99.73       |      97.28        |      273      |
| Neural Network                        |     93.25         |      99.43       |      96.24        |      387       |
| Neural Network with Bagging           |     93.14         |      99.37       |      96.15       |      389       |
| Linear Regression                     |     93.01         |      99.57       |      96.18       |      380       |
| Linear Regression with Bagging        |     93.03         |      99.51       |      96.16       |      389       |
| Stacking & Bagging                    |     96.54         |      99.22       |      97.86       |      212       |

+ check out our report to see more results
