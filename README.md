# A Hybrid Machine Learning and Evolutionary Approach to Material Selection and Design Optimization for Eco-Friendly Structures
Github code to support the paper entitled "A Hybrid Machine Learning and Evolutionary Approach to Material Selection and Design Optimization for Eco-Friendly Structures"


ICA, Université de Toulouse, ISAE-SUPAERO, MINES ALBI, UPS, INSA, CNRS, Toulouse, France.
Universidad de Sevilla

## Dependencies

PyTorch, scipy, numpy, matplotlib, pymoo


## Abstract

In an increasingly competitive and digital industrial environment, the optimization of structures is a key point not only to reduce costs but also to reduce the consumption of natural resources. To this end, different approaches have emerged throughout history based on the tools available at the time. With the current rise of artificial intelligence and the concept of Machine Learning, revolutionary ideas are emerging that allow an optimal dimensioning of structures in record time. This work presents the use of Variational Autoencoders and mixed variable solvers as a proposal for structural optimization and material selection.
It has expanded upon previous research by advancing in three directions: (1) Incorporating more material attributes, particularly relevant for environmental considerations. (2) A new constraint on the optimizer to steer far from vacant spaces in the VAE latent space. (3) A two-step hybrid approach to select the optimal candidate: preliminary filtering with VAE and final design via mixed variable model. Various examples demonstrate the applicability of the proposed method.




# Basic Information

The database of materials is inside the folder "data"

The figures are saved inside the folders "figures*"

The VAE is saved at the folder "results"

The folder "src" contains some python packages codes such as the material encoder, truss examples or the Finite Element Solver


## VAE_2D_Visual
It trains the VAE and displays a series of results such as the decoding error, the latent space (2D) considering 2 coordinates or the gradients of the properties.

## VAE_3D_Visual
It trains the VAE and displays a series of results such as the decoding error, the latent space (3D) considering 3 coordinates or the gradients of the properties.

## VAE_Single_pymoo
Solves the single-objective problem with NSGAII algorithm making use of the VAE

## VAE_Multi_pymoo
Solves the multi-objective problem with NSGAII algorithm making use of the VAE

## Bruteforce_analysis
Gets a solution by brute-force of a set of objectives and plots the Pareto front from the solution

## Integer_Optimizer
Performs a multiple optimization of material and geometry using the pymoo tool Multi-objective Optimization With Mixed Variables https://pymoo.org/customization/mixed.html

## Hybrid
Runs the Hybrid model.

## Hybrid_3objectives.ipynb
Same than Hybrid but adapted to 3 objectives and the three-dimensional truss

## Integer_Optimizer_3Dtruss.ipynb
Same than Integer_Optimizer but applied to the three-dimensional truss. Useful to get the compliance vs mass plot


