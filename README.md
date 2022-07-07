# Hairpinanalyzer
Hairpinanalyzer V0.3
by Mathias Bader (mail@mathiasbader.de)

**Please note that this repository is no updated. Instead I kindly refer all users to [Mathias Bader](https://github.com/mathiasbader). You can find the most recent version of the  Haripin Analyzer here: [Hairpin Analyzer v.0.3.0](https://github.com/mathiasbader/hairpin-analyzer)**

The gold standard when analysing DNA methylation is bisulfite sequencing. Genomic DNA is treated with sodium bisulfite which causes the conversion of cytosine to uracil, whereas 5-methyl cytosine (5mC) remains unchanged. After subsequent PCR and sequencing cytosine will be represented as thymine and 5mC as cytosine. The comparison to the genomic reference sequence then allows to determine the level of 5mC at a given CpG position. However, conversion of cytosine requires denaturation of DNA, resulting in the separation of Watson and Crick strand. Therefore, it is only possible to preserve the information of one DNA strand in subsequent PCR and sequencing. To overcome this limitation Laird et al. developed Hairpin Bisulfite Sequencing. During the course of this technique, the DNA is fragmented using restriction enzymes followed by covalent connection of Watson and Crick strand by ligation of a short hairpin oligo nucleotide, preventing the physical separation of both DNA strands during bisulfite treatment.

The analysis of Hairpin Bisulfite data is more challenging compared to standard BS methods. Once the methylation information is extracted from the sequencing data, the double strand information has to be restored. For this purpose we developed a small python based script, the HairpinAnalyzer.

The Hairpinanalyzer was developed by Mathias Bader and Julia Arand from Saarland University. It takes the methylation information output of the BiQ Analyzer HT (http://biq-analyzer-ht.bioinf.mpi-inf.mpg.de/) and performs an in silico refolding of the DNA double strand. The data is stored as text files and pattern maps (png). The ‘documentation.txt’ gives a more detailed description of the Hairpinanalyzer. The experimental workflow is outlined in several publications:

Laird, C. D., Pleasant, N. D., Clark, A. D., Sneeden, J. L., Hassan, K. A., Manley, N. C., ... & Stöger, R. (2004). Hairpin-bisulfite PCR: assessing epigenetic methylation patterns on complementary strands of individual DNA molecules. Proceedings of the National Academy of Sciences, 101(1), 204-209.

Arand, J., Spieler, D., Karius, T., Branco, M. R., Meilinger, D., Meissner, A., ... & Walter, J. (2012). In vivo control of CpG and non-CpG DNA methylation by DNA methyltransferases. PLoS genetics, 8(6), e1002750.

Arand, J., Wossidlo, M., Lepikhov, K., Peat, J. R., Reik, W., & Walter, J. (2015). Selective impairment of methylation maintenance is the major cause of DNA methylation reprogramming in the early embryo. Epigenetics & chromatin, 8(1), 1.

Giehr, P., Kyriakopoulos, C., Ficz, G., Wolf, V., & Walter, J. (2016). The influence of hydroxylation on maintaining CpG methylation patterns: a hidden Markov model approach. PLoS computational biology, 12(5), e1004905.

Giehr, P., & Walter, J. (2018). Hairpin Bisulfite Sequencing: Synchronous Methylation Analysis on Complementary DNA Strands of Individual Chromosomes. In DNA Methylation Protocols (pp. 573-586). Humana Press, New York, NY.



For more information please contact:

Mathias Bader:  mail@mathiasbader.de

Pascal Giehr: 	pascalgiehr@googlemail.com

Jörn Walter:    j.walter@mx.uni-saarland.de

