# Dual Character Fusion — AI Portrait Generator

> Fine-tuned FLUX LoRA models + ComfyUI workflows to generate unique merged AI portraits from dual character inputs.

🔗 **Project Writeup:** [Notion — MID Capstone](https://www.notion.so/MID-Capstone-Project-2e16618750508106b614c5f1293384e5?source=copy_link)

---

## Overview

Dual Character Fusion is a Generative AI capstone project that explores custom model fine-tuning and complex diffusion workflows. The goal: take two distinct character styles or inputs and generate a unique merged AI portrait that blends both identities into a single coherent image.

This project goes beyond prompt engineering — it involves training custom LoRA models on FLUX, building multi-node ComfyUI workflows, and managing the full diffusion pipeline from conditioning to output.

Built as the **MID Capstone Project** in the Applied GenAI cohort at **100x**.

---

## What I Built

- Fine-tuned custom **FLUX LoRA models** to capture and blend unique character styles
- Designed and managed **complex ComfyUI diffusion workflows** covering:
  - Model loading and LoRA stacking
  - Text and image conditioning
  - Sampler configuration (steps, CFG, scheduler)
  - Output post-processing
- Experimented with different fusion techniques for blending dual character inputs
- Documented results and workflow in a full project writeup

---

## Tech Stack

| Tool | Purpose |
|------|---------|
| ComfyUI | Node-based diffusion workflow builder |
| FLUX LoRA | Base model for fine-tuning |
| Hugging Face | Model hosting and dataset management |
| PyTorch | Model training and fine-tuning backend |

---

## How It Works

```
Input A (Character 1) ──┐
                         ├──► LoRA Fine-tuning ──► ComfyUI Workflow ──► Merged Portrait
Input B (Character 2) ──┘
```

1. Prepare training datasets for each character style
2. Fine-tune FLUX LoRA models on each character
3. Stack LoRA weights in ComfyUI with blended conditioning
4. Run diffusion sampling to generate the merged portrait
5. Iterate on CFG scale, steps, and conditioning weights for best fusion output

---

## Results

> _Add sample generated portraits here (before/after fusion comparison)._

Full project walkthrough and results available in the [Notion writeup](https://www.notion.so/MID-Capstone-Project-2e16618750508106b614c5f1293384e5?source=copy_link).

---

## Key Learnings

- LoRA fine-tuning requires clean, well-curated datasets — garbage in, garbage out
- ComfyUI's node-based architecture gives fine-grained control over every stage of diffusion
- LoRA weight blending ratios heavily influence the fusion output — small changes create dramatically different results
- FLUX outperforms SD 1.5 for character consistency and detail

---

## About the Builder

Built by **Krishna Sahaj D V** — MBA graduate and Generative AI builder with hands-on experience in model fine-tuning, diffusion workflows, and AI product development.

🔗 [LinkedIn](https://www.linkedin.com/in/krishna-sahaj-d-v-7b623b190) • [GitHub](https://github.com/sahajkrishna)
