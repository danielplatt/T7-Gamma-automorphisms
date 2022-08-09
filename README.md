# T7-Gamma-automorphisms

This repository computes the group of G2-automorphisms of the torus T^7 endowed with the flat G2-structure, and the orbifold T^7/Gamma endowed with the flat G2-structure, where T^7/Gamma is the simplest example of Joyce's Generalised Kummer Construction.
Namely:

```
alpha: (x1, ..., x7) -> (x1, x2, x3, -x4, -x5, -x6, -x7)
beta:  (x1, ..., x7) -> (x1, -x2, -x3, x4, x5, 1/2-x6, -x7)
gamma: (x1, ..., x7) -> (-x1, x2, -x3, x4, 1/2-x5, x6, 1/2-x7)
Gamma=<alpha, beta, gamma>
```

The results are:

* The automorphism group of T^7 contains 1344 elements, such as the permutation/reflection `([7, 4, 3, 6, 1, 2, 5], (False, False, False, False, True, False, True))`. Here, the first list denotes a permutation of the seven coordinates of T^7, and the second list denotes a reflection in the fifth and seventh coordinate that leaves the other coordinates unchanged. The automorphism is the reflection followed by permutation (in this order).
The full automorphism group of T^7 is then the semidirect product of this group with the group of translations on T^7.
  
* The automorphism group of T^7/Gamma is the translation group `{0, 1/2}^7`. That is: translations by 0 or 1/2 independently chosen in each coordinate. The automorphism group contains no reflections or permutations of coordinates.

This can be deduced from the output of `automorphism_group_of_t7gamma_output.txt`. The output is generated when running `compute_automorphism_group_of_t7gamma.py`.

This result is needed in *Daniel Platt: G2-instantons on resolutions of G2-orbifolds*.