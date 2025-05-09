Project Name: Physics-Informed Neural Networks for Ising and Hubbard Models
This repository contains various scripts and notebooks for generating datasets and training Physics-Informed Neural Networks (PINNs) on Ising and Hubbard models, both in 1D and 2D. The data generation and model training are tailored for different configurations of these physical systems, with a focus on utilizing RBMs and exact diagonalization for generating data and solving the corresponding models with PINNs.

Directory Structure
Data Generation
MC-RBM.ipynb: Code for generating data for the 1D Ising model using the Metropolis algorithm and Restricted Boltzmann Machines (RBM).

data_gen_2d.ipynb: Code for generating data for the 2D Ising model.

hubbard_datagen_1d.ipynb: Code for generating data for the 1D Hubbard model using exact diagonalization.

PINN Training
pinn-ising.ipynb: Code for training and testing a Physics-Informed Neural Network (PINN) on 1D Ising model data.

pinn_ising_2d.ipynb: Code for training and testing a Physics-Informed Neural Network (PINN) on 2D Ising model data.

pinn_hubbard.ipynb: Code for training and testing a Physics-Informed Neural Network (PINN) on 1D Hubbard model data.

Generated Datasets
ising_dataset.npz: Contains generated data for the 1D Ising model.

ising_2d_dataset_3x3.npz: Contains generated data for the 2D Ising model (3x3 lattice).

hubbard_data_n6.npz: Contains generated data for the 1D Hubbard model (with N=6 sites).

Usage
To use the code in this repository:

Data Generation: Use the respective notebooks (MC-RBM.ipynb, data_gen_2d.ipynb, hubbard_datagen_1d.ipynb) to generate data for the Ising or Hubbard models. The notebooks make use of numerical techniques such as Metropolis sampling, Gibbs sampling, and exact diagonalization to produce the datasets.

PINN Training: Once the data is generated, use the PINN training notebooks (pinn-ising.ipynb, pinn_ising_2d.ipynb, pinn_hubbard.ipynb) to train and test Physics-Informed Neural Networks. These models are designed to predict wavefunctions or other physical quantities for the Ising and Hubbard systems.

Dataset Loading: Load the generated datasets (ising_dataset.npz, ising_2d_dataset_3x3.npz, hubbard_data_n6.npz) into your models for training or analysis.

Requirements
To run the notebooks, you will need the following dependencies:

Python 3.x

NumPy

TensorFlow or PyTorch (depending on the framework used in the PINN notebooks)

Matplotlib (for plotting results)

Other specific libraries as used in the notebooks

You can install the required libraries using pip:

bash
Copy
Edit
pip install -r requirements.txt
License
This repository is licensed under the MIT License. See the LICENSE file for more information.

Acknowledgements
This work was inspired by the application of machine learning techniques to quantum many-body systems, and the use of Physics-Informed Neural Networks (PINNs) for solving complex systems in statistical physics.