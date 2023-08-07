# Structural Material Selection Using Deep Learning
Github code to support the thesis of Luis Yepes Llorente entitled "Structural Material Selection Using Deep Learning"


Universidad de Sevilla

ICA, Université de Toulouse, ISAE-SUPAERO, MINES ALBI, UPS, INSA, CNRS, Toulouse, France.

## Dependencies

PyTorch, scipy, numpy, matplotlib, pymoo


## Abstract

In an increasingly competitive and digital industrial environment, the optimization of structures
is a key point not only to reduce costs but also to reduce the consumption of natural resources.
To this end, different approaches have emerged throughout history based on the tools available
at the time.

With the current rise of artificial intelligences and the concept of Machine Learning,
revolutionary ideas are emerging that allow an optimal dimensioning of structures in record time.
This work presents the use of Variational Autoencoders as a proposal for structural optimization
solving mainly the discrete nature of the materials, being able to have a continuous space of
materials that allows to accelerate enormously the search of the material to be used with gradient
operations. An existing proposal based on this idea is improved and very important conclusions are
drawn for its future development.




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

## Pareto_Bruteforce
Gets a solution by brute-force of a set of objectives and plots the Pareto front from the solution

## Integer_Optimizer
Performs a multiple optimization of material and geometry using the pymoo tool Multi-objective Optimization With Mixed Variables https://pymoo.org/customization/mixed.html

## VAE_Mixed_Multi_pymoo
Runs a program similar to **VAE_Multi_pymoo** and then applies **Integer_Optimizer** to the reduced database

## Integer_Optimizer_3objectives
Performs the same operation than in "Integer_Optimizer" but considering three objectives and representing the Pareto front

## VAE_Mixed_Multi_pymoo_3D
Performs the same operation than in "VAE_Mixed_Multi_pymoo" but applied to a three-dimensional truss and considering three objectives

## VAE_Mixed_Multi_pymoo_3D_INDEX
Performs the same operation than in "VAE_Mixed_Multi_pymoo_3D" but considering the environmental consumption as objective


