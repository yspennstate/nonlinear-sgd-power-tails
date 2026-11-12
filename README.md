# Exact power tails and moment growth for a contractive nonlinear SGD model

Yitzchak Shmalo, Einstein Institute of Mathematics, The Hebrew University of Jerusalem

- Paper: [T228_Nonlinear_SGD_Power_Tails.pdf](T228_Nonlinear_SGD_Power_Tails.pdf)
- LaTeX source: [T228_Nonlinear_SGD_Power_Tails.tex](T228_Nonlinear_SGD_Power_Tails.tex)
- Exact rational arithmetic for the contraction and moment constants: [verify_arithmetic.py](verify_arithmetic.py), output in [verification_result.json](verification_result.json)

For the activation sigma(z) = z + 10^-3 tanh z, constant-step batch-one SGD on squared loss with Gaussian inputs and Gaussian label noise is contractive on average for every step size in [0.99, 1.01]. Its stationary law is unique and has an exact power tail with exponent in (1, 2) and a strictly positive tail constant. The paper also proves exact linear growth of the critical moment and finite positive limits for the normalized supercritical moments.

Build with `pdflatex T228_Nonlinear_SGD_Power_Tails.tex` (twice). Run the arithmetic check with `python3 verify_arithmetic.py`.

The paper is part of the Math Brain project: [repository](https://github.com/yspennstate/math-brain-public), [paper](https://github.com/yspennstate/math-brain-public/tree/main/papers/math-brain-2026-10-24). It is released under CC BY 4.0.
