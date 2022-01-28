# crup
##### a Collection of Random Unconstrained Polynomial optimization problems

This is a collection of sparse polynomials used in the computational experiments of the paper 
> D. Papp. Duality of sum of nonnegative circuit polynomials and optimal SONC bounds. (Submitted.) [https://arxiv.org/abs/1912.04718](https://arxiv.org/abs/1912.04718) 

## overview

The two folders in the repository contain the instances used the two sets of experiments:
* The folder `SdW` contains the most difficult instances of the repository of Seidler and de Wolff that accompanies their paper
> H. Seidler and T. de Wolff. An experimental comparison of SONC and SOS certificates for unconstrained optimization. arXiv preprint arXiv:1808.08431 [https://arxiv.org/abs/1808.08431](https://arxiv.org/abs/1808.08431)
>  
These are randomly generated polynomials with random non-simplex Newton polytopes, with varying numbers of varianles and degrees. Each have 500 monomials in their support.

* The folder `sparse` contains randomly generated polynomials of varying sparsity. Each have 25 variables and degree 8, the number of monomials vary between 165 and 3301.

## format description

* Each CSV file represents a single polynomial in standard comma-separated values format.
* Each line in an instance represents a monomial, with the exponent vector followed by the coefficient. For example, `0,1,1,-2` represents the monomial -2 *x*2 *x*3. The polynomial encoded in a file is the sum of the monomials encoded in each line.
* The filenames of the `SdW` instances refer to the number of the instance in the original repository.
* The filenames of the `sparse` instances are formatted as `[no. variables]_[degree]_[no. monomials]_[experiment no.].csv`. This is for informational purposes only, the contents of the file are sufficient to represent a unique polynomial without the filename.
