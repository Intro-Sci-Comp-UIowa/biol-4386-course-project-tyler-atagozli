# Title

Erives AJ, Fassler JS (2015) Metabolic and Chaperone Gene Loss Marks the Origin of Animals:
Evidence for Hsp104 and Hsp78 Chaperones Sharing Mitochondrial Enzymes as Clients. PLoS
ONE 10(2): e0117192. https://doi.org/10.1371/journal.pone.0117192

# Reference

[pdf](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4339202/)

# Introduction 

The authors of this paper were interested in seeing which genes were lost in the evolution of
animals. To do this they compared the genomes of closely related eukaryotes, such as yeast and
choanoflagellates, to animals and found that twenty-four genetic functions retained in lower order
eukaryotes but lost in animals. Most interestingly, they found two powerful molecular chaperones,
Hsp78 and Hsp104, were abruptly lost during the evolution of unicellular organisms to animals. It
is not clear why this occurred, but the authors suggest the loss of shared clients of Hsp78 and
Hsp104 played a role.

# Figure 

![Figure 1](https://www.ncbi.nlm.nih.gov/core/lw/2.0/html/tileshop_pmc/tileshop_pmc_inline.html?title=Click%20on%20image%20to%20zoom&p=PMC3&id=4339202_pone.0117192.g001.jpg)
**Twenty-five genetic functions undetectable in animals.**

# Figure 1 legend
(A) Heat map of twenty-seven genes (first twenty-seven rows with gene names) from the budding yeast S. cerevisiae (S. cer.) and their orthologs in related organisms with whole genome sequence assemblies and their closest matches in animals. Six of the twenty-seven yeast genes are the result of lineage-specific duplications in yeast (indicated by dark gray brackets, left of table), leaving twenty-four genetic functions either lost or not measurably conserved in metazoans. The heat map is based on the BLASTP expect values of the best match to the indicated yeast gene (see key, lower right of table). Species abbreviations: S. cer., Saccharomyces cerevisiae; S. pom., Schizosaccharomyces pombe; C. neo., Cryptococcus neoformans; P. gra., Puccinia graminis; B. den., Batrachochytrium dendrobatidis; C. owc., Capsaspora owczarzaki; M. bre., Monosiga brevicollis; S. ros., Salpingoeca rosetta; A. que., Amphimedon queenslandica; T. adh., Trichoplax adhaerens; M. lei., Mnemiopsis leidyi; N. vec., Nematostella vectensis; L. gig., Lottia gigantea; C. tel., Capitella teleta; H. rob., Helobdella robusta; D. mel., Drosophila melanogaster; and H. sap., Homo sapiens. Other abbreviations: Chytridio., Chytridiomycota; Placo., Placozoa; Ctenoph., Ctenophora; Ecdyso., Ecdysozoa; and Chor., Chordata. The last row is from an alternative screen for lost animal genes (see text) in which Amoebozoa PFAM domains that are absent in animals were identified (five genes already identified plus one new gene, PURB). (B) Close-up of the lost animal gene columns from panel A. This table shows either the taxonomic origin of a weak animal match, or the name of the gene if it is not directly related (i.e., not orthologous) to the named yeast gene (first column) for all matches with BLASTP expectation values < 1e-20. Most of the animal matches to the candidate lost genes correspond to lineage-specific horizontal gene transfers and/or environmental contaminants from unrelated (non-opisthokont) clades. Some matches correspond to non-orthologous genes such as ANKCLP (S2 Fig.) in the case of the eukaryotic clpB genes HSP78 and HSP104, or ACO1 in the case of LYS4 (Fig. 3). Only HIS2 might have been lost soon after early animal radiation based on the presence of a weak match in Trichoplax adhaerens. This gene is most similar to the version from Capsaspora and not to either of the two choanoflagellates, so it is of uncertain origin.

# My description of the Figure

Figure 1 of this paper uses computational methods to identify genes and genetic functions retained in fungi and choanoflagellates but lost in animals

# Materials and Methods

1. Generate a manageable gene list using Ensembl's BioMart query engine to iteratively identify orthologs present in fungi but absent in *Drosophila melanogaster* and *Homo sapiens*
2. There should be 802 genes now. Query the Joint Genome Institute's (JGI) BLASTP Sever (genome.jgi.doe.gov) with each yeast protein to identify fungal proteins which match with protein sequences from the choanoflagellate *M. brevicollis* with a BLASTP E-value of 1.0E-30 or lower
3. There should be 210 genes now. Use a threshold E-value of 1.0E-10 to remove yeast proteins that either had no matches or were not detectable for the colonial choanoflagellate S. rosetta and the filasterean C. owczarzaki.
4. Also remove those that have E-values in animals smaller (i.e., better) than any of the three listed non-animal holozoans (the choanoflagellates and filasterean)
5. For animals, use the sponge *Amphimedon queenslandica* (NCBI), the ctenophore *Mnemiopsis leidyi* (NHGRI), the placozoan *Trichoplax adhaerens* (NCBI), and the lophotrochozoans *Lottia gigantea*, *Capitella teleta*, and *Helobdella robusta*, all of which have complete genome sequence assemblies.
6. With these genomic comparisons, there should be twenty-seven yeast genes that are largely retained outside of animals in the analyzed genomes.
7. Six of these genes (TRR1/TRR2, LYS20/LYS21, and SCT1/GPT2) correspond to lineage-specific duplications in yeast (connected genes in Fig. 1). Thus, twenty-four genetic functions are definitively lost in animals or at least not retained at the same level of conservation as they are in non-metazoans

8. Make a heat map based on BLASTP expecr values of the best match to the indicated yeast gene  
9. Figure 1B should show either the taxonomic origin of a weak animal match, or the name of the gene if it is not directly related (i.e., not orthologous) to the named yeast gene (first column) for all matches with BLASTP expectation values < 1e-20.


