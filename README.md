# Fault-tolerant quantum computation on a line from one fixed translation-invariant rule

Seth Douglas and Nidhal Mghirbi. Preprint, version 1.0.0, November 2026.

## Abstract

One fixed, finite-range, translation-invariant, time-periodic quantum circuit on a ring performs any width-n, depth-D Toffoli/Hadamard circuit from a computable product preparation, with space and time at most A(n+D+log2(1/ε))^A and output error at most ε. The register per site and A are fixed. Independent depolarizing noise acts on every wire after every elementary layer, including every classical control wire, at any rate below a fixed positive threshold. The target circuit enters only through classical basis registers; all quantum registers start in zero. A deterministic classical decoder, depending only on n,D and a sufficient integer precision request, reads the final computational-basis measurement. A serial quantum processor is embedded in an initialized one-dimensional classical self-simulating hierarchy. Coordinatewise private teleportation corrections load repeated classical words without assuming that they are quantum codewords, and a closed tape-end rule confines faulty instruction decisions to one contact. With noiseless recursive encoding and recovery at the endpoints, the same circuit preserves arbitrary input entanglement with a reference. Independent whole-site replacement has a common positive threshold on the same hardware. This is a one-dimensional analogue of the two-dimensional construction of Dünnweber, Styliaris and Trivedi, following their suggested route through Gács's one-dimensional hierarchy. Our overhead is polynomial rather than polylogarithmic. The hierarchy is initialized and synchronous; the constants are extremely large.

## Results

Theorem numbers refer to `paper/main.pdf`.

- **Theorem A.** One fixed, finite-range, translation-invariant, time-periodic quantum circuit on a ring, with independent depolarizing noise on every wire after every elementary layer, including all classical control, below a fixed positive threshold, runs any width-n, depth-D Toffoli/Hadamard circuit from a computable product preparation to output error at most ε, with space and time at most A(n + D + log₂(1/ε))^A, read out by a deterministic classical decoder.
- **Theorem B.** With noiseless recursive encoding and recovery at the endpoints, the same hardware preserves arbitrary input entanglement with a reference through the computation.
- **Theorem C.** Independent whole-site replacement noise has a common positive threshold on the same hardware.

Prior work, as the paper credits it: this is a one-dimensional analogue of the two-dimensional construction of Dünnweber, Styliaris and Trivedi, which has polylogarithmic overhead; ours is polynomial. The classical hierarchy is that of Gács, through the authors' one-dimensional noise-diagram construction (version 2.0.0, doi:10.5281/zenodo.24352353), and the quantum gadgets and one-dimensional memory interface are those of the authors' quantum storage paper (version 3.0.0, doi:10.5281/zenodo.24354983).

## Archive contents

- `paper/` contains the manuscript PDF (30 pages), its LaTeX source, the plain-text abstract and build instructions.
- The root contains citation metadata, licensing information and `SHA256SUMS`, the SHA-256 digest of every distributed file except the checksum list itself. Verify it from the archive root with `sha256sum -c SHA256SUMS`.

## Build the paper

From `paper/`, run pdfLaTeX three times without shell escape. The tested engine is MiKTeX-pdfTeX 4.23 (MiKTeX 25.12).

## Citation and license

Douglas, Seth, and Nidhal Mghirbi (2026). *Fault-tolerant quantum computation on a line from one fixed translation-invariant rule*. Version 1.0.0. [Citation metadata](CITATION.cff)

Paper and documentation are licensed under CC BY 4.0. [Licensing details](RIGHTS.md)
