# Hydrogen atom

## Abstract (Alpha)

The hydrogen atom is a single particle of mass $m$ moving in the attractive Coulomb potential $-k/r$, in any number $d$ of spatial dimensions, with $d=3$ the physical case. Its Hamiltonian is the sum of the kinetic and potential operators on the Hilbert space of square-integrable functions on space. The bound-state energies are the Bohr levels, a Rydberg energy divided by the square of a shifted principal quantum number, and they give the Rydberg formula for the spectral series. The levels are reproduced in several independent ways: by quantising the radial equation, by explicit wave functions built from Laguerre polynomials and harmonic polynomials, and by Pauli's algebraic argument from the conserved Laplace–Runge–Lenz vector. The same ingredients give the large degeneracy of each level and, in three dimensions, the first-order fine structure. The statement that the Bohr levels are exactly the point spectrum of the self-adjoint Hamiltonian, and the scattering states, are not yet formalized.

## Content (Alpha)

### The system and its Hamiltonian

A hydrogen atom is specified by the dimension $d$, a mass $m>0$ and a coupling $k$, and its potential is $V(\mathbf x)=-k/\|\mathbf x\|$. The physical atom has $d=3$, $m$ the reduced mass of electron and proton, and $k=e^2/(4\pi\varepsilon_0)$; the formalization allows any real $k$, attractive when positive. [1] The Hamiltonian is the sum of the kinetic operator $(2m)^{-1}\mathbf p^2$ and the operator of multiplication by $V$, as partially defined operators on the Hilbert space of square-integrable functions on $d$-dimensional space. [2] For the general theory of such operators see the operator-algebra map {1} and for the Hilbert space see the map {2}.

The potential is singular at the origin, so the Hamiltonian is also considered in a regularized form in which $r$ is replaced by $\sqrt{r^2+\varepsilon^2}$ with $\varepsilon\neq 0$. This "soft-core" or truncated Coulomb potential is a standard device {3}{4}. [3] The unregularized Hamiltonian is densely defined in every dimension, because its domain contains the Schwartz functions satisfying a mild bound at the origin, and for $d\geq 3$ this is every Schwartz function. [4]

That the Hamiltonian is essentially self-adjoint for $d\geq 3$ and not essentially self-adjoint for $d<3$ is not yet proved. [TODO] That the closure of the Hamiltonian has point spectrum exactly the Bohr levels below, and continuous spectrum on the non-negative half line, is not yet proved. [TODO]

### Bohr levels and the Rydberg formula

The scale of the spectrum is the Rydberg energy $\mathrm{Ry}=mk^2/(2\hbar^2)$. The expected bound-state energies are $E_n=-\mathrm{Ry}/(n+(d-1)/2)^2$ for $n=0,1,2,\dots$; in three dimensions the shifted index is $n+1$, the usual principal quantum number {5}{6}. The levels are non-positive, are strictly negative for $d\geq 2$ and $k\neq 0$, and increase strictly with $n$. [5] These formulas define the levels and are proved independently of the Hamiltonian; the sections below show that they occur as eigenvalues of it.

The photon emitted when the atom drops from level $n_2$ to $n_1$ carries the energy difference, and so has frequency $\nu=(E_{n_2}-E_{n_1})/h$ and wavelength $c/\nu$. This gives the Rydberg formula $\nu=R_\nu\,(1/L_{n_1}^2-1/L_{n_2}^2)$ with $R_\nu=\mathrm{Ry}/h$ and $L_n=n+(d-1)/2$, and its wavenumber form $1/\lambda=(R_\nu/c)(1/L_{n_1}^2-1/L_{n_2}^2)$. As $n_2\to\infty$ the frequency tends to the series limit $R_\nu/L_{n_1}^2$. The Lyman, Balmer and Paschen series are the transitions to the first, second and third level, and for $d\leq 5$ every Balmer line lies below every Lyman line. [6]

### The Laplace–Runge–Lenz vector

