# RNA-Seq Analysis Project: SIRS vs Severe Sepsis

## Project Overview
This project investigates the differential gene expression between **Systemic Inflammatory Response Syndrome (SIRS)** and **Severe Sepsis** using RNA-Seq data. The goal is to identify genes and pathways that are uniquely upregulated or downregulated in Severe Sepsis compared to SIRS, providing insights into the biological mechanisms underlying these conditions.

## Hypothesis
Severe Sepsis samples are hypothesized to have a higher association with upregulated platelet aggregation genes compared to SIRS samples. Additionally, a downregulation of genes associated with cell viability and B lymphocyte activation is expected in Severe Sepsis.

## Methodology
### Data Processing
1. **Pre-alignment Quality Control:**
   - Evaluated read quality and distribution across samples.
2. **Alignment:**
   - Reads were aligned to the reference genome using **TopHat2**, and alignment metrics were analyzed.
3. **Gene Expression Analysis:**
   - Calculated Fragments Per Kilobase of transcript per Million mapped reads (FPKM) for quantifying gene expression.

### Analytical Approaches
- **Principal Component Analysis (PCA):**
  - Used to identify variance and clustering among samples.
- **Heatmaps and Dendrograms:**
  - Visualized patterns of gene expression.
- **Pathway Analysis:**
  - Conducted using Ingenuity Pathway Analysis (IPA) to highlight biological pathways impacted in Severe Sepsis.

### Findings
1. **Upregulated Genes:**
   - Genes associated with platelet aggregation were significantly upregulated in Severe Sepsis samples.
   - Early-stage Severe Sepsis demonstrated increased thrombocytosis.
2. **Downregulated Genes:**
   - Downregulation of B lymphocyte-associated genes, indicating lymphopenia.
   - Evidence of immune suppression, potentially increasing morbidity and mortality in sepsis patients.

### Conclusion
The study reveals significant differences in the gene expression profiles of Severe Sepsis and SIRS, supporting the hypothesis. Platelet aggregation and lymphocyte suppression are critical pathways in Severe Sepsis.

## Future Directions
- Improve sample alignment rates to ensure robust data analysis.
- Investigate sepsis-related thrombocytopenia and thrombocytosis in greater detail.
- Explore the immunosuppressive effects of sepsis, particularly lymphopenia, in larger datasets.

## File Descriptions
1. **RNA_seq_project.R**:
   - Contains the R script used for data processing, visualization, and statistical analysis.
2. **Presentation_Final.pptx**:
   - Summarizes the project's findings, methodology, and key conclusions.

## References
1. Tsalik, E. L., Langley, R. J., Dinwiddie, D. L., Miller, N. A., Yoo, B., van Velkinburgh, J. C., Smith, L. D., Thiffault, I., Jaehne, A. K., Valente, A. M., Henao, R., Yuan, X., Glickman, S. W., Rice, B. J., McClain, M. T., Carin, L., Corey, G. R., Ginsburg, G. S., Cairns, C. B., … Kingsmore, S. F. (2014). An integrated transcriptome and expressed variant analysis of sepsis survival and death. Genome Medicine, 6(11). https://doi.org/10.1186/s13073-014-0111-5 
2. NCI Dictionary of Cancer terms. National Cancer Institute. (n.d.). Retrieved November 30, 2021, from https://www.cancer.gov/publications/dictionaries/cancer-terms/def/sirs. 
3. Chakraborty, R. K., & Burns, B. (2021). Systemic Inflammatory Response Syndrome. In Statpearls. essay, StatPearls Publishing. 
4. Centers for Disease Control and Prevention. (2021, August 17). What is sepsis? Centers for Disease Control and Prevention. Retrieved November 30, 2021, from https://www.cdc.gov/sepsis/what-is-sepsis.html. 
5. Sepsis Alliance. (2021, August 4). What is sepsis. Sepsis Alliance. Retrieved November 30, 2021, from https://www.sepsis.org/sepsis-basics/what-is-sepsis/. 
6. Mayo Foundation for Medical Education and Research. (2021, January 19). Sepsis. Mayo Clinic. Retrieved November 30, 2021, from https://www.mayoclinic.org/diseases-conditions/sepsis/symptoms-causes/syc-20351214. 
7. Severe sepsis. Sepsis Alliance. (2021, February 21). Retrieved November 30, 2021, from https://www.sepsis.org/sepsis-basics/what-is-sepsis/severe-sepsis/. 
8. 24, N. H. S. (2021, November 1). Septic shock symptoms and treatment. Illnesses & conditions | NHS inform. Retrieved November 30, 2021, from https://www.nhsinform.scot/illnesses-and-conditions/blood-and-lymph/septic-shock. 
9. U.S. National Library of Medicine. (2015, January 1). Geo accession viewer. National Center for Biotechnology Information. Retrieved November 30, 2021, from https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE63042. 
10. Vardon-Bounes, F., Ruiz, S., Gratacap, M.-P., Garcia, C., Payrastre, B., & Minville, V. (2019). Platelets are critical key players in sepsis. International Journal of Molecular Sciences, 20(14), 3494. https://doi.org/10.3390/ijms20143494 
11. Sheikh Motahar Vahedi, H., Bagheri, A., Jahanshir, A., Seyedhosseini, J., & Vahidi, E. (2019). Association of Lymphopenia with Short Term Outcomes of Sepsis Patients; a Brief Report. Archives of academic emergency medicine, 7(1), e14.
12. Bakey, S., Karamanos, E., Louwers, L., Kolbe, N., Killu, K., Horst, H., Coba, V., & Rivers, E. (2013). Thrombocytosis versus Thrombocytopenia as Risk Factor for Increased Mortality in Sepsis. Critical Care Medicine, 41. https://doi.org/10.1097/01.ccm.0000440283.47246.33
