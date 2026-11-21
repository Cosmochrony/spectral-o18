This repository contains the source of the **O18** Cosmochrony paper
*Equivariant Born–Infeld Parity and the Fibre-Identification Problem of the Non-Injective Projection*.

This work belongs to the **spectral admissibility sub-programme** and determines exactly which part of the
fibre-identification problem left open by **O17** the Born–Infeld structure settles:

> Parity acts on the Born–Infeld response family with the character $(-1)^k$ of the derivative order:
> even-order responses are preserved, odd-order responses reversed. It does not, by itself, force the fibres of Π.

**Version 2.4.** Theorem 3.1 (O17 Theorem 2.1 and Corollary 2.3) is restated within O17's toy model; on the real
pipeline the equality $\delta_{q-c}=\delta_c$ for the exact block observable follows from O16's conjugate-block
identity. O17's $r(c,q)$ statement is scoped to its toy model, and the historical value 7.44 is no longer
attributed to O16.


# Context

**Version 2.3.** Withdraws the reciprocal-rate implication and its numerical-window selection.
The action parity, response covariance, countermodel and open fibre-classification problem are unchanged.

**O17** established, within its own toy model, that:

- conjugate Weil blocks $(c, q-c)$ carry identical raw dynamics (on the real O12/O13 pipeline the
  equality of conjugate exponents follows instead from O16's conjugate-block identity for the exact block
  observable)
- the pair observable
  $\sigma_{\mathrm{pair}}(n) = \sigma_c(n)\,\sigma_{q-c}(n)$
  is the correct pair-level observable
- the exponent doubling
  $\delta_{\mathrm{pair}} = 2\,\delta_c$
  is structurally derived

O17 §5.2 left one fundamental open problem:

- why conjugate pairs would define the **minimal fibres of the projection Π**

This identification was structurally consistent and supported by representation theory,
but not derived from the underlying χ-framework.
O18 delimits what its adopted Born–Infeld-type action itself contributes to that problem.


# Core Results

## 1. Parity of the adopted Born–Infeld-type action (proved)

The action satisfies

$S_{\mathrm{BI}}[-\chi] = S_{\mathrm{BI}}[\chi]$

because it depends on $\chi$ only through $F^2 = (D\chi)^2$, the contraction of the gradient with itself.
This is a Born–Infeld-type action of the gradient of $\chi$ adopted by O18 as its own model.
BornInfeld supplies a motivation for non-injectivity and the capacity axiom [A-cap]; it does not derive this
action, and its own Born–Infeld candidate is a functional of a gauge field strength whose relational origin is open.

## 2. Parity covariance of the response family (proved)

For the parity map acting simultaneously on configuration and probe,
$(\chi, \eta) \mapsto (-\chi, -\eta)$, a response of derivative order $k$ (a $k$-th functional
derivative of $S_{\mathrm{BI}}$ contracted with fixed admissible test directions) satisfies

$R[-\chi - \epsilon\eta] = (-1)^k\, R[\chi + \epsilon\eta]$

for all admissible probes $\eta$.
Even-order responses (the action among them) are preserved under the transported-probe comparison;
odd-order responses — the first-order response of the action included — reverse sign and generically
separate $\chi$ from $-\chi$.
The orbit $\{\chi, -\chi\}$ is therefore a **candidate** fibre only relative to a supplied restriction
of the observable family to even-order responses.

## 3. Evenness does not force fixed-probe indiscernibility (no-go, proved)

An explicit even countermodel, $R(x) = x^2$ with $\chi = 1$, $\eta = 1$, gives

$R(1+\epsilon) = (1+\epsilon)^2 \neq (1-\epsilon)^2 = R(-1+\epsilon)$,

so an even response can separate $\chi$ from $-\chi$ under one and the same perturbation.
Evenness of the action therefore does not place the parity orbit inside the fibres of any
projection defined by fixed-probe indiscernibility.

## 4. The fibre-identification problem, typed (posed, open)

