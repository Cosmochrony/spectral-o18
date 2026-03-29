This repository contains the source of the **O18** Cosmochrony paper  
[*Minimal Fibre Structure of the Non-Injective Projection from Born–Infeld Indiscernability:
Derivation of the Parity Involution*](out/SpectralO18.pdf).

This work extends the **spectral admissibility sub-programme** by resolving the
final structural gap left by **O17**:

> Why is the minimal fibre of the projection Π given by conjugate pairs, and can this be derived from first principles?


# Context

**O17** established that:

- conjugate Weil blocks $(c, q-c)$ carry identical dynamics
- the pair observable  
  $\sigma_{\mathrm{pair}}(n) = \sigma_c(n)\,\sigma_{q-c}(n)$
  is the correct physical observable
- the exponent doubling  
  $\delta_{\mathrm{pair}} = 2\,\delta_c$
  is structurally derived

However, O17 left one fundamental open problem:

- why conjugate pairs define the **minimal fibres of the projection Π**

This identification was:

- structurally consistent
- supported by representation theory
- but not derived from the underlying χ-framework

This defines the scope of O18.


# Core Result

The paper derives the **minimal fibre structure of Π from first principles**.

It proves that:

- the Born–Infeld action is even:
  $S[\chi] = S[-\chi]$
- this implies BI-indiscernability of configurations:
  $\chi \sim -\chi$
- therefore every fibre contains the involution:
  $\{\chi, -\chi\}$

Under a minimality assumption:

> the parity involution is the minimal non-injectivity of Π

Finally, in the Weil realisation:

- the involution is identified with:
  $c \leftrightarrow q-c$

Thus, conjugate pairs are no longer a hypothesis:

> they are the derived minimal fibres of Π.


# Main Structural Results

## 1. Parity of the Born–Infeld action

The action satisfies:

$S_{\mathrm{BI}}[-\chi] = S_{\mathrm{BI}}[\chi]$

because it depends only on:

$F^2 = (D\chi)^2$

This establishes a fundamental symmetry at the χ-level.

## 2. BI-indiscernability

A notion of physical indistinguishability is defined:

- two configurations are BI-indiscernible if
  all BI-admissible responses coincide

This implies:

$\chi \sim -\chi$

Therefore:

> the projection Π must identify parity-related configurations.

## 3. Fibre constraint

From BI-indiscernability:

- every fibre satisfies:
  $\{\chi, -\chi\} \subset \Pi^{-1}(y)$

Thus:

> parity is necessarily contained in every fibre.

## 4. Conditional minimality

Under the assumption:

> parity is the only global effective symmetry compatible with BI-admissible observables

it follows that:

- the minimal fibre is exactly:
  $\{\chi, -\chi\}$

Any larger identification would:

- either introduce additional symmetry
- or be unstable under admissible perturbations

## 5. Weil-level realisation

Using O17:

- $\rho_{q-c} = \overline{\rho_c}$
- conjugate blocks are dynamically indistinguishable

This identifies:

$\chi \leftrightarrow c,\quad -\chi \leftrightarrow q-c$

Therefore:

> the abstract parity involution is realised as  
> $c \leftrightarrow q-c$.


## 6. Closure of the O16–O17 gap

O18 proves that:

- fibre structure is not assumed
- but derived from the Born–Infeld framework

Thus:

> the identification used in O16–O17 is now a theorem.


# Observable Hierarchy (Completed)

With O18, the hierarchy is fully grounded:

- block-level observables (O12–O15)
- pair-level observables (O16–O17)
- fibre structure derived (O18)

The key statement becomes:

> observables are defined on fibres induced by Π,  
> and these fibres are determined by BI-indiscernability.


# Interpretation of the Result

The central conceptual result is:

> non-injectivity of Π is not arbitrary,  
> it is constrained by the Born–Infeld structure.

More precisely:

- projection fibres correspond to physically indistinguishable states
- indistinguishability is governed by BI-admissible responses
- parity is the minimal such identification

Thus, O18 establishes a direct link between:

- Born–Infeld dynamics
- projection structure Π
- observable definition


# Structural Role of O18

O18 completes the full chain:

- **O12–O13**: exact block extraction
- **O14**: observable mismatch
- **O15**: block-level no-go
- **O16**: pair observable (hypothesis)
- **O17**: pair dynamics (derived)
- **O18**: fibre structure (derived)

Thus:

- the observable is justified
- the fibre structure is derived
- the framework is structurally closed


# What O18 Adds

- derivation of parity involution from Born–Infeld structure
- definition of BI-indiscernability
- proof that fibres contain $\{\chi, -\chi\}$
- conditional minimality of the parity fibre
- identification of $c \leftrightarrow q-c$ as its Weil realisation
- closure of the O16–O17 foundational gap


# Outcome

The spectral admissibility framework is now:

- structurally grounded at the fibre level
- consistent with projection non-injectivity
- derived from the χ-level dynamics

The pair observable is now:

- physically justified
- mathematically derived
- no longer an assumption


# Residual Open Problems

The main remaining questions are:

1. **Canonical normalisation (O19)**  
   Remove residual dependence on $(b_1, b_2)$

2. **Spectral window selection (O20)**  
   Explain the restriction to $[7.4, 10.6]$

3. **Full δ → β\* derivation (O21)**  
   Derive the relation at the fibre level without pipeline assumptions

4. **Beyond minimal fibres**  
   Classify fibres in enriched frameworks with additional symmetries

# Status

The programme is now:

- observationally well-defined (**O17**)
- structurally grounded (**O18**)
- free of unresolved foundational assumptions

Remaining work is:

- technical normalisation
- dynamical selection
- extension to full χ-level derivations


# Repository Structure

```text
paper/
├── out/      # Compiled O18 PDF
├── tex/      # LaTeX sources
└── README.md
```
# Citation

If you reference this work, please cite:

J. Beau,
Minimal Fibre Structure of the Non-Injective Projection from Born–Infeld Indiscernability:
Derivation of the Parity Involution, Zenodo, 2026.

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
- Born–Infeld-induced projection structure
- Weil-level realisations

are welcome.

Please open an issue to discuss conceptual points,
technical details, or possible extensions.
