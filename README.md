# 882Final
Computational Analysis of Plant Cell-Wall Degrading using AlphaFold3

## Overview
This project uses AlphaFold3 (AF3) to predict protein–protein interactions between the RIXI protein and a set of xylanase enzymes. The goal is to evaluate binding interactions using the inter-protein TM-score (ipTM) and identify key residues involved in binding.

---

## Project Goals
- Predict RIXI–xylanase binding interactions
- Identify high-confidence binding pairs
- Evaluate the effect of RIXI mutations on binding (completed using RfDiffusion3) 
- Generate ipTM scores for comparison across sequences

---

## Workflow

### 1. Generate AF3 Input Files
Xylanase sequences are paired with the RIXI sequence to create JSON input files for AlphaFold3.

### 2. Run AlphaFold3
Each sequence pair is processed to:
- Generate MSAs (multiple sequence alignments)
- Perform structure prediction
- Model protein–protein complexes

### 3. Extract ipTM Scores
For each completed prediction, the ipTM score is extracted and saved for analysis.

---
## Computational Challenges
-AF3 needs to be run on GPU node
-Long runtimes
-Requires sufficient disk quota 
-Make sure model weights are sourced