The Coulomb problem has a hidden symmetry beyond rotations: the Laplace–Runge–Lenz vector $\mathbf A$, which in three dimensions is $\tfrac12(\mathbf p\times\mathbf L-\mathbf L\times\mathbf p)-mk\,\hat{\mathbf r}$, is conserved {6}. In $d$ dimensions it is the family of operators $A_i=\tfrac12(p_jL_{ij}+L_{ij}p_j)-mk\,x_i/r$, defined for the regularized potential. [7] It transforms as a vector under the angular momenta $L_{ij}$, and it is orthogonal to the angular momentum, in the sense that the cyclic combination $L_{ij}A_k+L_{jk}A_i+L_{ki}A_j$ vanishes. [8] Its components do not commute: the commutator of two of them is a multiple of the angular momentum, with a coefficient proportional to the Hamiltonian. Its square is $2mH\,(\mathbf L^2+\tfrac14\hbar^2(d-1)^2)+m^2k^2$, and the Hamiltonian commutes with $\mathbf A$. The orthogonality holds exactly, and the other identities hold with explicit correction terms proportional to $\varepsilon^2$, which vanish as the regularization is removed; the limit $\varepsilon\to0$ itself is not taken. [9] [TODO] The conservation of $\mathbf A$ and the commutation relations for the unregularized operators on their natural domain are not yet formalized.

### The radial equation and its quantisation

For a state of angular momentum quantum number $l$, write the wave function as $u(\rho)/\rho$ times an angular part, with $\rho$ the distance in units of the Bohr radius $a=\hbar^2/(mk)$. In units where the energy is $-\kappa^2$ Rydbergs, the reduced radial function solves $u''=\big(l(l+1)/\rho^2-2/\rho+\kappa^2\big)u$ on the half line. The bound-state solutions are $u_{\nu l}(\rho)=\rho^{l+1}e^{-\rho/\nu}L_{\nu-l-1}^{(2l+1)}(2\rho/\nu)$ with principal quantum number $\nu>l$ and $L$ the generalized Laguerre polynomial; they are not normalized. The radial wave function is $R_{\nu l}=u_{\nu l}/\rho$. [10] These are the standard radial functions of the hydrogen atom {5}{6}{7}. The functions $u_{\nu l}$ solve the radial equation with $\kappa=1/\nu$. [11] In physical units, for $d=3$ and attractive $k$, they solve $-\frac{\hbar^2}{2m}u''+\big(\frac{\hbar^2l(l+1)}{2mr^2}-\frac kr\big)u=Eu$ with $E=-\mathrm{Ry}/\nu^2$, the Bohr level from the previous section. [12]

The expectation values of inverse powers of the radius in these states, taken as quotients by the squared norm, are $\langle 1/\rho\rangle=1/\nu^2$, $\langle 1/\rho^2\rangle=1/(\nu^3(l+\tfrac12))$ and, for $l\geq 1$, $\langle1/\rho^3\rangle=1/(\nu^3\,l(l+\tfrac12)(l+1))$. The squared radial function at the origin of an $s$ state, relative to the squared norm of $u$, is $4/\nu^3$. [13]

Quantisation of the energy follows from normalizability. Take the ansatz $\rho^{l+1}e^{-\kappa\rho}$ times an everywhere convergent power series; the radial equation then forces a recursion between its coefficients. [14] If the series terminates, it is a Laguerre polynomial and the solution is a multiple of $u_{\nu l}$ with $\kappa=1/\nu$ for a natural number $\nu>l$; if it does not terminate, the solution grows and is not square integrable. Hence a square-integrable solution of this form exists only at the Bohr levels. [15] The power-series form need not be assumed: every solution which tends to zero at the origin is of this form, by a Wronskian argument with the regular solution, so the quantisation holds for any square-integrable solution of the radial equation that vanishes at the origin. [16] [TODO] That vanishing at the origin is the physical boundary condition, because the second solution is singular there and the resulting wave function is not in the domain of the Hamiltonian, is not yet formalized.

### Bound-state wave functions

