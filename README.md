# wesca
[![DOI](https://zenodo.org/badge/1075261206.svg)](https://doi.org/10.5281/zenodo.17508998)
WeSCA (standing for **We**ighing **S**cheme **C**onvergence **A**lgorithm) is a simple program done using Python [ShelXFile](https://github.com/dkratzert/ShelXFile) package.
Its main purpose is to automize weighing scheme optimization, especially if the convergence by classical methods takes longer than expected (especially for large structures).

### Installment
> [!IMPORTANT]
> Before installment make sure you have some **post-2017** version of [ShelXL](https://shelx.uni-goettingen.de/) [^1] added to your PATH list.

WeSCA is distributed as a single-file executable. In order for its appropriate working one must either drop both the ``` .hkl ``` and ``` .res ``` files (with the same project names!) to the folder containing the executable or add the ``` .exe ``` directory to the PATH list.  

### Argument list
The usage of WeSCA using command line is as follows:

```
wesca.exe [-h] [-i ITER] [-r REFINE] [-d DELTA] [-v VERBOSE] [-p PLOT] project
```
The parsing arguments are:
- ``` project ``` - name of project (same for both ``` .res ``` and ``` .hkl ``` file)
- ``` -i ``` or ``` --iter ``` - number of iterations (ShelXL runs) (20 by default)
- ``` -r ``` or ``` --refine ``` - number of refinement cycles in each iteration (10 by default)
- ``` -d ``` or ``` --delta ``` - convergence delta (0.0005 by default)
- ``` -v ``` or ``` --verbose ``` - show ShelXL output in each iteration (true by default)
- ``` -p ``` or ``` --plot ``` - show convergence plot (false by default)

### References
[^1]: Sheldrick, G. M. (2015). Acta Cryst. **C71**, 3-8. DOI: [10.1107/S2053229614024218]
