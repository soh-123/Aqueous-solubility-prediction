# Aqueous-solubility-prediction
Predicting how well a drug dissolves in water is not easy and here comes SolTranNet which is a  ML tool to predict aqueous solubility from a molecule’s SMILES representation.It's pretty accurate, with a low error rate in its predictions on two different sets of data.

## Identifiers
EOS model ID: `eos6oli`

Slug: `soltrannet-aqueous-solubility`

## Repository organisation
The repository is organised in folders:

- '/notebooks' contains the jupyter notebooks where most of the work is being developed
- '/data' contains all the .csv files. Model predictions are obtained outside this repository and saved in this folder. Subfolders might be created if needed
- '/src' contains important functions I will re-use throughout the repository, to avoid typing them each time
- '/figures' contains the plots I have produced during the model validation process
- 'requirements.txt' lists all the required packages to run the notebooks in this repository. If possible I also specify the version of the package I am using.

## Model Check
### 1. Model Bias Check
The scatter plot does not show clear signs of bias in the model's predictions in terms of systematic errors. The predictions are varied and do not exhibit a consistent pattern of over- or under-predicting solubility based on the molecule's ID in the dataset,  it's a positive indication that SolTranNet is a robust model for predicting aqueous solubility.
![Model Bias](./figures/Model%20Bias.png)
## License
All the code in this repository is licensed under a GPLv3 License.