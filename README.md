# 🧬 KRAS Mutation Context and Tumor Immune Programs in Lung Adenocarcinoma  
### TCGA Transcriptomic Analysis

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Status](https://img.shields.io/badge/Project-Completed-success)
![Dataset](https://img.shields.io/badge/Data-TCGA_LUAD-orange)
![Focus](https://img.shields.io/badge/Field-Cancer_Immunogenomics-red)

---

## 🔬 Research Motivation

This project was inspired by the study:

**“Kras G12C– and G12D–driven lung cancers differ in oncogenic potency, immunogenicity, and relapse after Kras inhibition in mouse models”**  
(*Science Translational Medicine*)

The study demonstrated that different KRAS mutation subtypes produce distinct immune phenotypes in mouse lung cancer models.

This raised a translational question:

> Do similar immune differences exist in **human lung adenocarcinoma**, and if so, are they driven by KRAS mutation subtype itself or by broader genomic mutation context?

To investigate this, I performed a structured computational analysis using publicly available TCGA mutation and RNA-seq datasets.

---

## 🎯 Project Objectives

- Evaluate whether KRAS mutation subtype influences tumor immune transcription  
- Determine whether major co-mutations (TP53, STK11, KEAP1) better explain immune differences  
- Identify immune genes and transcriptional programs associated with each mutation context  

---

## 🧪 Analysis Workflow

### **Week 1 — KRAS subtype comparison**

- Stratified tumors by KRAS mutation subtype  
- Computed immune cytotoxic gene signatures  
- Observed only modest immune differences between subtypes  

This suggested subtype alone may not explain immune variation in human tumors.

---

### **Week 2 — Co-mutation context analysis**

- Stratified KRAS tumors by major co-mutations:
  - TP53  
  - STK11  
  - KEAP1  

- Compared immune transcriptional activity across groups  

This revealed strong immune differences associated with mutation context.

---

### **Week 3 — Immune driver and pathway analysis**

- Identified immune-related genes enriched in mutation contexts  
- Detected elevated expression of:

  - interferon-stimulated genes  
  - T-cell recruitment chemokines  
  - antigen presentation genes  
  - immune checkpoint ligands  

- Computed pathway-level immune activity scores  

- Confirmed statistically significant differences using **Kruskal–Wallis testing (p < 10⁻⁶)**.

---

## 🧠 Key Biological Findings

✔ KRAS mutation subtype alone shows limited immune transcriptional differences in human LUAD  

✔ Co-mutation context strongly influences tumor immune programs  

✔ **KRAS+TP53 tumors** show coordinated activation of:

- interferon signaling  
- chemokine recruitment  
- antigen presentation  
- immune checkpoint expression  

✔ **KRAS+STK11 and KRAS+KEAP1 tumors** show comparatively reduced immune transcriptional activity  

---

## 📓 View Analysis Notebooks Online (No Setup Needed)

You can open the full analysis notebooks directly in your browser:

- Week 1 — KRAS subtype immune analysis  
https://nbviewer.org/github/SiyaSingh15/KRAS-immune-tcga/blob/main/notebooks/01_KRAS_subtype_analysis.ipynb  

- Week 2 — KRAS co-mutation immune context  
https://nbviewer.org/github/SiyaSingh15/KRAS-immune-tcga/blob/main/notebooks/02_KRAS_comutation_analysis.ipynb

- Week 3 — Immune driver gene and pathway analysis  
https://nbviewer.org/github/SiyaSingh15/KRAS-immune-tcga/blob/main/notebooks/03_immune_driver_analysis.ipynb

---

## 📊 Example Outputs

This repository includes:

- Immune pathway activity bar plots  
- Gene-level immune heatmaps  
- PCA visualization of tumor immune transcription  

(All generated from TCGA RNA-seq data.)

---

## ⚠️ Limitations

- TCGA RNA-seq represents bulk tumor tissue rather than single-cell resolution  
- Clinical covariates such as smoking history and tumor purity were not modeled  
- Results represent transcriptomic associations rather than causal mechanisms

---

## 💾 Dataset

- **TCGA Lung Adenocarcinoma (LUAD)**
- Mutation and RNA expression downloaded via UCSC Xena  

Raw files are not included due to size restrictions.

See: data/README.txt


for download instructions.

---

## 🛠 Tools Used

- Python  
- Pandas  
- NumPy  
- Seaborn  
- Scikit-learn  
- SciPy  

---

## 🛠 Tools Used

- Python  
- Pandas  
- NumPy  
- Seaborn  
- Scikit-learn  
- SciPy  

---

## 📂 Repository Structure

*notebooks/* → stepwise analysis notebooks

*figures/* → generated plots and visualizations

*data/* → instructions for downloading TCGA datasets


---

## ⚠️ Disclaimer

This is an exploratory transcriptomic analysis intended to investigate mutation-specific immune transcriptional patterns in publicly available cancer genomics datasets.  
Findings represent computational associations and not causal experimental validation.

