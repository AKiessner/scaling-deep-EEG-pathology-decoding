# scaling-deep-EEG-pathology-decoding

This repository contains resources that were used for our study entitled

"Kiessner, A. K., Schirrmeister, R. T., Boedecker, J., & Ball, T. (2024). Reaching the ceiling? Empirical scaling behaviour for deep EEG pathology classification. Computers in Biology and Medicine, 178, 108681.". [PDF](https://doi.org/10.1016/j.compbiomed.2024.108681)

## Contents

Temple University Hospital (TUH) Abnormal EEG Corpus (TUAB):

TUAB train/test split as provided by the TUH.

TUH Abnormal Expansion Balanced EEG Corpus (TUABEXB):

TUABEXB train/test as described in Kiessner, A. K., Schirrmeister, R. T., Gemein, L. A., Boedecker, J., & Ball, T. (2023). An extended clinical EEG dataset with 15,300 automatically labelled recordings for pathology decoding. NeuroImage: Clinical, 39, 103482.



TUABCOMB: Union of TUAB train set and TUABEXB train set

- dataset_description/ - description of all datasets and train/test data splits. Each description contains the path of the recordings used and pathology labels based on automated classification of the medical text reports. 'path_new' refers to the same recording in the current version of the Temple University Hospital EEG Corpus (v2.0.0).

- code/ - Python scripts and notebooks for data loading and training pipeline of the convolutional neural networks.

- indices_smaller_subsets/ - indices to identify the recordings for each of the randomly selected smaller subsets of each training dataset based in the description file.

- results_csv / contains the decoding accuracies of all runs and experiments

## Environments

This repository expects a working installation of [braindecode](https://github.com/braindecode/braindecode).  
Additionally, it requires to install packages listed in `environment.yml`. So download the reposiory and create the environment from the environment.yml file::

```
conda env create -f environment.yml
```



## Data

Our study is based on the Temple University Hospital Abnormal EEG Corpus (v2.0.0) and Temple University Hospital EEG Corpus (v1.1.0 and v1.2.0) avilable for download at: https://www.isip.piconepress.com/projects/tuh_eeg/html/downloads.shtml. We also provide an updated version of the dataset descriptions based on the Temple University Hospital EEG Corpus (v2.0.0) and the Temple University Hospital Abnormal EEG Corpus (v3.0.0) .

Our study is based on the TUH Abnormal EEG Corpus (v2.0.0) and the TUH Abnormal Expansion Balanced EEG Corpus (TUABEXB). The TUABEXB is based on the TUH EEG Corpus (v1.1.0 and v1.2.0).
Please note that the current version of the data is the TUH Abnormal EEG Corpus (v3.0.0) and the TUH EEG Corpus (2.0.0).
Updates include the removal of medical reports and the restructuring of the Unix-style hierarchical file tree structure. 
We have updated the record description of the TUABEXB to be compatible with the current version of the TUEG and TUAB.
The corresponding pathology labels for the TUH Abnormal Expansion Balanced EEG Corpus are available for download at \url{github.com/AKiessner/TUHAbnormal-Expansion-dataset}. The descriptions of the dataset variants used in this paper include the path of the recording within the TUEG and the associated labels for EEG pathology.




## Citing

If you use this code in a scientific publication, please cite us as:
```
Kiessner, A. K., Schirrmeister, R. T., Boedecker, J., & Ball, T. (2024). Reaching the ceiling? Empirical scaling behaviour for deep EEG pathology classification. Computers in Biology and Medicine, 178, 108681.
```
```
@article{KIESSNER2024Scaling,
title = {Reaching the ceiling? Empirical scaling behaviour for deep EEG pathology classification},
journal = {Computers in Biology and Medicine},
volume = {178},
pages = {108681},
year = {2024},
issn = {0010-4825},
doi = {https://doi.org/10.1016/j.compbiomed.2024.108681},
url = {https://www.sciencedirect.com/science/article/pii/S0010482524007662},
author = {Ann-Kathrin Kiessner and Robin T. Schirrmeister and Joschka Boedecker and Tonio Ball},
}

```
