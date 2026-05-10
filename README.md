# PMS-QC — Praxeological Meta-Structure for Quantum Computing

**PMS-QC** is an exploratory research project applying the **[Praxeological Meta-Structure (PMS)](https://github.com/tz-dev/Praxeological-Meta-Structure-Theory)** as a *formal structural and contextual layer* for quantum computing.  

While PMS provides the **canonical operator grammar** (Δ–Ψ) for modelling praxis, asymmetry, contextual framing, isolation, and integration, PMS-QC investigates how these operators can be coherently mapped onto quantum-computational paradigms without reducing them to metaphor or implementation detail.  

In particular, the project explores structural correspondences between PMS operators — operator algebra (Δ–Ψ), frame semantics (□), asymmetry (Ω), isolation (Χ), and integration (Σ) — and quantum-computational structures such as:  

* quantum circuits
* basis and context switching
* superposition and entanglement boundaries
* quantum measurement
* hybrid classical–quantum workflows

The framework explicitly distinguishes between three layers:

* **PMS** — the stable, substrate-independent operator grammar (Δ–Ψ, □, Ω, Χ, Σ)
* **PMS-QC** — a generic quantum-computational structural layer derived from PMS
* **PMS-QC-EXT** — optional, paper- or experiment-specific extensions

Only the **PMS-QC** layer is normative for this repository; all extensions are explicitly non-binding.

PMS-QC thus treats quantum computation not as a purely physical or algorithmic process, but as a **praxeologically structured domain** in which operational coherence, contextual asymmetry, and boundary conditions are explicitly modelled.

This repository contains the conceptual paper (HTML + PDF), minimal CSS styling, YAML-based model/spec layers (`/model`), and dedicated example suites (`/examples`) for both the PMS-QC base layer and the optional PMS-QC_EXT layer.

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.19654589.svg)](https://doi.org/10.5281/zenodo.19654589)

---

## Repository Structure

```text
PMS-QC/
│
├── css/
│   └── main.css                                   # Styling for HTML documents
│
├── examples/
│   ├── qc_examples.html                           # HTML rendering of PMS-QC base example suite
│   ├── qc_examples.yaml                           # PMS-QC base examples (YAML-compatible blocks)
│   ├── qc_ext_examples.html                       # HTML rendering of PMS-QC_EXT example suite
│   └── qc_ext_examples.yaml                       # PMS-QC_EXT examples (YAML-compatible blocks)
│
├── model/
│   ├── Model Specifications PMS-QC.html           # HTML model specification for PMS-QC base layer
│   ├── Model Specifications PMS-QC-EXT.html       # HTML model specification for PMS-QC_EXT layer
│   ├── PMS-QC - Model Specification.pdf           # PDF export of PMS-QC model specification
│   ├── PMS-QC-EXT - Model Specification.pdf       # PDF export of PMS-QC_EXT model specification
│   ├── PMS-QC.yaml                                # PMS-QC base spec layer (macros, constraints, mapping)
│   └── PMS-QC-EXT.yaml                            # Optional addendum / extensions
│
├── PMS Theory as a Structural Layer for Quantum Computing.html
├── PMS Theory as a Structural Layer for Quantum Computing.md
├── PMS Theory as a Structural Layer for Quantum Computing.pdf
│
├── LICENSE-CC-BY-4.0                              # Creative Commons license for the paper/spec prose
├── MIT-LICENSE                                    # MIT license for potential code additions
│
└── README.md                                      # You are here
````

---

## Overview

### ★ What is PMS-QC?

PMS-QC explores **how a unified operator-algebraic system model (PMS)** can serve as:

* a **conceptual OS/VM layer** for quantum computation
* an **intermediate semantic model** bridging classical and quantum execution
* a **frame-based context calculus** compatible with quantum state spaces
* a **policy-aware, structurally constrained** reasoning layer for hybrid systems

The PMS theory provides:

* a compact operator set
  `O = {Δ, ∇, □, Λ, Α, Ω, Θ, Φ, Χ, Σ, Ψ}`
* a compositional operator grammar with dependency constraints
* a hierarchical frame/context model
* a formal system for distinction, transformation, asymmetry, temporality, isolation, integration, and self-binding

The PMS-QC paper demonstrates how these primitives map to quantum algorithm structure.

PMS-QC is methodologically **bounded**. It does not replace quantum mechanics, does not compete with established circuit or mathematical formalisms at the physical level, and does not claim monopoly over high-level structural analysis. Its contribution is a disciplined structural overlay for describing, comparing, annotating, and constraining quantum-computational workflows.

---

## Model Layer (`/model`)

The `/model` folder contains the machine-readable **specification layers** for PMS-QC:

* **`PMS-QC.yaml`** — the generic PMS-QC base overlay, including:

  * operator-to-QC structural mappings
  * generic macro language (`QFRAME`, `QPREP`, `QORACLE_CALL`, `QITERATE`, `QDIFFUSION`, `QFT_ALIGN`, `QMEASURE`, `QSTABILIZE`)
  * structural policies and guardrails
  * minimal base examples
* **`PMS-QC-EXT.yaml`** — the optional, paper-specific refinement layer, including:

  * QPE ladder refinements
  * fixed-point / overshoot-regulated Grover refinements
  * attractor schedule templates
  * measurement-domain refinements
  * optional EXT-only policy refinements
* **`Model Specifications PMS-QC.html`** and **`Model Specifications PMS-QC-EXT.html`** — full human-readable HTML model specifications for both YAML files
* **`PMS-QC - Model Specification.pdf`** and **`PMS-QC-EXT - Model Specification.pdf`** — PDF exports of those model specifications

These model files are intended as a foundation for future tooling (validation, auditing, orchestration support, or compilation-adjacent hooks), without replacing existing QC formalisms.

---

## Example Layer (`/examples`)

The `/examples` folder contains explicit, YAML-compatible example suites for both repository layers:

* **`qc_examples.yaml`** — PMS-QC base examples
* **`qc_examples.html`** — human-readable HTML rendering of the base examples
* **`qc_ext_examples.yaml`** — PMS-QC_EXT examples
* **`qc_ext_examples.html`** — human-readable HTML rendering of the EXT examples

The example suites are designed to make the **base / extension boundary** concrete:

### PMS-QC base examples include:

* minimal Grover rendering
* minimal QPE rendering
* reframing-plus-measurement workflow
* stabilizer-oriented cycle
* entangle-plus-measurement workflow

### PMS-QC_EXT examples include:

* explicit QPE ladder refinement
* centered / regulated Grover refinement
* fixed-point-oriented attractor schedule example
* measurement projection refinement
* attractor-alignment refinement

These examples are structural and documentation-oriented. They are not claims of physical correctness, convergence proofs, or deployment adequacy.

---

## Why PMS for Quantum Computing?

Quantum computation is inherently:

* contextual
* operator-driven
* basis-dependent
* non-local
* relational
* superpositional

The PMS operator set encodes these kinds of transformations at a structural level.

This project highlights alignment between PMS and quantum computation:

| PMS Operator     | Quantum Interpretation (structural)                                            |
| ---------------- | ------------------------------------------------------------------------------ |
| □ (Frame)        | Register / workspace / Hilbert subspace boundary                               |
| Δ (Distinction)  | Distributed alternatives (superposition), state marking, subspace distinctions |
| Ω (Asymmetry)    | Controlled operations, oracle privilege, measurement asymmetry                 |
| Θ (Temporality)  | Iteration / scheduling / repeated circuit blocks                               |
| Φ (Reframe)      | Basis/context change (e.g., Fourier ↔ computational)                           |
| Χ (Isolation)    | Subsystem separation, boundary discipline, domain isolation                    |
| Σ (Integration)  | Commit boundary before downstream processing / measurement staging             |
| Λ (Non-event)    | Unrealised branches after collapse / excluded outcomes                         |
| Α (Attractor)    | Alignment / convergence patterns (e.g., amplitude amplification motifs)        |
| Ψ (Self-binding) | Invariants, stabilisation, error-correction / governance constraints           |

All interpretations presented here are structural and descriptive; they do not replace quantum-mechanical formalisms, gate semantics, or physical correctness criteria.

---

## Included Documents

### Main paper

The repository contains the full paper in three formats:

* **HTML (`.html`)** — browser-ready version styled via `css/main.css`
* **Markdown (`.md`)** — clean, version-controlled, GitHub-friendly source
* **PDF (`.pdf`)** — print-ready format for citation, distribution, or academic review

All formats contain the paper:

> **“PMS Theory as a Structural Layer for Quantum Computing”**

### Model specifications

The repository also contains dedicated model specification documents for both YAML layers:

* **PMS-QC base model specification**

  * HTML
  * PDF
* **PMS-QC_EXT model specification**

  * HTML
  * PDF

These documents restate the YAML layers in explicit prose, tables, macro inventories, policy summaries, and boundary conditions for human readers.

### Example specifications

The repository further includes HTML + YAML example suites for:

* **PMS-QC base examples**
* **PMS-QC_EXT extension examples**

Together, the paper, model specs, and example suites form a complete repository stack for theory, formal schema, and example-level structural rendering.

---

## Layer Discipline

A central principle of this repository is **strict layer separation**:

* **PMS** remains the canonical operator grammar
* **PMS-QC** defines the generic QC structural overlay
* **PMS-QC-EXT** remains optional and paper-specific

This means in practice:

* PMS-QC does **not** redefine Δ–Ψ
* PMS-QC does **not** modify the PMS dependency spine
* PMS-QC_EXT does **not** override PMS-QC base semantics
* paper-specific refinements must **not** be silently promoted into the base layer
* compliance with structural policies does **not** imply physical correctness, safety, or deployment readiness

The repository is therefore designed to stay strong in structural clarity while remaining disciplined about boundedness, non-finality, and non-guarantee.

---

## Intended Uses

This repository is intended to support:

* structural documentation of QC workflows
* structural QC analysis and comparison
* meta-compiler annotation layers
* audit-oriented reconstruction of QC processes
* bounded AI–QC policy-layer reasoning
* research into praxeological constraints in quantum architectures
* paper-specific refinement work under explicit EXT discipline

It is **not** intended to provide:

* a replacement for quantum mechanics
* hardware-level safety certification
* physical noise modelling
* performance guarantees
* validated agent governance
* deployment-ready orchestration architecture
* anthropomorphic interpretations of quantum systems

---

## Links & Resources

PMS-QC exists within a broader **praxeological ecosystem** spanning formal operator theory, applied anthropology, executable specifications, and interactive tooling.

The resources below provide different **points of access** into that ecosystem: from canonical PMS grammar definitions and formal papers, to applied models, books, and architecture explorations. Together, they form a coherent reference space rather than independent artifacts.

PMS–AXIOM is part of a broader **praxeological ecosystem** spanning formal operator theory, applied anthropology, governance analysis, and executable specifications.

| Category                | Resource                                                                                                                           | Description                                                                                      |
| ----------------------- | ---------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------ |
| Model website           | [PMS Theory Site](https://pms-theory.netlify.app)                                                                                  | Canonical PMS theory reference                                                                   |
| Book websites           | [Maturity in Practice (EN)](https://maturity-in-practice.netlify.app)                                                              | *Maturity in Practice* — English edition (praxeological anthropology)                            |
|                         | [Reife im Vollzug (DE)](https://reife-im-vollzug.netlify.app)                                                                      | *Reife im Vollzug* — Deutsche Ausgabe                                                            |
|                         | [PMS Stack](https://pms-stack.netlify.app)                                                                                         | PMS-STACK reference architecture                                                                 |
| Amazon                  | [Maturity in Practice (EN)](https://www.amazon.com/dp/B0G4XBKNNR)                                                                  | *Maturity in Practice: A Praxeological Anthropology* — English edition                           |
|                         | [Reife im Vollzug (DE)](https://www.amazon.de/dp/B0G4SPBDQD)                                                                       | *Reife im Vollzug: Eine praxeologische Anthropologie* — Deutsche Ausgabe                         |
|                         | [PMS-STACK](https://www.amazon.com/dp/B0G6G7V38P)                                                                                  | *PMS-STACK — A Praxeological Operating System Architecture*                                      |
| GitHub implementation   | **[PMS-RUST](https://github.com/tz-dev/PMS-RUST)**                                                                                 | Executable PMS-STACK Evidence Spine: Rust kernel, REPL, validation, JSONL, vFS, demos, AI bridge |
| GitHub theory / specs   | [PMS Theory / Repo](https://github.com/tz-dev/Praxeological-Meta-Structure-Theory)                                                 | Canonical PMS grammar, theory, YAML/JSON definitions, and model specification                    |
| GitHub books / analyses | [Maturity-in-Practice](https://github.com/tz-dev/Maturity-in-Practice)                                                             | Book sources & applied praxeological anthropology                                                |
|                         | [PMS-QC](https://github.com/tz-dev/PMS-QC)                                                                                         | PMS-QC — Praxeological Meta-Structure for Quantum Computing                                      |
|                         | [PMS-LOGIC](https://github.com/tz-dev/PMS-LOGIC)                                                                                   | PMS-LOGIC — Structural Responsibility, Logical Limits, and Post-Moral Effects                    |
|                         | [PMS-ANTICIPATION](https://github.com/tz-dev/PMS-ANTICIPATION)                                                                     | PMS-ANTICIPATION — Structural Conditions, Risks, and Viability of Anticipatory Praxis            |
|                         | [PMS-CRITIQUE](https://github.com/tz-dev/PMS-CRITIQUE)                                                                             | PMS-CRITIQUE — From Irritation to Correction: A Praxeological Grammar of Critique                |
|                         | [PMS-EDEN](https://github.com/tz-dev/PMS-EDEN)                                                                                     | PMS-EDEN — Structural Drift from Praxis to Comparison and Reciprocity Loss                       |
|                         | [PMS-SEX](https://github.com/tz-dev/PMS-SEX)                                                                                       | PMS-SEX — From Impulse to Self-Binding: A Praxeological Grammar of Sexuality                     |
|                         | [PMS-CONFLICT](https://github.com/tz-dev/PMS-CONFLICT)                                                                             | PMS-CONFLICT — Conflict as Stabilized Incompatibility: Cost, Binding, and Tragic Non-Integration |
|                         | [PMS-AXIOM](https://github.com/tz-dev/PMS-AXIOM)                                                                                   | PMS-AXIOM — Cartography of Classical Closure-Demands Across the PMS Stack                        |
| Custom GPTs             | [PMS Model Assistant](https://chatgpt.com/g/g-69358a2a4980819183da6a97893389cf-pms-model-assistant)                                | Interactive PMS.yaml exploration & validation                                                    |
|                         | [Maturity in Action](https://chat.openai.com/g/g-693460d3def48191ad08647301645a2e-maturity-in-action-a-praxeological-anthropology) | Applied praxeological anthropology assistant                                                     |

---

## Contributing

Contributions, critiques, and theoretical extensions are welcome.
Please open an issue or submit a pull request.

Contributions should preserve:

* the distinction between PMS base, PMS-QC base, and PMS-QC_EXT
* the non-guarantee discipline of the repository
* the non-anthropomorphic reading of structural renderings
* the methodological boundedness of the project

---

## License

* The **paper** and accompanying specification prose are released under **CC BY 4.0** (`LICENSE-CC-BY-4.0`).
* Any **code** added to this repository is released under the **MIT License** (`MIT-LICENSE`).

---

## Contact

Maintained by **tz-dev**.
For discussions or questions, please use GitHub issues.
