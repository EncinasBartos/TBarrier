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

Computation of hyperbolic LCS [1,2,3,4]

The demo is inside the folder "Main":

_"HyperbolicLCSAgulhas": Hyperbolic LCS demo applied to AVISO data set in Agulhas region.

_"HyperbolicLCSTurbulence": Hyperbolic LCS demo applied to 2D turbulence simulation. The two dimensional turbulence dataset (velocity and vorticity fields in the folder "Data") and the advected trajectories ("particles1100.mat") for the Lagrangian calculations can be downloaded from: https://polybox.ethz.ch/index.php/s/L0b0piQEqhOqNjg. The combined size of the entire dataset is approximately 10GB.

Auxiliary functions in current folder:

_"orient_vectorfield": Locally (within a grid-cell) re-orients the globally non-orientable eigenvector field and evaluates the eigenvector at 'x' via linear interpolation.
_"RK4_tensorlines": Defines update scheme (RK4-integration) in order to integrate tensorlines. Separate functions for compressible/incompressible velocity fields.
_"scaling_vectorfield": Rescales eigenvector so that tensorline singularites are turned into fixed points (see [1]). Separate functions for compressible/incompressible velocity fields.
_"tensorlines": Wrapper functions for _RK4_tensorlines_incompressible()/_RK4_tensorlines_compressible().

References:

[1] Farazmand, M., & Haller, G. (2012). Computing Lagrangian coherent structures from their variational theory. Chaos: An Interdisciplinary Journal of Nonlinear Science, 22(1), 013128.

[2] Farazmand, M., & Haller, G. (2013). Attracting and repelling Lagrangian coherent structures from a single computation. Chaos: An Interdisciplinary Journal of Nonlinear Science, 23(2), 023101.

[3] Onu, K., Huhn, F., & Haller, G. (2015). LCS Tool: A computational platform for Lagrangian coherent structures. Journal of Computational Science, 7, 26-36.

[4] Notebook 5.6. in "Transport Barriers and Coherent Structures in Flow Data" by Prof. George Haller.
