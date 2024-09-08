# protein-structure-prediction-with-ESMFold

**ESMFold** (https://www.biorxiv.org/content/10.1101/2022.07.20.500902v2) is a powerful tool in protein structure prediction, leveraging advanced deep learning techniques to predict the three-dimensional structures of proteins from their amino acid sequences. It is built on a 15 billion parameter Transformer language model called ESM-2 that learns the statistical patterns in protein sequences to infer their folded structures. It uses a learned language model(also known as LLM) representation that requires only the amino acid sequence as input, unlike other methods like AlphaFold2 which need additional databases.

ESMFold works by first encoding the input protein sequence using the ESM-2 language model, which learns representations capturing structural information. These representations are then fed into a downstream component similar to AlphaFold2 that predicts the 3D coordinates of the atoms in the folded structure.

ESMFold was trained using a large dataset of protein sequences from the UniRef90 database. All PDB chains until May 1, 2020 with resolution greater than 2Å were used as the training set, providing a diverse set of high-quality protein structures
