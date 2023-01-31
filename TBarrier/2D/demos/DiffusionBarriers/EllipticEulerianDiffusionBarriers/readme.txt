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

Computation of elliptic Eulerian diffusion barriers [1,3] using the null-geodesics algorithm introduced by [2].

The demo is inside the folder "Main":

_"EllipticEulerianDiffusionBarriersAgulhas": Elliptic Eulerian diffusion barriers demo applied to AVISO data set in Agulhas region.

Auxiliary functions in current folder:

_"closed_curve": Checks if curve is smooth and closed and returns the closed curve if it exists.
_"find_outermost_closed_curve": Computes outermost elliptic Eulerian diffusion barrier within each family of elliptic  elliptic Eulerian diffusion barriers.
_"init_level_set": Computes set of ICs based on transport density.
_"phi_prime":	Computes Interpolants for phi_prime and denominator of phi_prime
_"RK4_integration": Defines RK4-integration scheme.
_"closed_null_geodesics": Wrapper function to compute outermost closed null geodesics (=outermost elliptic Eulerian diffusion barrier)

References:

[1] Haller, G., Karrasch, D., & Kogelbauer, F. (2018). Material barriers to diffusive and stochastic transport. Proceedings of the National Academy of Sciences, 115(37), 9074-9079.

[2] Serra, M., & Haller, G. (2017). Efficient computation of null geodesics with applications to coherent vortex detection. Proceedings of the Royal Society A: Mathematical, Physical and Engineering Sciences, 473(2199).

[3] Notebook 8.2. in "Transport Barriers and Coherent Structures in Flow Data" by Prof. George Haller.

[4] Link to YouTube Tutorial: https://youtu.be/gyDxsiqKezk