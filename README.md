# ComparisonStudy
Matlab programs to perform exemple 3.1.

Workplace.m : Mainscript to execute the calibration method.
Figures.m : displays figures present in the paper.
fftma.m : function to perform fast Fourier transform moving average simulations (FFTMA)
TourBandSpec.m : function to perform spectral turning band simulations (STBM)
LUsim.m : function to perform Choleski decomposition simulations (LU)
TourBandSpecOpt.m : function to perform sequential spectral turning band methods (S-STBM)
GDOpt.m :: function to perform gradual deformation (GD)
ISROpt.m : function to perform Iterative spatial resampling (ISR)
PhaseAnnealing2D.m : function to perform phase annealing in 2D only (PA) 
fftmaSA.m : function to perform FFTMA simulated annealing (FFTMA-SA)
VanCorput.m : generate quasi-random sequences (for S-STBM)
DensSpec1Ddl.m : Compute the 1D spectral density of convariance function (for S-STBM)
covardm.m : compute covariance function
KrigingS.m : performs simple kriging
postcond.m : performs post-conditioning by kriging.

The other examples are easily realized by changing the objective function.

Both hydrogeological examples (section 3.3) used the Matlab Reservoir Simulation Toolbox (MRST) of the Computational Geosciences group in the Department of Mathematics and Cybernetics at SINTEF Digita. MRST is a free open-source software for reservoir modelling and simulation.  Link : https://www.sintef.no/projectweb/mrst/

Further details are found, for each variogram-based inversion method, in their original manuscript, namely:

GD :Hu, L. Y. (2000).  Gradual deformation and iterative calibration of Gaussian-related stochastic models. Mathematical Geology,32, 87–108. doi:10.1023/a:1007506918588.

ISR : Mariethoz, G., Renard, P., & Caers, J. (2010). Bayesian inverse problem and optimization with iterative spatial resampling.Water Resources Research,46. doi:10.1029/2010wr009274.

PA : Hörning, S., & Bárdossy, A. (2018).  Phase annealing for the conditional simulation of spatial random fields.Computers & Geosciences,112, 101–111. doi:10.1016/j.cageo.2017.12.008.

FFTMA-SA : Lauzon, D., & Marcotte, D. (2019). Calibration of random fields by FFTMA-SA.Computers & Geosciences,127, 99–110. doi:10.1016/j.cageo.2019.03.003.

S-STBM : Lauzon, D., & Marcotte, D. (2020). Calibration of random fields by a sequential spectral turning396bands method.Computers & Geosciences,135, 104390. doi:10.1016/j.cageo.2019.104390.

