# scaling-deep-EEG-pathology-decoding

This repository contains resources that were used for our study entitled

"XXXXX".

## Contents

Temple University Hospital (TUH) Abnormal EEG Corpus (TUAB):

TUAB train/test split as provided by the TUH.

TUH Abnormal Expansion Balanced EEG Corpus (TUABEXB):

TUABEXB train/test as described in Kiessnerk et al. (2023)



TUABCOMB: Union of TUAB-R train set and TUABEXB-R train set

- dataset_description/ - description of all datasets and train/test data splits. Each description contains the path of the recordings used and pathology labels based on automated classification of the medical text reports. 'path_new' refers to the same recording in the current version of the Temple University Hospital EEG Corpus (v2.0.0).

- code/ - Python scripts and notebooks for processing of the text files and training pipeline of the convolutional neural networks.

- indices/ - indices to identify the recordings for each of the randomly selected smaller subsets of each training dataset based in the description file.

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


```
