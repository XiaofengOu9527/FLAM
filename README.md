FLAM (Fast Linear Algebra in MATLAB)
====================================

This MATLAB library implements various fast algorithms for matrices with hierarchical low-rank block structure. Such matrices have appeared in the literature under an assortment of related names (H-, H2-, FMM, HODLR, HSS, HBS, etc.) and commonly arise in physical problems, including many classical integral and differential equations. Other application domains include data analysis and uncertainty quantification (covariance matrices).

The primary purpose of this library is for personal prototyping, though it has been recognized that others may find it useful as well. Consequently, the algorithms do not contain all the latest features, but they can be considered reasonably complete; for example, most codes support full adaptivity.

It is also worth noting that we mainly use the interpolative decomposition (ID) for low-rank approximation. This is by no means the only choice, but we find it convenient due to its structure-preserving and numerical compression properties. Since the ID is such a core component of this library, we would be remiss if we did not properly alert the user to its use.

Currently implemented algorithms include:

- core routines:

 - tree construction

 - interpolative decomposition

 - fast spectral norm estimation

- dense matrix routines:

 - recursive skeletonization (multiply, sparse extension)

 - recursive skeletonization factorization (multiply, solve)

 - hierarchical interpolative factorization (multiply, solve)

 - interpolative fast multipole method (multiply)

Still to come (hopefully):

- sparse matrix routines

- Cholesky multiply/solve, determinant, selected inversion

All algorithm directories contain extensive tests. Please refer to the individual source codes for reference information.

FLAM is freely available under the GNU GPLv3; for alternate licenses, please contact the author.