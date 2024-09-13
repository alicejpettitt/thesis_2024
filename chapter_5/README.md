# Biophysical characterisation of ORF6 from SARS-CoV-2 

Scripts used to produce figures in Alice Jane Pettitt's thesis. Submitted September 2024 to University College London. 

I used PLUMED version 2.7.1 and GROMACS 2021.2. 

## This repository contains scripts to produce some of the Figures, analysis, and input files from Chapter 5:
1. `full-length_orf6` directory containing two subdirectories. `Analysis` contains the scripts and data to repeat the metadynamic simulations analysis and reproduce the simulation figures. `PLUMED_input_files` contains the files to rerun the metadynamic simulations of full-length ORF6 simulations in the AMBER03ws force field. The `setup` subdirectory contains the GROMACS files used to collapse the linear peptide at 400 K then generate the 128 starting conformations and equilibrate the system at 310 K for the metadynamic sims. 
2. `orf6-rae1-nup98` directory contains the `PLUMED_input_files` to rerun the metadynamic simulations of full-length orf6 - RAE1 - NUP98-GLEBS. `PDB_files` contains the PDB files used to make both orf6-rae1-nup98 figures in Chapter 5.

Large data files (including trajectories, metadynamics weights, and Lennard Jones/Coulomb interaction energies) are hosted on Zenodo here: `https://doi.org/10.5281/zenodo.13757998` and `https://doi.org/10.5281/zenodo.13757998`

If you find bugs please email [`alicepettitt98@gmail.com`](alicepettitt98@gmail.com)

