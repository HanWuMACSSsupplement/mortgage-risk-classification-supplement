# Online Supplement

## Paper

**From Prediction to Risk Classification: Temporal Transport and Model-Induced Reclassification in Mortgage Assessment**

This repository provides the Online Supplement accompanying the paper.

The study follows mortgage-risk assessment through four linked stages:

1. predictive discrimination
2. historical probability calibration
3. classification under a common illustrative loss rule
4. model-induced loan-level reclassification

The empirical analysis uses purchased/eligible Freddie Mac mortgages and compares Logistic Regression, Random Forest, and XGBoost in an out-of-time design.

## Full Supplement

[**Open the full Online Supplement**](./Online_Supplement.pdf) · [Detailed navigation guide](./SUPPLEMENT_GUIDE.md)

The Supplement contains detailed evidence on data construction, temporal model selection, calibration, decision sensitivity, model-induced reclassification, disagreement-direction analysis, robustness, and reproducibility/provenance.

## Main findings documented in the Supplement

- Flexible-model discrimination gains are metric-dependent.
- Historical isotonic calibration worsens probability quality for all three primary models in the 2023 cohort.
- Under the common illustrative 5:1 FN:FP loss ratio, all three primary model-based costs exceed the all-non-risky benchmark.
- The benchmark relation persists across R1–R7.
- Logistic Regression and XGBoost disagree on 12.06% of mortgages in the primary 2023 cohort.
- Reclassification is sensitive to population and timing assumptions, especially R3 and R7.

## Recommended reading paths

### Prediction and calibration

Start with **S.A, Tables S1–S2** for predictors, temporal selection, and historical isotonic estimation. Continue to **Appendix Figure A1** and **S.B, Table S3 / Figure S1** for raw ROC AUC / AP and raw-versus-calibrated probability quality in 2020 and 2023.

### Decision analysis

Read **Appendix Figure A2** and **S.C, Table S4** for the common illustrative 5:1 FN:FP rule, its all-non-risky benchmark, and alternative loss ratios. **Table S5** separates raw-probability sensitivity from validation-optimal thresholds transported unchanged to 2023.

### Model-induced reclassification

Use **S.D, Tables S6–S7** for Logistic–XGBoost disagreement directions and mortgage-characteristic profiles. **Table S8** reports adjusted directional associations; **S.F** explains the Firth fallback and numerical estimation.

### Robustness

Begin with **Appendix Table A2**, then **S.E, Tables S9–S10 / Figure S3** for R1–R7. Pay particular attention to R3's remaining-on-book population and R7's First Payment Date timing proxy. The [guide](./SUPPLEMENT_GUIDE.md) provides verified PDF starting pages.

## Data

The analysis uses the Freddie Mac Single-Family Loan-Level Dataset.

The source Freddie Mac data are not redistributed in this repository. Readers should obtain the dataset from Freddie Mac using the official documentation cited in the paper and Supplement, including the [Release 47 General User Guide](https://www.freddiemac.com/fmac-resources/research/pdf/general_user_guide_july_2026.pdf).

## Version

Version: UChicago MACSS writing-sample supplement  
Date: 6 October 2026

SHA-256 of `Online_Supplement.pdf`:

```text
935c6223c355edb7411a5f135612c6f41da3a8a387907f5f485b5261d1395567
```
