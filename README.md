# Fault-tolerant quantum computation on a line from one fixed translation-invariant rule

Seth Douglas and Nidhal Mghirbi. Preprint, version 1.1.0, November 2026. [Archive DOI](https://doi.org/10.5281/zenodo.24357734) (all versions); version 1.0.0: [10.5281/zenodo.24357735](https://doi.org/10.5281/zenodo.24357735); version 1.1.0: [10.5281/zenodo.24453268](https://doi.org/10.5281/zenodo.24453268)

## Abstract

One fixed finite-range, translation-invariant, time-periodic quantum circuit on a one-dimensional ring samples the computational-basis output of any width-n, depth-D Toffoli/Hadamard circuit on the all-zero input within total variation error ε. The ring size and number of periods are at most A(n+D+log₂(1/ε))^A for a fixed A, and the per-site register is fixed. The polynomial-time computable product preparation puts the program in classical basis registers and initializes all quantum registers to zero; a deterministic polynomial-time classical decoder uses only n, D and a sufficient integer precision request. Independent wire depolarization or whole-site replacement acts after every elementary layer, including on classical control, below a fixed positive threshold. Theorem D extends the accuracy and polynomial resource bounds to sufficiently small general local fault-path noise, including coherent errors and correlated bath interactions satisfying a fault-path superset bound. Its threshold is positive but astronomically small. The proof combines exact recovery on certified supports, multiscale dense-witness counting for overlapping long tests, and the established fault-path superset method. Noiseless recursive encoding and recovery give the corresponding reference-entangled input/output guarantee. An elementary register-bank corollary replaces the periodic word by one fixed channel at every step, preserves noise after every original layer, and stores a reference-entangled qubit with fidelity at least 15/16 through a horizon linear in ring size. Its ideal onsite bank shift is a noiseless timing structure; noise within a decomposition of that shift and times beyond the horizon are not covered. The construction follows the one-dimensional route proposed by Dünnweber, Styliaris and Trivedi for their two-dimensional construction, which already treats general local fault-path noise with polylogarithmic overhead. Our overhead is polynomial, with very large constants and an initialized synchronous hierarchy.

## Results

Theorem numbers refer to `paper/main.pdf`.

- **Theorem A.** One fixed, finite-range, translation-invariant, time-periodic quantum circuit on a ring, with independent depolarizing noise on every wire after every elementary layer, including all classical control, below a fixed positive threshold, runs any width-n, depth-D Toffoli/Hadamard circuit from a computable product preparation to output error at most ε, with space and time at most A(n + D + log₂(1/ε))^A, read out by a deterministic classical decoder.
- **Theorem B.** With noiseless recursive encoding and recovery at the endpoints, the same hardware preserves arbitrary input entanglement with a reference through the computation.
- **Theorem C.** Independent whole-site replacement noise has a common positive threshold on the same hardware.
- **Theorem D.** The same circuit keeps its preparation, decoder, polynomial resource bound and requested accuracy under general local fault-path noise of strength at most a fixed η₀ > 0 (independent of n, D and ε), including arbitrary CPTP gate replacements within η₀ of the ideal gate in diamond norm, coherent errors and correlated bath interactions satisfying the fault-path superset bound. The threshold is positive but astronomically small.
- **Corollary (one fixed channel).** An elementary register-bank construction gives one fixed translation-invariant channel applied identically at every step with the same computation and resources, keeping the noise after every original layer, and stores a reference-entangled qubit with fidelity at least 15/16 through a horizon linear in the ring size. Its ideal onsite bank shift is a noiseless timing structure; noise inside a decomposition of that shift, and times beyond the horizon, are not covered.

Prior work, as the paper credits it: this is a one-dimensional analogue of the two-dimensional construction of Dünnweber, Styliaris and Trivedi, which has polylogarithmic overhead; ours is polynomial. The classical hierarchy is that of Gács, through the authors' one-dimensional noise-diagram construction (version 2.1.0, doi:10.5281/zenodo.24408026), and the quantum gadgets and one-dimensional memory interface are those of the authors' quantum storage paper (version 3.1.0, doi:10.5281/zenodo.24431439). The general-noise theorem uses the fault-path superset method of Aliferis, Gottesman and Preskill; Dünnweber, Styliaris and Trivedi already treat this noise model in two dimensions, and what is new here is the dense-witness counting for the one-dimensional hierarchy. Pattison, Haah and Preskill (arXiv:2611.23919) give concurrent and independent planar work with streamed instructions and a noiseless global clock.

## Archive contents

- `paper/` contains the manuscript PDF (43 pages), its LaTeX source, the plain-text abstract and build instructions.
- The root contains citation metadata, licensing information and `SHA256SUMS`, the SHA-256 digest of every distributed file except the checksum list itself. Verify it from the archive root with `sha256sum -c SHA256SUMS`.

## Build the paper

From `paper/`, run pdfLaTeX three times without shell escape. The tested engine is MiKTeX-pdfTeX 4.23 (MiKTeX 25.12).

## Citation and license

Douglas, Seth, and Nidhal Mghirbi (2026). *Fault-tolerant quantum computation on a line from one fixed translation-invariant rule*. Version 1.1.0. [Archive DOI](https://doi.org/10.5281/zenodo.24357734) · [Citation metadata](CITATION.cff)

Paper and documentation are licensed under CC BY 4.0. [Licensing details](RIGHTS.md)
