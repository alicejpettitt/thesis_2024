# Biophysical characterisation of ORF6 from SARS-CoV-2 

Scripts used to produce figures in Alice Jane Pettitt's thesis. Submitted September 2024 to University College London. 

I used PLUMED version 2.7.1 and GROMACS 2021.2. 

## This repository contains scripts to produce some of the Figures from Chapter 4:
1. The simulated ZZ-exchange cross-peak intensity as a function of the exchange rate.
2. The torsion potential energy of the a03ws and C36m force fields as a function of the omega angle. 
3. The `setup` subdirectory contains the input files used to set up the orf6-ctr peptide metadynamic simulations in GROMACS. The `setup` subdirectory contains the GROMACS files used to collapse the linear peptide at 600 K then generate the 128 starting conformations and equilibrate the system at 310 K for the metadynamic sims. 

Most other analyses in Chapter 4 can be found at: https://github.com/alicejpettitt/orf6-ctr_cis_trans_conformers 

If you find bugs please email [`alicepettitt98@gmail.com`](alicepettitt98@gmail.com)

