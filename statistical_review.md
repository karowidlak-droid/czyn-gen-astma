# Statistical Review Report

**Manuscript Title:** Genetic Factors Influencing Asthma Exacerbation Frequency: A Systematic Review of Candidate Gene Polymorphisms

## 1. Candidate Gene Approach vs. GWAS Vulnerabilities ("Winner's Curse")
The manuscript relies heavily on the "candidate gene" approach for identifying associations. Statistically, this methodology is notoriously prone to false positives (Type I error) and the "winner’s curse," where initial studies overestimate effect sizes. While the review mentions GWAS in the search strategy and includes some GWAS data, it structurally privileges candidate genes without enforcing strict genome-wide significance thresholds ($p < 5 \times 10^{-8}$) for all cited variants. A more robust statistical approach would explicitly stratify evidence by the statistical threshold met (e.g., candidate gene nominal $p < 0.05$ vs. true GWAS significance).

## 2. Issues with Meta-Analytic Pooling and Heterogeneity
The manuscript attempts a meta-analysis (Figure 2) for the *ADRB2* rs1042713 variant.
* **Heterogeneity Metric:** The text claims "minimal heterogeneity ($I^2 = 0\%$)", but given the small number of studies pooled (only 3), the $I^2$ statistic is heavily underpowered to detect true clinical or methodological heterogeneity. A $p$-value for Cochran's Q should be explicitly reported alongside the $I^2$ value.
* **Random vs. Fixed Effects:** The Forest plot indicates a "Random Effects" model was used. With only 3 studies, estimating the between-study variance ($\tau^2$) in a random-effects model is highly imprecise. A fixed-effect model (or a Bayesian approach with informative priors on $\tau^2$) is generally recommended when $k < 5$, or the limitations of the random-effects estimate must be explicitly acknowledged.

## 3. Multiple Testing and Pleiotropy
When reviewing associations across 13 different genes and numerous SNPs, there is a profound multiple testing burden. The review rarely discusses whether the primary source studies utilized appropriate multiple-testing corrections (e.g., Bonferroni, FDR, or Benjamini-Hochberg) for the number of SNPs tested within a given cohort. Uncorrected nominal $p$-values in candidate gene studies strongly inflate false discovery rates.

## 4. Evaluation of Publication Bias
The methodology section claims "Funnel plots and Egger's test" will be used for publication bias assessment. However, funnel plots and Egger's tests are statistically invalid and highly misleading when fewer than 10 studies are included in a meta-analysis. Given that the only meta-analysis presented contains 3 studies, these tools cannot be used to rule out publication bias. The review should acknowledge this significant limitation rather than presenting an "undetected" publication bias in the GRADE table as a definitive conclusion.

## 5. Confounding and Gene-Environment (GxE) Interactions
Asthma exacerbations are highly driven by environmental factors (viral infections, allergens, ICS adherence). The review appropriately notes that "retrospective electronic health record studies were noted to have a higher risk of bias regarding medication adherence control." However, statistically, if the base studies did not explicitly model Gene $\times$ Environment (GxE) interactions or adjust for ICS dose as a time-varying covariate, the marginal genetic effect sizes (Odds Ratios) reported in the summary tables are likely biased or confounded.

## 6. Predictive Modeling Claims
In the conclusions, the authors state: *"integrating these robust, exacerbation-specific genomic profiles into polygenic risk scores and routine clinical practice will be paramount in shifting the paradigm from managing asthma exacerbations to predicting and preventing them."*
From a statistical prediction standpoint, this is an overstatement. Single SNPs or small panels of candidate genes typically explain $< 5\%$ of the phenotypic variance ($R^2$) for complex traits. Without reporting the Area Under the Curve (AUC), C-statistic, or pseudo-$R^2$ of these Polygenic Risk Scores (PRS) in hold-out validation cohorts, claims of clinical predictive utility are statistically unsubstantiated.

## Recommendations for Improvement
1. **Explicitly separate** loci reaching strict genome-wide significance ($p < 5 \times 10^{-8}$) from those only reaching nominal candidate-gene significance.
2. **Revise the Meta-Analysis:** Acknowledge the extreme limitation of using a random-effects model and assessing $I^2$ with only $k=3$ studies.
3. **Remove claims of Egger's test/Funnel plots** for publication bias, as the study count is too low for mathematical validity.
4. **Temper predictive claims:** Clearly state the anticipated variance explained by these genetic models to provide readers with a realistic statistical perspective on clinical implementation.
