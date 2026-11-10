# CRC-RadioRec

### CT Radiomics-Based Prediction of Postoperative Recurrence in Stage II Colorectal Cancer

This repository provides supplementary materials for a retrospective study investigating the prediction of postoperative recurrence in patients with stage II colorectal cancer using computed tomography (CT) radiomics and clinicopathological information.

## Study Overview

The study included 263 patients with stage II colorectal cancer who underwent R0 resection at Tottori University Hospital, Japan. Postoperative recurrence was observed in 41 patients (15.6%).

A total of 107 radiomics features were extracted from preoperative contrast-enhanced CT images. After assessment of interobserver reproducibility and feature correlation, 26 features were retained for model development.

Three types of prediction models were evaluated:

- **Integrated model:** Radiomics and clinicopathological features
- **Radiomics-only model:** CT-derived radiomics features
- **Clinical-only model:** Clinicopathological variables

Candidate models were screened using stratified five-fold cross-validation. The top 10 candidates in each category were subsequently evaluated using five-fold cross-validation repeated 10 times.

## Key Findings

| Model | Classifier | Mean ROC-AUC ± SD |
|---|---|---|
| Integrated | SVM-RBF | 0.762 ± 0.089 |
| Radiomics-only | SVM-RBF | 0.704 ± 0.096 |
| Clinical-only | Logistic regression | 0.691 ± 0.101 |

The selected integrated model combined seven radiomics features with preoperative carcinoembryonic antigen (CEA) >5.0 ng/mL.

SHAP analysis identified preoperative CEA as the largest contributor to model predictions.

These findings suggest that CT radiomics may complement clinical information in postoperative recurrence risk assessment. However, the models were developed and selected using the same single-center cohort, and independent validation is required.

## Repository Contents

**`Supplementary_Tables.xlsx`**

This Excel workbook contains eight supplementary tables accompanying the manuscript.

| Table | Description |
|---|---|
| S1 | Radiomics feature selection and interobserver reproducibility |
| S2 | Integrated model candidates and cross-validation results |
| S3 | Radiomics-only model candidates and cross-validation results |
| S4 | Clinical-only model candidates and cross-validation results |
| S5 | Performance comparison with all-variable models |
| S6 | Individual predictor discrimination |
| S7 | Additional evaluation in patients without preoperative treatment |
| S8 | Machine learning classifier settings |

## Data Availability

The supplementary workbook provides feature-level summaries, model configurations, and evaluation results.

Patient-level clinical data and original CT images are not included in this repository.

## Citation

**Iwata H, et al.** CT radiomics-based prediction of postoperative recurrence in stage II colorectal cancer.

*Manuscript in preparation.*

The complete bibliographic information and DOI will be added following publication.

## Contact

**Hiroaki Iwata**

Department of Biological Regulation  
Faculty of Medicine, Tottori University  
Yonago, Japan

Email: iwata.hiroaki@tottori-u.ac.jp

## License

Reuse conditions for the supplementary materials have not yet been specified.
