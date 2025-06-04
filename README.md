# D4: Deep Drug-Drug Interaction Discovery and Demystification

D4 is a novel method for predicting drug-drug interactions along with their mechanisms of interaction. It uses 11 different mechanisms  at the pharmacokinetic, pharmacodynamic, multi-pathway, and pharmacogenetic levels. D4 utilizes neuro-symbolic deep learning strategies to encode background knowledge about basic biological processes and phenomena about drugs. 

This repository contains scripts which were used to build a supervised artificial neural network model, an optimization of the artificial neural network model using hypers, along with the script for drawing AUCs for evaluating the model's performance.

# Dependencies
To install python dependencies run: pip install -r requirements.txt

# Scripts
The scripts require embedding files, which can be found: https://bio2vec.cbrc.kaust.edu.sa/data/D4/embeddings/

- Hypers.py: This scripts requires 2 inputs file: 1) the embedding; and 2) the DDIs file representing each drug as a vector. 
- ANNmodel.py: This scripts requires 2 inputs file: 1) the embedding; and 2) the DDIs file representing each drug as a vector. The scripts comes after Hypers.py to use the best hyperparameters.
- AUC.py: This scripts requires 1 input file that is the.pckl file to drew the AUC curve. 

# Data
- D4 predictions of novel DDIs can be found at: https://bio2vec.cbrc.kaust.edu.sa/data/D4/predictions/
- D4 embeddings of all drugs can be found at: https://bio2vec.cbrc.kaust.edu.sa/data/D4/embeddings/

# Citation
In case of using our scripts, datasets, or predictions, please cite our work: Noor, A., Liu-Wei, W., Barnawi, A., Nour, R., Assiri, A. A., Chan Bukhari, S. A., & Hoehndorf, R. (2020). D4: deep drug-drug interaction discovery and demystification. bioRxiv, 2020-04