A derivation of the fibre structure of Π must supply:

- **(D1)** the configuration space with its boundary conditions
- **(D2)** the group of candidate transformations and the prior quotients
- **(D3)** the complete separating family of response functionals, with the comparison
  convention (fixed-probe or transported-probe) fixed once for the whole family and any restriction
  to even-order responses stated explicitly
- **(D4)** a factorisation theorem identifying response equivalence with the fibre
  partition of Π

The absence-of-further-symmetries hypothesis, called **(H-rank)** in downstream papers, is a
clause of this problem, not a theorem and not yet a classifiable statement on its own:
before (D1)–(D3) are supplied, the class of transformations over which "only" quantifies is
undefined.
The derivative-only action moreover has the constant-shift symmetries $\chi \mapsto \chi + a$
unless boundary conditions or a prior quotient remove them.

## 5. Weil level: spectral equivalence, open bridge

Using O17:

- $\rho_{q-c} = \overline{\rho_c}$ proves a **spectral equivalence** of blocks $c$ and $q-c$
- the correspondence $\chi \leftrightarrow c$, $-\chi \leftrightarrow q-c$ — i.e. that the
  two blocks form one **physical fibre** of Π — is an **open bridge**: a structural
  candidate, spectrally supported, not derived


# Status of the Pair-Level Programme

- block-level observables (O12–O15): derived
- pair dynamics $\delta_{q-c} = \delta_c$: derived in O17's toy model for the raw counts; on the real
  pipeline from O16's conjugate-block identity for the exact block observable
- pair observable as fibre observable (O16–O18): **structurally motivated hypothesis**,
  spectrally supported, awaiting a solution of the fibre-identification problem

O6 proves only $\beta_{\mathrm{eff}}\leq1/(\alpha+1/2)$ under its effective growth hypothesis
(G_R) and a power-law redundancy Ansatz in the exploration variable $p$.
Its countermodel $\alpha=8$, $p=n^{1/17}$ satisfies those premises but refutes equality.
The reciprocal is retained only as a defined legacy diagnostic; the historical range $[7.4,10.6]$
is neither a necessary nor a sufficient condition selecting the charged-lepton cascade window.

The fibre identification does not restore the withdrawn equality.
A supplied pair exponent near 7.44 defines only the comparison value $1/(7.44+1/2)\approx0.126$.


# Residual Open Problems

1. **Fibre-identification problem**
   Supply (D1)–(D4) and classify the effective symmetries of $S_{\mathrm{BI}}$.

2. **Weil-level bridge**
   Derive $\chi \leftrightarrow c$, $-\chi \leftrightarrow q-c$ from χ-space variables.

3. **Canonical normalisation (O19)**
   Remove residual dependence on $(b_1, b_2)$.

4. **Persistence comparison (O20)**
   Assess its symbolic threshold interval independently of the historical range $[7.4,10.6]$;
   no physical restriction to that range follows from the O6 upper bound.


# Repository Structure

```text
paper/
├── out/      # Compiled O18 PDF (generated by compile.sh, git-ignored)
├── tex/      # LaTeX sources
└── README.md
```

# Citation

If you reference this work, please cite via the Zenodo concept DOI:

J. Beau,
*Equivariant Born–Infeld Parity and the Fibre-Identification Problem of the Non-Injective Projection*,
Zenodo, 2026. [doi:10.5281/zenodo.19321413](https://doi.org/10.5281/zenodo.19321413)

# Acknowledgements

Portions of the derivations, conceptual synthesis, numerical strategy,
and editorial refinement benefited from iterative interactions with
large language models used as analytical assistants.
All theoretical results, computations, and interpretations remain the
sole responsibility of the author.

# Contributions

This repository is intended as a research reference.

Critical feedback, independent verification, and further analysis of:

- fibre-level admissibility
- Born–Infeld parity covariance
- Weil-level realisations

are welcome.

Please open an issue to discuss conceptual points,
technical details, or possible extensions.
