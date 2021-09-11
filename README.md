# ComparisonStudy

Simply run the script 'WorkplaceSim.m'. The directives are mentioned in the script.
The variable named type holds the number of the case under study.



Folder Description

1- The folder named 'Data' contains the reference data for the simulation. The data are saved in a .mat file named ExX_Data.mat 
where X is the number of the case. The .mat file contains all the information need to reproduce the case shown in the manuscript.

2- The folder named 'Figures' contains five Matlab functions to generate the figures presented in the manuscript. Only need
 to run the function code for the case study to show the figure. Some figures may take time to be generated especially ones 
 for statistical analysis (case 1 and case 2). 

3- The folder named 'Function' contains Matlab functions for calibration purpose

   CODE OF THE VARIOGRAM-BASED INVERSION METHODS
   SSTBM.m   : Sequential spectral turning band method
   FFTMASA.m : Fast Fourier Transform Moving Average Simulated Annealing
   ISR.m     : Iterative spatial resampling
   PA.m      : Phase annealing (Only works in 2D) 
   GD.m      : Gradual deformation
    
   ObjectiveFunction.m : Contains the objective function for the five cases.
   ParamSimulation.m   : COntains parameters for the simulation (e.g. covariance model, size grid, ...)

   The other functions are needed to run the five variogram-based inversion methods listed above
       
   FFTMA.m         : Fast Fourier Transform Moving Average, generated uncalibrated simulations
   STBM.m          : Spectral turning band method, generated uncalibrated simulations
   LUsim.m         : Cholesky decomposition simulation, generated uncalibrated simulations
   covardm.m       : Computes the covariance matrix
   DensSpecDdl.m   : Computes the one-dimensional spectral density from the desired covariance matrix
   grille2.m       : Generated the regular 2D grid
   grille3.m       : Generated the regular 3D grid
   postcond.m      : Performs post-conditionning by kriging
   VanCorput.m     : Genereted random line direction over a unit half-sphere using the van der Corput sequence
   varioFFT2D_dl.m : Compute variograms, cross-variograms, covariograms, directional asymmetry,... using FFT.

4- The folder named 'Reference' contains the reference function to generete the five cases

5- The folder named 'Results' keeps the results for each case.
    

Both hydrogeological examples (cases 3 and 4) used the Matlab Reservoir Simulation Toolbox (MRST) of the Computational Geosciences group in the Department of Mathematics and Cybernetics at SINTEF Digita. MRST is a free open-source software for reservoir modelling and simulation.  Link : https://www.sintef.no/projectweb/mrst/

   Further details are found, for each variogram-based inversion method, in their original manuscript, namely:

  GD :Hu, L. Y. (2000).  Gradual deformation and iterative calibration of Gaussian-related stochastic models. Mathematical Geology,32, 87–108. doi:10.1023/a:1007506918588.

   ISR : Mariethoz, G., Renard, P., & Caers, J. (2010). Bayesian inverse problem and optimization with iterative spatial resampling.Water Resources Research,46.        doi:10.1029/2010wr009274.

  PA : Hörning, S., & Bárdossy, A. (2018).  Phase annealing for the conditional simulation of spatial random fields.Computers & Geosciences,112, 101–111. doi:10.1016/j.cageo.2017.12.008.

  FFTMA-SA : Lauzon, D., & Marcotte, D. (2019). Calibration of random fields by FFTMA-SA.Computers & Geosciences,127, 99–110. doi:10.1016/j.cageo.2019.03.003.

  S-STBM : Lauzon, D., & Marcotte, D. (2020). Calibration of random fields by a sequential spectral turning396bands method.Computers & Geosciences,135, 104390. doi:10.1016/j.cageo.2019.104390.
