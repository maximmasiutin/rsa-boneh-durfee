# Boneh & Durfee RSA Low Private Exponent Recovery

This software demonstrates the Boneh & Durfee attack to recovery a low private exponent of an RSA key.

Lattice reduction technique of Coppersmith's method for finding small roots of
univariate or bivariate modular polynomial equations originally proposed to
extract ciphertext bits as described in https://link.springer.com/article/10.1007/s001459900030
can also be used to recover the private exponent (d)
of the RSA key when the exponent is low relative to the public modulus (n), 
e.g. d < n^0.292, as described by Dan Boneh & Glenn Durfee in a 1999
conference paper available at https://doi.org/10.1007/3-540-48910-X_1
that was an improvement over the 1990 result of Wiener showing that when 
d < N 0.25 the RSA system is insecure, as described in https://doi.org/10.1109/18.54902