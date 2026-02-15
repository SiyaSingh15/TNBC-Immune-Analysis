# **RESULTS**

### 1. TNBC tumors exhibit significantly higher immune activation

Using a curated immune gene panel (including CD8A, GZMB, CXCL9, CXCL10, LAG3, PDCD10/11, IFNGR1/2, PRF1, ICOS, etc.), we computed an immune activation score for each tumor as the mean standardized expression of these genes.

Comparison between TNBC and non-TNBC tumors revealed:

TNBC samples had visibly higher immune scores.

The median immune score for TNBC was above zero, whereas non-TNBC tumors were predominantly below zero.

A Mann–Whitney U test confirmed this difference to be highly significant:
𝑝 = 1.05 × 10^−8

This indicates that the observed immune activation difference is extremely unlikely to be due to chance.

Biologically, this supports the established observation that TNBC tumors often display increased immune infiltration and inflammatory signaling compared to hormone receptor–positive subtypes.

### 2. Tumors exhibit substantial immune heterogeneity

Hierarchical clustering of immune gene expression revealed clear variability across samples:

* A subset of tumors showed coordinated upregulation of cytotoxic T-cell and interferon-related genes.
* Other tumors displayed uniformly low immune gene expression.

Importantly:

* While many immune-high tumors were TNBC, not all TNBC tumors were immune-high.
* Some non-TNBC tumors also exhibited strong immune activation.

This demonstrates that immune activity is not binary across subtype categories but instead reflects biological heterogeneity within breast cancer.

### 3. Unsupervised clustering reveals intrinsic immune subtypes

K-means clustering (k=2) performed solely on immune gene expression identified two distinct tumor groups:

* Immune-High cluster
* Immune-Low cluster

The mean immune scores of the clusters showed strong separation:

* Cluster 1: High immune activation (~0.97)
* Cluster 0: Low immune activation (~-0.28)

Cross-tabulation showed enrichment of TNBC within the immune-high group, though both subtypes were represented in both clusters.

This demonstrates that immune-based tumor subtypes can be discovered without prior subtype labels, highlighting the power of unsupervised genomic analysis.

### 4. Immune gene expression predicts TNBC status

A logistic regression classifier was trained using immune gene expression features.

Model performance:

* Accuracy: 83%
* TNBC precision: 0.67
* Non-TNBC precision: 0.89
* ROC curve showed strong discrimination (AUC visually ~0.8+)

This indicates that immune gene expression contains substantial predictive information for TNBC classification.

However, imperfect TNBC recall confirms that immune activation alone does not fully define subtype identity, reflecting TNBC biological diversity.

### 5. Key immune genes driving TNBC prediction

Feature importance analysis revealed that genes such as:

* PDCD10
* GZMB
* CXCL10
* CXCL9
* LAG3

contributed strongly to TNBC classification.

These genes are associated with:

* Cytotoxic T-cell activity
* Interferon signaling
* Immune checkpoint pathways

This reinforces the biological plausibility of the model.


Together, these findings highlight that immune contexture is a major dimension of breast cancer biology and can be quantified effectively using gene expression–based approaches