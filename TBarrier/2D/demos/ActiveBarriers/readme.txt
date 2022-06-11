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

Computation of active momentum and vorticity barriers according to [1,2]. The two dimensional turbulence dataset (velocity and vorticity fields in the folder "Data") and the advected trajectories ("particles1100.mat") for the Lagrangian calculations can be downloaded from: https://polybox.ethz.ch/index.php/s/L0b0piQEqhOqNjg. The combined size of the entire dataset is approximately 10GB.

The demos are inside the folders "aFTLE2D/aPRA2D/aTRA2D/aTSE2D/Hamiltonian"

Auxiliary functions in current folder:

_"InstantaneousActiveMomentum":  Interpolant for RHS of active instantaneous (Eulerian) linear momentum barrier equation.
_"InstantaneousActiveVorticity": Interpolant for RHS of active instantaneous (Eulerian) vorticity barrier equation.
_"LagrangianActiveMomentum":     Interpolant for RHS of active Lagrangian linear momentum barrier equation.
_"LagrangianActiveVorticity":    Interpolant for RHS of active Lagrangian vorticity barrier equation.

References:

[1] Haller, G., Katsanoulis, S., Holzner, M., Frohnapfel, B., & Gatti, D. (2020). Objective barriers to the transport of dynamically active vector fields. Journal of Fluid Mechanics, 905.

[2] Notebook 9.7.1. in "Transport Barriers and Coherent Structures in Flow Data" by Prof. George Haller.