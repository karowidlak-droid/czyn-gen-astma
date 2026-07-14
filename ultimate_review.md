# Ultimate Expert Panel Review: Pulmonology, Genetics, and Statistics

**Manuscript Title:** Genetic Factors Influencing Asthma Exacerbation Frequency: A Systematic Review of Candidate Gene Polymorphisms

As an interdisciplinary panel, we have reviewed the manuscript one final time. The authors have done a magnificent job integrating our previous feedback, covering T2-High/Low endotyping, Eurocentric PRS bias, IL-5 signaling dynamics, epistasis, and statistical limitations.

However, we have identified two final, critical issues regarding **Methodological Consistency** and **Data Synthesis Accuracy** that must be addressed before the manuscript is fully publication-ready.

## 1. Methodological Inconsistency: The 2015-2025 Search Limit vs. Included Citations
* **The Issue:** In the Methods section (Section 2.2 and Table S1), the authors explicitly state that the inclusion criteria and search strategy were strictly "restricted to studies published between 2015 and 2025" to capture the most current genomic insights. However, the manuscript cites older literature to substantiate the newly added pharmacogenes (e.g., *GLCCI1* from Tantisira et al., 2011, and *FCER2* from Koplin et al., 2013).
* **The Clinical/Statistical Problem:** From a systematic review standpoint, this is a major methodological protocol violation. You cannot state a strict 2015-2025 search limit and then include primary source data from 2011/2013 in the results.
* **Recommendation:** The authors must either:
   a) Explicitly amend the "Study Selection" or "Eligibility Criteria" section to state that while the primary search was restricted to 2015-2025, seminal pharmacogenomic validation studies for *FCER2* and *GLCCI1* were included *a priori* via manual secondary sourcing.
   b) Remove the 2011/2013 citations and replace them with more recent (2015+) replication cohorts demonstrating the same *FCER2*/*GLCCI1* exacerbation risks.

## 2. Incomplete Biological Modeling
* **The Issue:** The authors provide a beautifully constructed "Biological Model of Asthma Exacerbation Susceptibility" (Figure 1). However, the recently integrated findings regarding the IL-5 axis, and the critical pharmacogenes *FCER2* and *GLCCI1*, are entirely missing from this visual model.
* **The Clinical Problem:** A biological model is meant to synthesize the core findings of the paper. Since the text explicitly states *GLCCI1* and *FCER2* govern steroid response, and *IL5* governs Th2 inflammation, their omission from the diagram leaves the visual synthesis incomplete.
* **Recommendation:** Update Figure 1 (the TikZ `tikzpicture`) to include *FCER2* and *GLCCI1* in the "Steroid Response & Pharmacogenetics" block, and include *IL5*/*IL5RA* in the "Th2 Inflammation & Cytokine Signaling" block.

## Summary
Addressing the methodological time-frame discrepancy and updating the visual biological model to reflect the complete gene set will finalize this manuscript for peer-reviewed publication.