In $d\geq 2$ dimensions the angular part of a state of angular momentum $l$ is a homogeneous harmonic polynomial $P$ of degree $l$; in three dimensions these are the solid harmonics $r^lY_{lm}$. For a radial function $f$ the Laplacian of $f(r)P$ away from the origin is $(f''+(d-1+2l)f'/r)P$, and the radial factor $e^{-\kappa r}L_N^{(2l+d-2)}(2\kappa r)$ solves the corresponding radial equation by the Laguerre equation. [17]

The bound state $\psi=e^{-\kappa r}L_N^{(2l+d-2)}(2\kappa r)\,P(\mathbf y)$, with decay constant $\kappa=1/(a(n+(d-1)/2))$ and $n=N+l$, satisfies $-\frac{\hbar^2}{2m}\Delta\psi-\frac kr\psi=E_n\psi$ at every point away from the nucleus, with $E_n$ the Bohr level. The $s$ states ($P=1$) and $p$ states ($P=y_j$) are the first examples. [18]

This is a pointwise statement about a smooth function away from the origin. It does not say that these are all the eigenfunctions, nor that they lie in the domain of the Hamiltonian as an operator. [TODO] The bound states are not smooth at the nucleus; to apply the Hamiltonian to them one uses regularized versions $\psi_\varepsilon$ whose radius is replaced by $\sqrt{r^2+\varepsilon^2}$. On the domain of the Hamiltonian its action is the differential expression $-\frac{\hbar^2}{2m}\sum_i\partial_i^2+V$ almost everywhere. [19] Green's identity, which moves the Laplacian from a Schwartz function onto a bound state, holds for smooth functions of polynomial growth and, by dominated convergence in the limit $\varepsilon\to0$, for the bound states themselves. [20][21] [TODO] That the bound states are eigenvectors of the adjoint of the Hamiltonian with the Bohr eigenvalue, that is, the weak eigenvalue equation, is not yet formalized.

The bound states are square integrable, so they define vectors of the Hilbert space of square-integrable functions on $d$-dimensional space. [22] [TODO] That the bound states of all levels exhaust the point spectrum is not yet formalized.

### Degeneracy of the levels

The homogeneous harmonic polynomials of degree $l$ in $d\geq 2$ variables form a space of dimension $\binom{l+d-1}{d-1}-\binom{l+d-3}{d-1}$, which is $2l+1$ in three dimensions {9}, and every such polynomial gives a bound state at the level $n=N+l$. [23] The bound states of one level $n$, built from polynomials of degrees $l=0,\dots,n$, are linearly independent, so the level carries at least $\sum_{l\leq n}(2l+1)=(n+1)^2$ independent eigenfunctions in three dimensions. [24] The same independence holds as vectors of the Hilbert space, over the real and over the complex numbers, so the bound states of the level span a complex subspace of dimension $(n+1)^2$ in three dimensions. [25] [TODO] That the degeneracy is exactly $(n+1)^2$, with no further eigenfunctions, is not yet formalized.

### Pauli's algebraic derivation

Pauli obtained the spectrum from the commutation relations alone {8}. On an eigenspace of the Hamiltonian with eigenvalue $E<0$ the rescaled vector $\mathbf K=\mathbf A/\sqrt{-2mE}$ makes $\mathbf J_\pm=(\mathbf L\pm\mathbf K)/2$ two commuting copies of the angular momentum algebra, which is the $\mathfrak{so}(4)$ symmetry of the Coulomb problem {6}. The relations $\mathbf L\cdot\mathbf A=0$ and the formula for $\mathbf A^2$ make the Casimir of each copy the scalar $-(\hbar^2+mk^2/(2E))/4$.

The argument is formalized for operators on an arbitrary complex vector space in three dimensions that satisfy the hydrogen relations at $\varepsilon\to0$. [26] It shows that every non-zero finite-dimensional eigenspace of $H$ with negative eigenvalue $E$ has $E$ equal to a Bohr level, and that its dimension is at least $(n+1)^2$ at the level with principal quantum number $n+1$. [27] The step that realizes the Pauli relations by the actual hydrogen operators on a function space is not formalized. [TODO]

### Fine structure

At first order in $\alpha=k/(\hbar c)$ the level $(\nu,l)$ is shifted by three relativistic corrections: the relativistic kinetic energy $-\langle(E_\nu-V)^2\rangle/(2mc^2)$, the spin–orbit coupling $\frac{k}{2m^2c^2}\langle 1/r^3\rangle\langle\mathbf L\cdot\mathbf S\rangle$, and the Darwin term $\frac{\pi k\hbar^2}{2m^2c^2}|\psi(0)|^2$, which acts only on $s$ states {5}{6}{7}. [28] Evaluated with the radial expectation values above and the eigenvalues of $\mathbf L\cdot\mathbf S$ on the states of total angular momentum $j=l\pm\tfrac12$, the sum is $E_\nu\,\alpha^2\nu^{-2}\big(\nu/(j+\tfrac12)-\tfrac34\big)$ in both cases, so it depends only on $j$. In particular $2s_{1/2}$ and $2p_{1/2}$ remain degenerate at this order. [29] The eigenvalues of $\mathbf L\cdot\mathbf S$ come from the coupling of angular momenta. [30]

The three perturbation operators, the first-order formula $\Delta E=\langle H'\rangle$, the identity $\langle p^4\rangle=4m^2\langle(E-V)^2\rangle$, and $|\psi(0)|^2=|R(0)|^2/(4\pi)$ are taken as physical input rather than derived. [TODO] The derivation of the correction terms from the Dirac equation or the Breit–Pauli Hamiltonian is not formalized. [TODO] The Lamb shift, hyperfine structure, the Zeeman effect and the Stark effect are not formalized. [TODO]

## Lean References

1. Physlib/QuantumMechanics/Hydrogen/Basic.lean — `HydrogenAtom`, `potential_eq`
2. Physlib/QuantumMechanics/SpaceDQuantumSystem.lean — `SpaceDQuantumSystem`,
   `kineticOperator`, `potentialOperator`, `hamiltonianOperator`
3. Physlib/QuantumMechanics/Hydrogen/Basic.lean — `hamiltonianRegCLM`, `hamiltonianRegCLM_eq`
4. Physlib/QuantumMechanics/Hydrogen/Basic.lean —
   `polyBddSchwartzSubmodule_le_hamiltonianOperator_domain`, `hamiltonianOperator_hasDenseDomain`
5. Physlib/QuantumMechanics/Hydrogen/Rydberg.lean — `rydbergEnergy`, `levelIndex`, `energyLevel`,
   `energyLevel_nonpos`, `energyLevel_neg`, `energyLevel_strictMono`
6. Physlib/QuantumMechanics/Hydrogen/Rydberg.lean — `transitionEnergy`, `transitionFrequency`,
   `rydbergFrequency`, `wavelength`, `transitionFrequency_eq`, `wavelength_inv`,
   `tendsto_transitionFrequency`, `lymanFrequency`, `balmerFrequency`, `paschenFrequency`,
   `balmerFrequency_lt_lymanFrequency`
7. Physlib/QuantumMechanics/Hydrogen/LaplaceRungeLenzVector.lean — `lrlOperator`, `lrlOperator_eq'`
8. Physlib/QuantumMechanics/Hydrogen/LaplaceRungeLenzVector.lean —
   `angularMomentum_commutation_lrl`, `angularMomentum_cyclic_lrl`, `lrl_cyclic_angularMomentum`
9. Physlib/QuantumMechanics/Hydrogen/LaplaceRungeLenzVector.lean — `lrl_commutation_lrl`,
   `hamiltonianReg_commutation_lrl`, `lrlOperatorSqr_eq`
10. PhyslibAlpha/QuantumMechanics/Hydrogen/RadialFunctions.lean — `radialPoly`, `radialU`,
    `radialR`, `radialU_eq_mul_radialR`
11. PhyslibAlpha/QuantumMechanics/Hydrogen/RadialFunctions.lean — `radialU_ode`
12. PhyslibAlpha/QuantumMechanics/Hydrogen/RadialFunctions.lean — `bohrRadius`, `radialFun`,
    `radialFun_schrodinger`
13. PhyslibAlpha/QuantumMechanics/Hydrogen/RadialFunctions.lean — `radialMoment`, `radialMean`,
    `radialMoment_zero`, `radialMean_one`, `radialMean_two`, `radialMean_three`,
    `radialR_zero_sq_div`
14. PhyslibAlpha/QuantumMechanics/Hydrogen/RadialQuantization.lean — `radialSeries`,
    `recursion_of_radial_ode`
15. PhyslibAlpha/QuantumMechanics/Hydrogen/RadialQuantization.lean —
    `radialSeries_eq_of_terminating`, `not_integrableOn_of_nonterminating`, `radial_quantization`
16. PhyslibAlpha/QuantumMechanics/Hydrogen/RadialCompleteness.lean — `radialPot`, `regCoeff`,
    `radial_ode_of_radialRec`, `wronskian_eq_zero_of_tendsto`, `radial_regular_solution`,
    `radial_quantization_of_tendsto`
17. PhyslibAlpha/QuantumMechanics/Hydrogen/Eigenfunctions.lean — `laplacian_radial_mul`,
    `laplacian_radial_harmonic`, `radialFactor`, `radialFactor_ode`
18. PhyslibAlpha/QuantumMechanics/Hydrogen/Eigenfunctions.lean — `boundKappa`, `boundState`,
    `boundState_eigen`, `boundState_eigen_s`, `boundState_eigen_p`
19. PhyslibAlpha/QuantumMechanics/Hydrogen/BoundStatesAdjoint.lean — `laplacian_regBoundState`,
    `boundState_eq_regG`, `hamiltonianOperator_apply_ae`
20. PhyslibAlpha/QuantumMechanics/Hydrogen/GreenIdentity.lean —
    `integral_ofReal_mul_sum_deriv_deriv`, `regG`
21. PhyslibAlpha/QuantumMechanics/Hydrogen/BoundStatesAdjoint.lean —
    `integral_regBoundState_mul_sum_deriv_deriv`, `integral_boundState_mul_sum_deriv_deriv`
22. PhyslibAlpha/QuantumMechanics/Hydrogen/BoundStatesL2.lean — `memHS_boundState`,
    `boundStateHS`
23. PhyslibAlpha/QuantumMechanics/Hydrogen/Degeneracy.lean — `harmonicSubmodule`,
    `finrank_harmonicSubmodule`, `finrank_harmonicSubmodule_three`,
    `boundState_eigen_of_mem_harmonicSubmodule`
24. PhyslibAlpha/QuantumMechanics/Hydrogen/Degeneracy.lean — `boundStateMap`,
    `boundStateMap_injective`, `finrank_range_boundStateMap`,
    `finrank_range_boundStateMap_three`
25. PhyslibAlpha/QuantumMechanics/Hydrogen/BoundStatesL2.lean — `boundStateMapHS_injective`,
    `finrank_range_boundStateMapHS_three`, `finrank_span_range_boundStateMapHS_three`
26. PhyslibAlpha/QuantumMechanics/Hydrogen/PauliSpectrum.lean — `PauliSystem`
27. PhyslibAlpha/QuantumMechanics/Hydrogen/PauliSpectrum.lean — `exists_energyLevel`,
    `exists_energyLevel_le_finrank`
28. PhyslibAlpha/QuantumMechanics/Hydrogen/FineStructure.lean — `fineStructureConstant`,
    `relativisticShift`, `spinOrbitShift`, `darwinShift`, `fineStructureShift`
29. PhyslibAlpha/QuantumMechanics/Hydrogen/FineStructure.lean — `fineStructureShift_upper`,
    `fineStructureShift_lower`, `fineStructureShift_upper_eq_lower`
30. PhyslibAlpha/QuantumMechanics/AngularMomentum/SpinOrbit.lean — `spinOrbitValue`,
    `dot_coupled_stringVec`

## References

1. Operator algebra API map — Physlib/QuantumMechanics/Operators/API-map.md
2. Hilbert spaces on space API map — Physlib/QuantumMechanics/HilbertSpaces/SpaceD/API-map.md
3. R. L. Hall, N. Saad, K. D. Sen and H. Ciftci, Energies and wave functions for a soft-core
   Coulomb potential, Physical Review A 80 (2009), 032507, doi:10.1103/PhysRevA.80.032507.
4. R. L. Hall, N. Saad and K. D. Sen, Soft-core Coulomb potentials and Heun's differential
   equation, Journal of Mathematical Physics 51 (2010), doi:10.1063/1.3290740.
5. D. J. Griffiths, Introduction to Quantum Mechanics, 2nd edition, Pearson Prentice Hall (2005),
   reissued by Cambridge University Press (2017): section 4.2 (the hydrogen atom), page 145,
   and section 6.3 (the fine structure of hydrogen), page 266.
6. J. J. Sakurai and J. Napolitano, Modern Quantum Mechanics, 3rd edition, Cambridge University
   Press (2020): section 3.7.4 (the Coulomb potential), section 4.1.4 (SO(4) symmetry in the
   Coulomb potential), sections 5.3.1 and 5.3.2 (relativistic correction and spin–orbit
   interaction in hydrogenlike atoms).
7. H. A. Bethe and E. E. Salpeter, Quantum Mechanics of One- and Two-Electron Atoms, Springer,
   Berlin (1957), doi:10.1007/978-3-662-12869-5.
8. W. Pauli, Über das Wasserstoffspektrum vom Standpunkt der neuen Quantenmechanik,
   Zeitschrift für Physik 36 (1926), 336–363, doi:10.1007/BF01450175.
9. S. Axler, P. Bourdon and W. Ramey, Harmonic Function Theory, 2nd edition, Graduate Texts in
   Mathematics 137, Springer (2001), chapter 5 (harmonic polynomials),
   doi:10.1007/978-1-4757-8137-3_5.
