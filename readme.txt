Retrosynthesis Reaction Prediction with SMILES Augmentation
This repo details experiments on predicting retrosynthesis reactants from products using neural machine translation and SMILES based data augmentation.

Overview and Results
We trained a transformer sequence to sequence model for retrosynthesis reactant prediction and experimented with the effect of SMILES based augmentation. We find that SMILES based augmentation increases Top 1 accuracy, but can lead to a decrease in Top K accuracy due to the model predicting different SMILES variants of the same molecule. These are results on the USPTO_50k benchmark retrosynthesis dataset relative to published results by Liu et al and Lin et al. For a full description of the problem, data representation, SMILES augmentation, model implementation and results analysis, see the full document below.



Model	            Top-1 Accuracy	Top-3 Accuracy	Top-5 Accuracy	Top-10 Accuracy
Liu et al	            37.4	           52.4	              57	              61.7
Lin et al	            54.6	           74.8	              80.2	            84.9
No Augmentation	      53.7	           67.7	              71.2	            73.9
4x Augmentation	      56.0	           67.6	              72.3	            76.5
16x Augmentation	    61.3             70.9	              74.2	            76.4
40x Augmentation	    62.1	           64.1              	65.0	            66.4
