# An autonomous four-dimensional quantum memory from a time-independent Toom Lindbladian

Seth Douglas and Nidhal Mghirbi.

Preprint, version 1.0.0, November 2026

DOI: to be assigned

## Abstract

We prove exponential storage for the time-independent four-dimensional Toom dissipative toric code under any sufficiently weak additive finite-range Markovian Lindblad noise generator, including coherent Hamiltonian terms and non-unital dissipation such as amplitude damping. From an encoded start, a decoder reading only the current syndrome has worst-case fidelity at least 1 − C e^(−cL) at every 0 ≤ t ≤ e^(cL), in both CSS sectors and for all six logical qubits entangled with an untouched reference. The coherent threshold applies to the amplitude |h|, not h². For such additive noise this realizes the fully autonomous memory setting of Drechsler, Oreg and Aharonov, with translation invariance when the noise is homogeneous. The correction generator is exact; perturbations of its own jump operators and general non-Markovian baths remain open. Separate stochastic-Pauli theorems give explicit syndrome structure and allow spacetime local stochastic bounded-range multi-qubit and adaptive faults on unit time cells (one inverse correction rate), with a noise law independent of the logical input. On ℤ⁴, the independent-noise syndrome process has exponential component-diameter tails uniformly in time from empty syndrome. The corner convention is related to Pastawski, Clemente and Cirac's rule by x ↦ −x and a uniform X/Z relabelling. The general proof combines Poisson clearance and Toom contours with a coherent protected-region estimate, exact mixed differences and dense-set counting. The thresholds are non-explicit and astronomically small, and the size requirements are astronomically large.

## Results

Theorem numbers refer to `paper/main.pdf`.

- **Theorem 10.1 (general local noise).** For the time-independent four-dimensional Toom correction Lindbladian of the 4D toric code plus any sufficiently weak additive finite-range Markovian Lindblad noise generator, including coherent Hamiltonian terms (threshold on the amplitude |h|) and non-unital dissipation such as amplitude damping, a decoder reading only the current syndrome has worst-case decoded fidelity at least 1 − C e^(−cL) at every deterministic time 0 ≤ t ≤ e^(cL), in both CSS sectors and for inputs entangled with a reference. The correction generator is exact; perturbations of its own jump operators and non-Markovian baths are not covered.
- **Theorem 2.1 (independent Pauli noise).** The same exponential bound under independent single-qubit Pauli noise, the noise model of Drechsler, Oreg and Aharonov, with explicit syndrome structure.
- **Theorem 9.2 (correlated Pauli noise).** The same bound under spacetime local stochastic Pauli noise on unit time cells, allowing bounded-range multi-qubit and adaptive faults, with a noise law independent of the logical input.
- **Theorem 2.2 (infinite lattice).** On ℤ⁴, from an empty syndrome, the independent-noise syndrome process has exponential component-diameter tails uniformly in time.

Prior work, as the paper credits it: the correction rule is Toom's, as proposed for the 4D toric code by Pastawski, Clemente and Cirac (2011), who gave numerical evidence (the conventions differ by x ↦ −x and an X/Z relabelling). Drechsler, Oreg and Aharonov (arXiv:2610.05589) proved thresholds for synchronous and periodically driven versions and posed the time-independent case; they also state that, outside the thermal-equilibrium setting, no rigorous proof of a fully autonomous quantum memory was known. The thermal precedent is the 4D toric code under Davies dynamics (Alicki, Horodecki, Horodecki and Horodecki, 2010). The contour machinery is that of Swart, Szabó and Toninelli; continuous-time stability of monotone systems goes back to Gray (1999) and Bramson and Gray, and Chakraborty and Lee (arXiv:2610.40651) use a related slab comparison for monotone dynamics. Ponarovsky (arXiv:2610.38847) treats synchronous sweep cycles with noiseless classical processing. The method is standard in kind; its application to the non-monotone syndrome dynamics of the 4D toric code is, as far as the authors know, new.

## Archive contents

- `paper/` contains the manuscript PDF (47 pages), its LaTeX source and bibliography, the plain-text abstract and build instructions.
- The root contains citation metadata, licensing information and `SHA256SUMS`, the SHA-256 digest of every distributed file except the checksum list itself. Verify it from the archive root with `sha256sum -c SHA256SUMS`.

## Build the paper

From `paper/`, run pdfLaTeX, BibTeX and pdfLaTeX twice, without shell escape (main.bbl is included, so three pdfLaTeX passes also work). The tested engine is MiKTeX-pdfTeX 4.23 (MiKTeX 25.12).

## Citation and license

Douglas, Seth, and Nidhal Mghirbi (2026). *An autonomous four-dimensional quantum memory from a time-independent Toom Lindbladian*. Version 1.0.0. [Citation metadata](CITATION.cff)

Paper and documentation are licensed under CC BY 4.0. [Licensing details](RIGHTS.md)
