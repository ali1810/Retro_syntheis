Retrosynthesis Reaction Prediction with SMILES Augmentation
This repo details experiments on predicting retrosynthesis reactants from products using neural machine translation and SMILES based data augmentation.

Overview and Results
We trained a transformer sequence to sequence model for retrosynthesis reactant prediction and experimented with the effect of SMILES based augmentation. We find that SMILES based augmentation increases Top 1 accuracy, but can lead to a decrease in Top K accuracy due to the model predicting different SMILES variants of the same molecule. These are results on the USPTO_50k benchmark retrosynthesis dataset relative to published results by Liu et al and Lin et al. For a full description of the problem, data representation, SMILES augmentation, model implementation and results analysis.



