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

Computation of LAVD [1,2]

The demos are inside the folder "Main":

_"LAVDAgulhas": LAVD demo applied to AVISO data set in Agulhas region

_"LAVDTurbulence": LAVD demo applied to 2D turbulence simulation. The two dimensional turbulence dataset (velocity and vorticity fields in the folder "Data") and the advected trajectories ("particles1100.mat") for the Lagrangian calculations can be downloaded from: https://polybox.ethz.ch/index.php/s/L0b0piQEqhOqNjg. The combined size of the entire dataset is approximately 10GB.

Auxiliary functions in current folder:

_"LAVD": computes the LAVD along trajectories
_"find_outermost_contour": computes the outermost nearly convex closed contour.

References:

[1] Haller, G., Hadjighasem, A., Farazmand, M., & Huhn, F. (2016). Defining coherent vortices objectively from the vorticity. Journal of Fluid Mechanics, 795, 136-173.

[2] Notebook 5.4. in "Transport Barriers and Coherent Structures in Flow Data" by George Haller.
