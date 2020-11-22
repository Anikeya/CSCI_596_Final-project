# CSCI_596_Final-project
What is MD? 

Molecular dynamics (MD) is a computational method to model and simulate materials. Molecular dynamics simulates interaction between atoms and molecules over a fixed period of time. MD is used to compute structural, mechanical, chemical, and thermodynamical properties of materials. 
Trajectories of particles are calculated using Newton’s equations of motion, and forces and potential energy are calculated using interatomic potentials. This makes the interatomic potential a very important component of the MD system. 

Why NNMD?

The accuracy of molecular dynamics depends on the accuracy of the interatomic potential being used in the simulation. Interatomic potentials are developed using ab initio methods like density functional theory, but this is very computationaly demanding. In recent time, a new method has been employed to develop interatomic potentials using Machine Learning. Machine Learning Potentials can be as accurate as their first principles reference method but at a fraction of the computational cost. They scale linearly with the number of atoms and model complexity.

Project Motivation

It has been observed that the simulations using NNMD fails sooner as the number of atoms in the system increases. This can be explained by using the gaussian distribution. The force prediction using NNMD MLP follows a gaussian distribution and there will be some outlier force predictions, and it requires only a few extreme force predictions to blow up a simulation. As the number of atoms increases in the system we will see more extreme force values causing the failer of simulation. In the project we would like to calculate the "statistical scalability" of NNMD and define the "computational Weibull strength" of NNMD.

![CS596-Project-imag1](https://user-images.githubusercontent.com/13280755/99920128-4c520800-2cd6-11eb-912b-05c3e52f3649.png)
