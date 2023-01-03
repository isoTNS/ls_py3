# line search package for python 3

The original line search package (ls) created from the nlpy package seems to have conflict with python >= 3.6.
This is true; C extension modules changed between python2 and python3, so I rewrote the C wrapper that calls the Fortran linesearch code. 
-- SAJANT ANAND

