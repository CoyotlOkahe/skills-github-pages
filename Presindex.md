
---
layout: page
title: "Automated Cytometric Gating with Human-Level Performance (UNITO)"
---

## Paper
- *Automated cytometric gating with human-level performance using bivariate segmentation*
- **Journal:** Nature Communications (2025)
- **Link:** https://www.nature.com/articles/s41467-025-56622-2

---

## Slide Plan (40-minute Journal Club)

### 1. Title & Objectives (2 min)
- Paper title, authors, journal
- Why automated gating matters in flow cytometry
- Learning objectives

### 2. Background: Manual Gating & Its Limitations (4 min)
- Hierarchical bivariate gating in flow vs mass cytometry
- Technical & biological variability
- Pre-gating challenges (debris, doublets, artifacts)

### 3. Existing Automated Approaches (4 min)
- Density-based gating (FlowDensity)
- Unsupervised clustering (FlowSOM)
- Supervised ML/DL (DeepCyTOF, logistic regression)
- Key gaps vs human gating

### 4. Conceptual Idea Behind UNITO (3 min)
- Reframing gating as image segmentation
- Why bivariate density maps match human reasoning
- Advantages of pixel-level prediction

### 5. UNITO Framework Overview (6 min)
- Input: Bivariate density plots
- Labels: Human-annotated masks
- Preprocessing steps
- ConvNet-based segmentation
- Convex hull post-processing

### 6. Hierarchical Gating Strategy (4 min)
- Cascading gates to mirror manual workflows
- Pre-gating → downstream phenotyping
- Interpretability benefits

### 7. Datasets & Experimental Design (3 min)
- Mass cytometry cohorts
- Flow cytometry cohort
- Manual consensus from multiple immunologists

### 8. Benchmarking & Comparators (4 min)
- Static gates
- FlowDensity, FlowSOM
- Logistic regression, DeepCyTOF
- PeacoQC (singlet gate only)

### 9. Performance Results (6 min)
- Correlation with human consensus
- Accuracy, precision, recall, F1
- Comparison vs individual human gators
- Key figures walkthrough

### 10. Generalization & Robustness (3 min)
- In-batch vs out-of-batch testing
- Cross-cohort performance

### 11. Strengths of the Approach (3 min)
- Human-level accuracy
- Handles pre-gating
- Interpretable contours
- Panel-agnostic learning

### 12. Limitations & Practical Considerations (3 min)
- Training data requirement
- Panel changes require retraining
- Computational considerations

### 13. Implications for Flow Cytometry Labs (3 min)
- Standardization across operators
- High-throughput studies
- QC and reproducibility

### 14. Discussion Questions (3 min)
- Would you trust automated pre-gating?
- How might this integrate into existing pipelines?
- Risks of learning human bias?

### 15. Take-Home Messages (2 min)
- Gating as segmentation is powerful
- UNITO matches expert performance
- Automation without losing interpretability

---

## Optional Appendix
- UNITO preprocessing details
- ConvNet architecture (high level)
- Full benchmark tables
- Supplementary figures

## Presenter Notes
- Designed for ~1–3 min per section
- Emphasize figures and workflow over equations
- Encourage critique of consensus ground truth

