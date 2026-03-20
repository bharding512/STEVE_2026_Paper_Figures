# STEVE_2026_Paper_Figures
Code to run the model and create figures for the Harding and Gasque (2026) paper: Harding and Gasque (2026) paper:  "Electron-Impact Excitation of N$_2$ is Insufficient to Produce the NO$_2$ Continuum in STEVE"

 - **The main code is in "Harding_Gasque_2026_Figures.ipynb"**
 - The module "steve_n2v.py" is required
 - Cross sections are in the file "cross_sections_N2_laporta_subset.nc"
 - BOLSIG+ runs, used for Run 3, were pre-computed and the EEDFs are available in the "EEDFs_subset.csv" file. A Python reader for this file is available in steve_n2v.py
 - Each of the 3 runs may take a few hours at high resolution. For each, a low-resolution option is the default option for quick testing. Uncomment the high-resolution option to make the exact figures in the publication
 
This requires "itm_models" to be installed (https://github.com/bharding512/itm_models). But it's just used to initialize densities to MSIS, so it should be straightforward to replace it with any other implementation of MSIS, or you can just manually input neutral densities. 
