# ASD Severity Estimation Using Functional Connectivity (ABIDE)

This project explores the modeling of Autism Spectrum Disorder (ASD) severity using functional connectivity features from the ABIDE neuroimaging dataset. Rather than treating ASD as a binary condition, the goal is to predict continuous severity scores through regression, interpret feature importance, and link model behavior to known neurobiological networks.

## Project Overview
- Works with high-dimensional resting-state fMRI connectome data  
- Treats ASD severity as a regression task instead of binary classification  
- Implements multiple feature selection methods to reduce dimensionality  
- Evaluates classical ML models and compact deep learning architectures  
- Uses interpretability tools (e.g., SHAP, gradient-based saliency) to validate neurobiological relevance  

## Methodology (Current Prototype)
- Extraction of functional connectivity matrices (20,000+ features per subject)  
- Comparative feature selection: PCA, RFE, ReliefF, SelectKBest, μ-Relief  
- Model benchmarking: SVM, XGBoost, Random Forest, Logistic Regression, DNNs  
- Mapping influential features back to cortical and subcortical regions  
- Alignment of model attention with known ASD-related networks (DMN, salience, frontoparietal)  

## Current Status
The core regression pipeline, feature selection experiments, and interpretability analyses are implemented in Python. Work is ongoing to refine model stability, enhance biological consistency, and improve generalization under limited data.

## Planned Enhancements
- More robust cross-validation and nested CV for high-dimensional regimes  
- Investigation of non-linear feature extraction and graph-based embeddings  
- Integration of multimodal behavioral or clinical measures  
- Exploration of lightweight deep architectures for improved performance  
- Better visualization tools for connectome-level interpretability  

## Motivation
This project is part of a broader effort to rethink how neurodevelopmental conditions like ASD are modeled. By moving beyond binary labels and incorporating interpretability, the aim is to produce computational tools that reflect the spectrum-like nature of ASD and support more informed clinical research.

## License
MIT License

