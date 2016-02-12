# conformer_search
Thoroughly generate possible conformations of small molecules for subsequent semi-empirical optimization.

Conformations are in general created by rotating in 30 degree increments around each bond, recognizing symmetry (in some cases) and bond hybridization to avoid redundant or unphysical conformers. In addition the free lone-pair (if existing) on tetrahedral Nitrogen is inverted by interchanging two of the bonded groups.

The idea behind the program is that we can bruteforce enough structures such that we will end up with all relevant conformations following optimization by force-fields or semi-empirical methods.


Usage: python conformer_search <gzmat file>

Note: The extensive flag can be changed to enable how thorough the search should be.
