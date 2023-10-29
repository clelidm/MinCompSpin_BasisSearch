# MinCompSpin_BasisSearch
This program searches for the Best Basis representation for a chosen binary dataset.

## Requirements

The code uses the C++11 version of C++.

## Usage with Makefile:

Run the following commands in your terminal, from the main folder (folder containing the `makefile` document):

 - **To compile:** `make`

 - **To Execute:** `make run` . This will use the datafile and variables that are specified in the makefile.

To change datafile: open the makefile and replace the values of the two following variables at the very top of the file (an example is provided):
>  - `datafile`: name of your datafile; this file must be placed in the folder `INPUT`
>  - `n`: number of variables in your file; maximum possible value `n = 128`.

You can also execute the code by running in your terminal the command (from the main folder):
```bash
./BestBasis.out  datafilename  n
```

where you must replace `datafilename` by the name of your datafile and `n` by your number of variables.

 - **To clean:** `make clean` (to use only once you're done using the code)

## Examples

All the functions that can be called from `int main()` are declared at the beginning of the `main.cpp` file. The most useful functions are described in the section "General information" above. 

In the `INPUT` folder, we provided two examples:
  - the binary dataset `SCOTUS_n9_N895_Data.dat`, which is the dataset of votes of the US Supreme court analysed in Ref.[3] and used as an example in Ref.[1]. 
  - the binary dataset `Big5-IPC1_VS3_Ne5.dat`: this is a binarized version of the first `100 000` samples of the Big 5 dataset [4], which has `50` variables. See paper [1] for comments on the Best Basis obtained for this dataset.

Each of these two datasets can be the one run as an example by commenting/uncommenting the correct datafile choice at the beginning of the `makefile`.

For hands-on and simple tests of the program, please check the examples in the function `int main()` of the `main.cpp` file. 

[3] E.D. Lee, C.P. Broedersz, W. Bialek, Statistical Mechanics of the US Supreme Court. [J Stat Phys 160, 275–301 (2015)](https://link.springer.com/article/10.1007/s10955-015-1253-6).

[4] Big 5 dataset, add reference (reference can be found in [1])

## License

This code is an open source project under the GNU GPLv3.
