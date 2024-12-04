# Multi-Stage QLoRA with Augmented Structured Dialogue Corpora: Efficient and Improved Conversational Healthcare AI

This repository contains the code, datasets, and methodology for **Med-Nirvana 8B**, a cost-effective and powerful conversational healthcare AI developed using **QLoRA supervised fine-tuning (SFT)**.

## Overview

Large language models (LLMs) typically require significant computational resources for full fine-tuning. To address this challenge, we employed a **two-stage QLoRA-based fine-tuning process** using the open-source **LLaMA 3.1 8B Instruct model**.

### Fine-Tuning Process

1. **Stage 1: Medical Knowledge and Reasoning**
   - Fine-tuning was conducted using a mixture of medical benchmark datasets:
     - **MedQA**
     - **MedMCQA**
     - **PubMedQA**
   - Focus: Enhance factual knowledge, reasoning, and decision-making skills in a structured environment.

2. **Stage 2: Real-Life Scenario Training**
   - Fine-tuned with the **NoteChat dataset**, consisting of synthetic patient-physician conversations.
   - Focus: Equip the model to handle complex real-life situations, such as diagnosing patients and managing natural conversations.

### Novel Approach: Dual-stage Mixed Fine-tuning (DMT)

We introduced **Dual-stage Mixed Fine-tuning (DMT)**, a novel SFT strategy that carefully composes fine-tuning data to enable the acquisition of multiple critical skills in a low-resource setup. 

### Key Features

- **Cost-Effective**: Leveraged QLoRA to minimize computational demands.
- **Performance**:
  - Strong results on medical benchmarks compared to similar-scale models.
  - Accurate, concise, and human-like responses in real-world patient interactions.

## Results

**Med-Nirvana 8B** demonstrates significant improvements in conversational healthcare tasks, validating the effectiveness of this fine-tuning methodology in a resource-constrained environment.

## Citation

If you use this work, please cite:

