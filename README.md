# -Searching-for-Mutations-Leading-to-Isoniazid-Resistance-in-Tuberculosis

## Project overview

Tuberculosis (TB) remains a global health concern, and the emergence of drug-resistant strains poses a significant challenge to effective treatment. Isoniazid is a key first-line drug used in the treatment of TB, and resistance to this drug can compromise the success of therapy.
This project aims to identify and characterise genetic mutations associated with isoniazid resistance in _Mycobacterium tuberculosis_, the causative agent of Tuberculosis.

## Project method
The Sequence reads were downloaded and trimmed using **Sickle** (as a form of quality control). The trimmed reads were mapped or aligned to a Reference genome using **BWA-Burrows-wheeler Aligner** and the information was stored in a SAM file. After mapping, the SAM files were converted to BAM files and the BAM files were sorted. 
VCF tools such as **mpileup** command was used to generate a coverage information for all the bases and the variance was called up using **bcftools** and then finally a post vcf analysis and Variant annotation was performed using **SnpEff**. The Variant calling algorithm applied; basically calls variance, identifies these variants and store them in a file called Variant call format file (VCF). The VCF (Variant call format) file generated stores variants present in the data. SnpEff is used to annotate variants by providing functional information about them


## Interpretation/Discussion
  katG mutations are prevalent in isoniazid resistance. Across all samples; IGV visualisation of mutations in katG sequences (Position: 2153889 - 2156111) and IGV browser gives colours to interesting events. Variants that affect a gene's function are the most harmful and detrimental, yet they can occur anywhere along the genome sequence. A variation or mutation that impacts the gene regulatory region has the potential to repress, inhibit, or activate or deactivate a gene.
At Position: 2153889 – 2156111; Sample 1,3 and 4 showed no variants, While Variants were detected in Sample 2, 5,6,7,8,9, and 10, particularly homozygous variants, where NC_000962.3 is the reference sequence in Genbank
For Sample 2 and Sample 5; The variant NC_000962.3:c.944G>C p.(Ser315Thr), indicating a single nucleotide polymorphism(SNP), where a guanine (G) nucleotide at position 944 has been replaced by a cytosine (C) nucleotide. The p.(Ser315Thr) indicates the amino acid change caused by the SNP, In this case, a serine (Ser) amino acid at position 315 has been replaced by a threonine (Thr) amino acid. This is a missense mutation, as it results in a change in a single amino acid , causing Isoniazid resistance.
Sample 6, 7,8,9 and 10 produced two variants; The variant NC_000962.3:c.944G>C p.(Ser315Thr) and The variant NC_000962.3:c.723C>G p.(Pro241Pro). The former being a missense variation and the Latter being a synonymous variant (the variation doesn’t alter the encoded amino acid).
The mutation occurs at a coding region causing a structural and conformational change and preventing it from binding to the target resulting hence resulting in Isoniazid deactivation and resistance. [Larsen et al, 2002].  

Isoniazid resistance in Mycobacterium tuberculosis can arise from mutations in various genes and alterations in biological pathways. Understanding these pathways is crucial for developing new strategies to combat drug-resistant Tuberculosis. Some key pathways associated with Isoniazid resistance include; Pharamacokinetics/Pharmacodynamics factors, Drug efflux systems, Mycobacterial Cell wall, Drug misuse, generation or use of alternative biochemical pathways.



## Conclusion
Mutations were identified in 7 samples; with 5 samples having two variants. Isoniazid resistance is due to the mutation of katG gene --Ser315-Thr--. These mutations reduce its activity, making it difficult to treat Tuberculosis
