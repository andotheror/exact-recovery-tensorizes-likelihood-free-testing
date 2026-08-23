# Exact Recovery Tensorizes Likelihood-Free Testing

## Abstract

Likelihood-free testing classifies one target using samples from two unknown reference distributions. What is the cost of classifying many targets exactly when reference samples can be shared and sampling can be fully adaptive? A recent distribution-clustering result answers this question up to a factor $\log K$. We close the gap. For $K$ targets over an $N$-symbol alphabet, separation $\varepsilon$ in total variation, and exact-recovery error $\delta$, the minimax total sample complexity for arbitrary discrete distributions is 

$$\Theta\\!\left(\begin{aligned} &\frac{K\log(K/\delta)}{\varepsilon^2} +\frac{\sqrt{NK\log(K/\delta)}}{\varepsilon^2}\\\\ &\quad+\left(\frac{N^2K\log(K/\delta)}{\varepsilon^4}\right)^{1/3} \end{aligned}\right).$$

 The cubic term disappears for uniformly bounded probability masses, and both nuisance-estimation terms disappear when the references are known. The lower bound holds even when the two class sizes are known, the targets arrive in revealed pairs containing one member of each class, and the algorithm allocates samples adaptively. The proof introduces a directed adaptive tensorization lemma. Neighboring wrong outputs have total probability at most $\delta$, while a capped changed pair receives only $O(T/K)$ samples on average. Joint convexity of binary relative entropy then forces one capped likelihood-free experiment to carry $\Omega(\log(K/\delta))$ information. Dense Paninski and sparse Poisson-mixture priors produce the square-root and cubic phases. The result shows that the union-bound logarithm in exact likelihood-free classification is minimax, rather than an artifact of testing targets separately.

## Contributions

- an adaptive exact-recovery tensorization lemma for experiments with a shared nuisance distribution
- the exact finite-confidence minimax rates for known, bounded discrete, and unrestricted discrete references
- lower bounds that retain known balanced class sizes and revealed opposite-label pairings
- a direct resolution of the classification-stage logarithmic gap in

## Keywords

likelihood-free hypothesis testing, tensorization, exact recovery, sample complexity, two-sample testing, minimax rates

## Files

- `main_old_2026-08-12.pdf`, the paper as first published, with its OpenTimestamps proof `main_old_2026-08-12.pdf.ots`.
- `supplement_old_2026-08-12.pdf`, the supplement as first published, with its OpenTimestamps proof `supplement_old_2026-08-12.pdf.ots`.
- source: `aistats2027.sty`, `main.tex`, `references.bib`, `supplement.tex`.
- also: `main.bbl`, `supplement.bbl`.
