# Biophysical characterisation of ORF6 from SARS-CoV-2

Scripts used to produce figures in Alice Jane Pettitt's thesis. Submitted September 2024 to University College London. 

I used PLUMED version 2.7.1 and GROMACS 2021.2. 

## This repository contains: 

#### Jupyter notebook 
A Jupyter Notebook detailing the analysis performed to reproduce the figures as reported in my thesis is included `ORF6-METADYNAMICS-ANALYSIS.ipynb` and `ORF6-MODEL-SYSTEM-METADYNAMICS-ANALYSIS.ipynb`. The easiest way to try out the notebooks is by using [`conda`](https://www.anaconda.com/products/individual). We include the environment, which specifies the packages needed for the analysis and plotting of the results. To create the environment, run `conda env create -f environment.yml` for Mac and `conda env create -f environment_linux.yml` for Linux operating systems. This can take a hot minute to complete depending on the operating system. Activate the new environment with `conda activate analysis`. 

If the above environments do not work, the following packages are required for running the jupyter notebook:
- Numpy
- SciPy
- Pandas 
- Matplotlib
- Lmfit
- MDTraj
- Seaborn
- SciKit-Learn 

Open the Jupyter notebook with `jupyter lab` and select the notebook from the sidebar. Large data files referenced in the Notebook (including trajectories and metadynamics weights) are hosted on Zenodo [`https://doi.org/10.5281/zenodo.13757998`](https://doi.org/10.5281/zenodo.13757998) and [`https://doi.org/10.5281/zenodo.13748215`](https://doi.org/10.5281/zenodo.13748215)

The data should be downloaded and placed in a directory called `Metadynamic_ORF6_full_length_simulations_Zenodo` and `Metadynamic_simulations_Zenodo` (this is from the manuscript titled 'An integrative characterisation of proline cis and trans conformers in a disordered peptide' for comparison of the corresponding region from full-length orf6 simulations). This should be in the same diectory as `ORF6-METADYNAMICS-ANALYSIS.ipynb`, with the `README_metadynamic_simulations.md` file. 

#### System subdirectories   
There are subdirectories containing experimental data and PLUMED files required for `ORF6-METADYNAMICS-ANALYSIS.ipynb` and `ORF6-MODEL-SYSTEM-METADYNAMICS-ANALYSIS.ipynb`. 
1. The PBMetaD bias from the `COLVAR_nohead` file is required for blocking analysis for each system.
2. The chemical shifts and `camshift_plumed.dat` are available to run CamShift (1) for each trajectory locally. Experimental chemical shift data was measured at 310.15 K (37 degrees celsius). 
3. The `model_ctr` subdirectory contains files for the last 21-residues from the full-length ORF6 metadynamic simulations. 

#### Blocking analysis 
Blocking analysis scripts were taken from [`blocking analysis scripts`](https://github.com/fpesceKU/BLOCKING) (2). Both of these python scripts are used in the Jupyter notebook 


## References
1. Kohlhoff KJ, Robustelli P, Cavalli A, Salvatella X, Vendruscolo M. Fast and accurate predictions of protein NMR chemical shifts from interatomic distances. J Am Chem Soc. 2009 Oct 7;131(39):13894-5. doi: 10.1021/ja903772t. PMID: 19739624.

