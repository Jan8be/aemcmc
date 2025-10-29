# aemcmc
MCMC simulations of proteins using autoencoder-generated structures

In this repository, you can find jupyter notebooks with the code used to perform MCMC simulations of (mini)proteins. 

- Notebook `trj2npy` contains code used to prepare training dataset - extract Cartesian coordinates of protein atoms from supplied 
xtc file and save it as a numpy array. 
- Notebook `ae` contains the code for building the autoencoder ML model, trains it on the (mini)protein structures and 
saves it. 
- Notebook `analyse_ls` contains code for analysing the AE latent space, and allown for precise selection of latent space coordinates, 
decoding a protein structure from them and calculating its potential energy. 
- Notebook `MC` provides the code for loading the trained model, conducting MCMC simulation using the decoder, and analysing the sampled 
population of structures.

Notebooks `analyse_ls` and `MC` can be ran straight after the ML model is prepared in `ae` in any order.
