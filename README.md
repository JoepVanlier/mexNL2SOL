# mexNL2SOL
Mex wrapper for NL2SOL

NL2SOL MEX

Here you can find a very minimal MATLAB wrapper to NL2SOL (with bound constraints) from the PORT library. I have so far only tested it on Linux with MATLAB R2013b, but I think it should also function properly under windows and mac.

Installing is easy if you have a FORTRAN and C compiler installed and configured for compiling MEX files. Simply add the repo to your MATLAB path. Type compileNL2SOL, and you should be ready to go.

Syntax is similar to lsqnonlin. [X,RESNORM,RESIDUAL,EXITFLAG,ITERATIONS,FEVALS,JACOBIAN] = mexnl2sol(FUN,X0,(LB),(UB),(OPTIONS))

Note however that the output struct of lsqnonlin is replaced with iterations and lambda with the number of function evaluations.

If you have tested it on another MATLAB/OS combination, or find a bug in the code, please drop me a line, then I will update the code/wiki.
