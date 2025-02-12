# README

This folder has the scripts used in `Bulla, et al 2025` to generate the UMAPs from the `Alam et. al 2024` dataset.


## Generating path-length distances between clusters of 20 UMAP iterations

-  We used Alam et al's spectograms for 31 birds behind their Fig. 2c provided by the authors at [iso.csv](ADD LINK) and [tut.csv](ADD link)
-  Using **this DATA and that SCRIPT/S LINK ALSO TO THE DATA and SCRIPTS OR FOLDER WITH SCRIPTS** we generate 20 UMAP iterations, while changing no parameters, except the seed for the random number generator.
-  In each of the UMAP iteration, we compute the path length for each bird in the following way: ADD
-  This gives 31*20=620 path lengths (20 per bird).
-  The resulting datasets
1.  `Dat_path_length.csv`
    - is available [here](ADD LINK)
    - contains columns: *bird_id* - unique bird identifier, *iteration* - unique UMAP iteration number, *rseed* - random seed used in the UMAP computation, *n_syll* - syllable countbird_id,iteration,rseed,n_syll columns are clear.
   - is used to compute repeatability and reliability of path-length metric: https://martinbulla.github.io/rebuttal_alam_2024/
2.  `path_length_matrix.npy`
	- Matrix representation of `kdistance` for easy loading into python.

The file X and X provides session info.
