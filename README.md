# RFdiffusion Generative Evaluation

## Project Summary

RFdiffusion is a denoising diffusion model built on RoseTTAFold that generates protein backbone structures under various structural and functional constraints. In this work, we:

1. **Unconditionally** generate novel protein backbones and assess their structural plausibility.  
2. **Calibrate diffusion steps** to understand trade‑offs between sampling quality and computational cost.  
3. **Design symmetric oligomers** (e.g., C4, D2) by enforcing group symmetries during generation.  
4. **Create hotspot‑guided binders** by conditioning the diffusion process on specific residue contacts.  

Our evaluation measures metrics such as pLDDT confidence scores and backbone RMSD, and compares performance across different tasks. Full details—including methodology, results, and discussion—are in the report. :contentReference[oaicite:0]{index=0}:contentReference[oaicite:1]{index=1}

## Contents

- **`CSIC689_Final_Report.pdf`**  
  Detailed write‑up of background, methodology, experiments, results, and future directions. :contentReference[oaicite:2]{index=2}:contentReference[oaicite:3]{index=3}  
- **`rfdiffusion.ipynb`**  
  Jupyter notebook implementing all experiments:  
  1. Unconditional protein generation  
  2. Diffusion step calibration  
  3. Symmetric oligomer construction  
  4. Hotspot‑guided binder design  

## Prerequisites

- **Python 3.8+**  
- **PyTorch 1.12+**  
- **Conda** (recommended) or **venv**  
- Structural biology libraries: **biopython**, **mdtraj**, **nglview**

## Installation

1. **Clone this repo**  
   ```bash
   git clone https://github.com/your‑org/rfdiffusion‑eval.git
   cd rfdiffusion‑eval
