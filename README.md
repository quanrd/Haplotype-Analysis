# GDA
Genetic Data Analysis

This repository is a collection of programs developed for analysis of genetic data. While there are now a lot of new programs for genomewide association analysis (GWAS) they form the basic elemements.  These programs were in the Rockefeller list currently available from https://github.com/gaow/genetic-analysis-software
 
I have also converted some functionalities into R/gap available from CRAN (https://cran.r-project.org/).

###REFERENCES

**2LD**

Zhao, J. H. (2004). 2LD, GENECOUNTING and HAP: Computer programs for linkage disequilibrium analysis. Bioinformatics, 20, 1325-1326

Zapata C, Carollo C, Rodriguez S. (2001). Sampling variance and distribution of the D' measure of overall gametic disequlibrium between multiallelic loci. Annals of Human Genetics, 65, 395-406


**EH+**

Zhao, J. H., Curtis, D., Sham, P. C. (2000). Model-free analysis and permutation tests for allelic associations. Human Heredity, 50(2), 133-139


**FASTEH+**

Zhao, J. H., Sham, P. C. (2002). Faster allelic association analysis using unrelated subjects. Human Heredity, 53(1), 36-41


**GENECOUNTING**

Zhao, J. H, .Lissarrague, S., Essioux, L., Sham, P. C. (2002). GENECOUNTING: haplotype analysis with missing genotypes. Bioinformatics, 18(12), 1694-1695.

Zhao, J. H. (2004). 2LD, GENECOUNTING and HAP: Computer programs for linkage disequilibrium analysis. Bioinformatics, 20, 1325-1326 

**HAP**

Zhao, J. H. (2004). 2LD, GENECOUNTING and HAP: Computer programs for linkage disequilibrium analysis. Bioinformatics, 20, 1325-1326

### Additional note

**2LD**, **EH+**, **FASTEH+**, **GEECOUNTING((, **HAP** can be put in the same directory with call to the appropriate executables. **EH+**, **FASTEH+** and **GENECOUNTING** can also share the same parameter and data file. I have tested them extensively under Windows, Sun, Dec Alpha and Linux systems. A brief comparison is shown in the following table. Program **MCETDT** (Monte Carlo module for the Extended Transmission Disequilibrium Test) is distributed with **ETDT** and unavailable from this site. Note to enter MS-DOS under the default setup for Windows Visa, you need to run c:\windows\system32\cmd.exe first. 

Package name | Executable names| Documentation | Features | Limitations
-------------|-----------------|---------------|----------|------------
**2LD**| `2ld` | `2ld.doc`, `2ld.htm` |  D', SE(D'), Cramer's V for two multiallelic loci, r | Requires **LDSHELL** for many markers, does not show D' in graphics
**EH+** | `eh`, `ehplus`, `fehp`, `pm`, `pmplus` | `pm.doc`, `pm.stm` |  Model-free and permutation tests of allelic association. **EH** compatible and very easy to use. (having been the top paper in Hum Hered in 2005/6/7). | Slower than **FASTEH+** and **GENECOUNTING** but call **FASTEH+** for permutation tests from version 1.2
**FASTEH+** | `fpmp`,`fehp`,`pfehp` | `fpmp.doc` | Faster algorithm and likelihood-based LD measures | Does not handle missing data, less statistics than **EH+**
**GENECOUNTING**  | `gc`,`gcp`,`gcx`,`pgc` | `gc.txt` | Haplotype frequency estimation and reconstruction, flexible in missing data patterns and X chromosome data, haplotype-specific tests | Limited to about 15 SNPs and slow with multiple multiallelic loci with missing data
**HAP** |  `hap`,`mia` | `hap.txt` | Large number of SNPs and multiple imputations, missing data, multiallelic loci | Possibly sub-optimal solution
