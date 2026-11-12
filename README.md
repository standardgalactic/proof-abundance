# Proof Abundance: Understanding, Attribution, and Reuse

Flyxion, Independent Researcher. November 2026.

This repository holds the LaTeX source of a monograph on what a proof gives its recipient after it has been checked. It is a companion to *Portable Warrant*, which asks when a judgment certified in one setting may be relied on in another. The present work starts at the point of arrival: a certificate has crossed from its source to a recipient, it verifies, and the recipient now holds a proposition that may be used within a stated scope. The question pursued is whether the proof also equips the recipient to make a further mathematical move.

The compiled monograph is available as a PDF at [Proof Abundance](https://standardgalactic.github.io/portable-warrant/proof-abundance.pdf). An audio overview, [Why Automated Verification Does Not Equal Understanding](https://standardgalactic.github.io/portable-warrant/proof-abundance-oscilloscope.html), is published alongside it.

## The idea

The phrase "the use of a proof" has two senses. To use a proof in the first sense is to rely on what it establishes: cite the theorem and proceed within the limits of what was shown. To use it in the second sense is to be equipped by it, to adapt the construction to a neighbouring case, to see which hypothesis carries the weight, and to recognize in advance where a similar argument will fail. The book calls the first reliance and the second continuation. It gives both a common formal frame, with three components: the certified judgment together with the scope in which it may be relied on, the continuation task, which is a further move a reader might want to make, and a resource bound, without which the frame cannot register that a proof teaches a reader anything.

The central formal result is that certified warrant and continuation gain are independent. Within an explicit finite model there are artifacts that supply the first without the second, the second without the first, both, and neither. The result is proved in Appendix B, and the mathematical examples illustrate it without replacing the proof. A running example carries the argument throughout: the infinitude of the primes, established by Euclid's construction and by Euler's analytic argument, together with a family of continuation tasks drawn from primes in arithmetic progressions.

## Structure

The book has four parts. Part I, The Scope of a Proof, treats certified judgments, the fibers of the certification map (what verification forgets), and the transport of warrant between environments, including a case where individually justified transfers compose to an unjustified one. Part II, The Transfer of Mathematical Understanding, defines understanding as a resource-bounded capacity for continuation, treats the relegation of search to routine in mathematical exposition, and proves the independence result for sketches, certificates, and open obligations. Part III, Mathematical Work as a Gift, takes up reciprocity through reuse, attribution and answerability, and the conditions under which early disclosure of work is worthwhile. Part IV, Proof Abundance, asks where the costs of generation, selection, and reuse fall when certified proofs are cheap, and closes with a worked dossier that applies the frame to a single claim and its provenance record.

Three appendices fix the formal details: a syntax for certificates and a separate judgment for scoped reliance, a bounded continuation calculus with explicit witnesses for the independence result, and record forms for checking dependencies, reported transmission, and answerability.

## Building

The document is a single file, `proof-abundance.tex`, with its bibliography included as a `thebibliography` environment, so no BibTeX run is needed. It uses the `book` class and standard packages (amsmath, amssymb, amsthm, mathtools, microtype, booktabs, hyperref, setspace). With a standard TeX Live installation, run

    pdflatex proof-abundance.tex
    pdflatex proof-abundance.tex

Two passes are needed to resolve the table of contents and cross-references.

## Status

This is a working draft, published as it is produced and revised in place. It is dedicated to the public domain.
