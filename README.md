## Brain Network Analysis for Early Detection of Alzhiemer's Disease

Project led and maintained by [Rajas Gupta](https://github.com/rajasg) and Vijay Sharma

Contributors:
[Omkar Yadav](https://github.com/omkar-yadav-12), [Brandon Xu](https://github.com/brx021)

# Introduction 
Alzheimer's Disease (AD) is a neurodegenerative disorder of uncertain cause and pathogenesis that primarily affects older adults and is the most common cause of dementia. We sought to apply machine learning to AD classification on brain imaging. Brain Imaging via magnetic resonance imaging (MRI), is used for evaluation of patients with suspected AD. MRI findings include both local and generalized shrinkage of brain tissue. Some studies have suggested that MRI features may predict the rate of decline of AD and may guide therapy in the future. Specifically, we trained our model with white matter maps from the OASIS AD dataset. White matter maps measure the density of which messages pass between different areas in the central nervous system.

* data_preprocessing.ipynb selects our sample from the OASIS dataset. We seperated patients into AD and TD, while trying to make the demographics as uniform as possible. 
* network_extraction.ipynb processes the MRI data and performs the analysis and classification of our dataset.
* oasis_cross-sectional.csv contains patient information for the dataset.
* patient_ids.csv contains the patient ids for our selected dataset.

# Dependencies
* python 3.7.13
* nilearn 0.9.1
* sklearn 1.0.2

# Results
We found strong evidence that white matter maps can be used to differentiate between AD and control brains. We found that our model attained a mean accuracy score of 0.8145 on a five fold cross-validation. The dataset consisted of 53 samples, 27 were control while 26 were AD.
