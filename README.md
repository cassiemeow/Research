# Research
Qualifying Exam Data Analysis

Issues need to be careful in the future:
1. When filtering out the 50 genes in PAM50 from our own data, sometimes we cannot select out all 50 of them because the pam50 reference data is not the most recently updated version. 
   Gene symbols can have different names, comparing to the symbol names we match to in database such as org.Hs.eg.db.
2. For normalization using method: Median of Ratios (the one that DESeq2 uses), geometric mean is calculated using "exp(rowMeans(log(Data)))" since ($\prod_n^{i-1}$)
