# line search package for python 3

We assume you are running python 3. The original line search package (ls) created from the nlpy package seems to have conflict with python >= 3.6.
(SAJANT:) This is true; C extension modules changed between python2 and python3, so I rewrote the C wrapper that calls the Fortran linesearch code. To install the package, follow these instructions.

To install, unzip the ls\_py3.zip, and from the ls directory, do
```
python setup.py install
```

You out to be in a virtual environment with the desired python version, as this command will create a package local to that environment. If you see errors about missing executables, you probably need to install a Fortran compiler. The following should work.

```
sudo apt-get update; sudo apt-get install gfortran
```

Once you've successfully installed the 'ls' package (can import it), remove the directory.

```
rm -r ls_py3
```

-- SAJANT ANAND
