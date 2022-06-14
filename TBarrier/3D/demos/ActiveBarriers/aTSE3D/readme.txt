%%%%%%%%%%%%%%%%%%%%%%              ____________________   ___             %%%%%%%%%%%%%%%%%%%%%
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

Computation of active TSE (aTSE) [1,3]

The demo is inside the folder "Main":

_"aTSEABCviscous": active TSE uncovers hyperbolic barriers to linear momentum and vorticity in a viscous, unsteady ABC flow.
_"aTSE3DChannel_part1": active TSE uncovers hyperbolic barriers to linear momentum and vorticity in a turbulent channel flow, part 1.
_"aTSE3DChannel_part2": active TSE uncovers hyperbolic barriers to linear momentum and vorticity in a turbulent channel flow, part 2.

NOTE: "aTSE3Dchannel_part2" is conceptually the same as "aTSE3Dchannel_part1" on a different domain. The reason why we include it, is that it reproduces the results on the momentum barriers [2] available in matlab on https://github.com/haller-group/TRA_TSE.

References:

[1] Haller, G., Katsanoulis, S., Holzner, M., Frohnapfel, B., & Gatti, D. (2020). Objective barriers to the transport of dynamically active vector fields. Journal of Fluid Mechanics, 905.

[2] Aksamit, N.O., & Haller, G. (2022). Objective momentum barriers in wall turbulence. Journal of Fluid Mechanics, 941.

[3] Encinas Bartos, A. P., Aksamit, N. O., & Haller, G. (2021). Quasi-Objective Eddy Visualization from Sparse Drifter Data. arXiv preprint arXiv:2111.14117.

[4] Notebook 9.7.2. in "Transport Barriers and Coherent Structures in Flow Data" by Prof. George Haller.