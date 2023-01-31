%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%%%%%%%%%%%%%%%%%%%%              ____________________   ___             %%%%%%%%%%%%%%%%%%%%%
%%%%%%%%%%%%%%%%%%%%%             /  ________   ___   /__/  /             %%%%%%%%%%%%%%%%%%%%%
%%%%%%%%%%%%%%%%%%%%%            /  _____/  /  /  /  ___   /              %%%%%%%%%%%%%%%%%%%%%
%%%%%%%%%%%%%%%%%%%%%           /_______/  /__/  /__/  /__/               %%%%%%%%%%%%%%%%%%%%%
%%%%%%%%%%%%%%%%%%%%%     Swiss Federal Institute of Technology Zurich    %%%%%%%%%%%%%%%%%%%%%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
%%%%%%%%%%%%%%%%%%%%%  Authors:    Alex P. Encinas Bartos, George Haller  %%%%%%%%%%%%%%%%%%%%%
%%%%%%%%%%%%%%%%%%%%%  Revised by: Balint Kaszas                          %%%%%%%%%%%%%%%%%%%%%
%%%%%%%%%%%%%%%%%%%%%  Email:      enalex@ethz.ch                         %%%%%%%%%%%%%%%%%%%%%
%%%%%%%%%%%%%%%%%%%%%  Date:       07/06/2022                             %%%%%%%%%%%%%%%%%%%%%
%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%

Computation of active momentum and vorticity barriers from aFTLE according to [1,2]. The two dimensional turbulence dataset (velocity and vorticity fields in the folder "Data") and the advected trajectories ("particles1100.mat") for the Lagrangian calculations can be downloaded from: https://polybox.ethz.ch/index.php/s/L0b0piQEqhOqNjg. The combined size of the entire dataset is approximately 10GB.

The demos are inside the folders "Main"

_"aFTLE2DTurbulenceLagrangianVorticity": aFTLE to visualize Lagrangian vorticity barriers.
_"aFTLE2DTurbulenceLagrangianLinearMomentum": aFTLE to visualize Lagrangian linear momentum barriers.
_"aFTLE2DTurbulenceEulerianVorticity": aFTLE to visualize Eulerian vorticity barriers.
_"aFTLE2DTurbulenceEulerianLineraMomentum": aFTLE to visualize Eulerian linear momentum barriers.

References:

[1] Haller, G., Katsanoulis, S., Holzner, M., Frohnapfel, B., & Gatti, D. (2020). Objective barriers to the transport of dynamically active vector fields. Journal of Fluid Mechanics, 905.

[2] Notebook 9.2. in "Transport Barriers and Coherent Structures in Flow Data" by Prof. George Haller.

[3] [YouTube Tutorial](https://youtu.be/4YwqRtyN0CI)