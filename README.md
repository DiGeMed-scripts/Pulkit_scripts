# GREP (Gut-microbiome REporting Pipeline)

## 🧬 Summary

This repository contains a fully automated Snakemake pipeline for gut microbiome analysis.

---

### 🔄 Clone This Repository

```bash
git clone --branch gut_microbiome_automation --single-branch https://github.com/DiGeMed-scripts/Pulkit_scripts.git
cd Pulkit_scripts
```

## 🛠️ Installation Guide

### 1. Install Miniconda (if not already installed)

Follow the official instructions: https://docs.conda.io/en/latest/miniconda.html

Or use this command (Linux):

```bash
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
```
```bash
bash Miniconda3-latest-Linux-x86_64.sh
```
Create New conda environment using given yml file
```bash
conda env create -f envs/gut_snakemake_env.yml
```
Activate the new environment
```bash
conda activate gut_microbiome_env
```
Run Snakemake pipeline
```bash
snakemake --cores all --use-conda all
```