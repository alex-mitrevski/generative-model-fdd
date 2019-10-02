# generative-model-fdd

Accompanying code for our paper

A. Mitrevski and P. G. Plöger, “Data-Driven Robot Fault Detection and Diagnosis Using Generative Models: A Modified SFDD Algorithm,” in *30th International Workshop on Principles of Diagnosis (DX)*, Klagenfurt, Austria, 2019.

## Short description

The repository includes:
* `black_box_data`: Data collected from a ROPOD platform using the black box data logger at https://github.com/ropod-project/black-box (both nominal and faulty data). The subdirectories of `black_box_data` contain descriptions of the conditions under which the data were collected as well as descriptions of the recorded data items
* `sw_faults_current.ipynb`: Illustrates the anomaly detection procedure using a restricted Boltzmann machine (RBM) as described in the paper. The notebook includes our implementation (a very naive, non-optimised version) of a deep belief network, the procedure for training correlation dependency models, as well as evaluation on the faulty data
* `sw_faults_current_gmm.ipynb`: This notebook is the same as the previous one, except that the RBM models are replaced by Gaussian Mixture Models (GMMs)

## Requirements

The code in the provided notebooks depends on the packages specified in `requirements.txt`.
