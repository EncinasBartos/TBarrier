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

Computation of elliptic LCS using the null-geodesics algorithm introduced by [1,2]

The demo is inside the folder "Main":

_"EllipticLCSAgulhas":    Elliptic LCS demo applied to AVISO data set in Agulhas region.

_"EllipticLCSTurbulence": Elliptic LCS demo applied to 2D turbulence simulation. The two dimensional turbulence dataset (velocity and vorticity fields in the folder "Data") and the advected trajectories ("particles1100.mat") for the Lagrangian calculations can be downloaded from: https://polybox.ethz.ch/index.php/s/L0b0piQEqhOqNjg. The combined size of the entire dataset is approximately 10GB.

Auxiliary functions in current folder:

_"closed_curve":      			Checks if curve is smooth and closed and returns the closed curve if it exists.
_"find_outermost_closed_curve":     Computes outermost elliptic LCSs within each family of elliptic LCSs.
_"init_level_set":             	Computes set of ICs based on stretching parameter.
_"phi_prime":				Computes Interpolants for phi_prime and denominator of phi_prime
_"RK4_integration": 			Defines RK4-integration scheme.
_"closed_null_geodesics":           Wrapper function to compute outermost closed null geodesics (=outermost elliptic LCS)

References:

[1] Serra, M., & Haller, G. (2017). Efficient computation of null geodesics with applications to coherent vortex detection. Proceedings of the Royal Society A: Mathematical, Physical and Engineering Sciences, 473(2199).

[2] Notebook 5.4.2. in "Transport Barriers and Coherent Structures in Flow Data" by Prof. George Haller.