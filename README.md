# DLH_Cervical_Cancer_Local_Explanations

## Documents
Main notebook can be found at: [DL4H_Team_94.ipynb](https://github.com/QinxiW/DLH_Cervical_Cancer_Local_Explanations/blob/main/%5BProj_Final_Report%5D_DL4H_Team_94.ipynb)

## Specification of dependencies
To run the notebook please use Python 3.10, pip packages included at [requirement.txt](https://github.com/QinxiW/DLH_Cervical_Cancer_Local_Explanations/blob/main/requirements.txt)

## Running the code
We recommend that you run the notebook in top-down order, execute each previous code block before the next.
The one part you can skip is the local explanation generation for the 5 models under 'Explainability results' section, 
this is the most computation intensive chunk of all the operations. We saved the local explainability results generated using
the methods in the original pape, and in the notebook we provided code to load them again in the 'Analyses' subsection under 'Results'. 

-------------------------------------------------------------------------
## Table of contents of the main notebook
### Introduction
Present the general problem and specific approach in the original paper
### Methodology
#### Environment
package installations and setup
#### Data
The dataset used in the paper is available from the UCI repository (Fernandes et al., 2017). It is open source, and available on Kaggle for download directly. We kept a copy of the data in the /data directory.
Load and process dataset, including analysis, visualization, and train/test split.
#### Model
Define the 5 model architecturesZ that have widely been used in prior literature for cervical cancer risk assessment
#### Training
Training the 5 models, hyperparams and computation requirement discussions
#### Evaluation
Metrics descriptions, evaluation the 5 models
### Results
Model eval and empirical study result on local explanation techniques
#### Explainability results
Generate local explanations for each trained model (you can skip the local explanation methods in each of the model and load it back into memory here
##### Feature importance and local explanation methods generation
Examine feature importances in the models, and generate local explanations including SHAP, TreeSHAP, LIME, DICE and other related interpretability methods
##### Ablation Study
Remove features one at a time and compare model performance
#### Analyses of explainability
Faithfulness, Contribution, Consistency, Compactness, Stability, Feature and Rank disagreement
### Discussions
Discuss the implications of the hypothesis and results from the original paper along with our reproduced results
Retro on what went well vs difficult, along with suggestions for improving reproducibility
### References
citation of the original paper