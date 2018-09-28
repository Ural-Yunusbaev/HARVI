# GDI (Genomic Data Integrator)
# HARVDI (Haplotype, Ancestry & Risk Variant Data Integrator)

Python script to integrate  Beagle3 phased haplotypes, PCADMIX ancestry data, VEP, LOFTEE, CADD deleterious variants

### Usage

There are 2 ways to start GDI:

To integrate Beagle3 and PCADMIX files type
<pre>./gdi.py 22 individuals.list PathToBeagleFiles PathToPCADMIXFiles</pre>

To integrate Beagle3, PCADMIX, VEP and CADD files type
<pre>./gdi.py 22 individuals.list PathToBeagleFiles PathToPCADMIXFiles PathToVEPFiles PathToCADDFiles</pre>

were
22 - chromosomes number
individuals.list - individuals list


Test run using example files
<pre>./gdi.py 1 oneindividual.list IN IN IN IN</pre>



### Output files examples

<pre>
<pre>

head OUT/GS000010321-ASM.haps.anc.vep.cadd
#       GS000010321-ASM Posterior(PROXY_for_WEA, PROXY_for_EA)
#Chrom  Pos     Hap1    Hap2    Hap1Anc1        Hap1Anc2        Hap1Anc3        Hap2Anc1        Hap2Anc2        Hap2Anc3        Hap1Gene        Hap1Feature     Hap1Consequence Hap1Canonical     Hap1_LoF        Hap1_Phred      Hap1_Source     Hap2Gene        Hap2Feature     Hap2Consequence Hap2Canonical   Hap2_LoF        Hap2_Phred      Hap2_Source
1       567697  A       A       -       -       -       -       -       -       ENSG00000237973 ENST00000414273 non_coding_transcript_exon_variant      YES     -       9.452   VCENSG00000237973 ENST00000414273 non_coding_transcript_exon_variant      YES     -       9.452   VC
1       567697  A       A       -       -       -       -       -       -       ENSG00000198744 ENST00000416718 upstream_gene_variant   YES     -       9.452   VC      ENSG00000198744   ENST00000416718 upstream_gene_variant   YES     -       9.452   VC
1       567697  A       A       -       -       -       -       -       -       ENSG00000225972 ENST00000416931 downstream_gene_variant YES     -       9.452   VC      ENSG00000225972   ENST00000416931 downstream_gene_variant YES     -       9.452   VC
1       567697  A       A       -       -       -       -       -       -       ENSG00000229344 ENST00000427426 upstream_gene_variant   YES     -       9.452   VC      ENSG00000229344   ENST00000427426 upstream_gene_variant   YES     -       9.452   VC
</pre>

<pre>

head OUT/GS000010321-ASM.haps.anc
#       GS000010321-ASM Posterior(PROXY_for_WEA, PROXY_for_EA)
#Chrom  Pos     Hap1    Hap2    Hap1Anc1        Hap1Anc2        Hap1Anc3        Hap2Anc1        Hap2Anc2        Hap2Anc3
1       567697  A       A       -       -       -       -       -       -
1       568201  C       C       -       -       -       -       -       -
1       568256  T       T       0.00507307      0.994927        -       0.00626922      0.993731        -
1       568361  C       C       0.00507307      0.994927        -       0.00626922      0.993731        -
1       752721  A       G       -       -       -       -       -       -
1       755274  T       C       -       -       -       -       -       -
1       756781  A       G       -       -       -       -       -       -
1       757103  T       C       0.00149201      0.998508        -       0.00219325      0.997807        -
</pre>

 File names format:<br>
 individual_id.suffix.chromosome<br>
 Examles:<br>
 PathToBeagleFiles/GS000010321-ASM.bgl.1<br>
 PathToVEPFiles/GS000010321-ASM.vep.1<br>
 PathToCADDFiles/GS000010321-ASM.cadd.1<br>

 File names format:<br>
 individual_id.suffix.chromosome.haplotype<br>
 PathToPCADMIXFiles/individual_id.pcadmix.1.1<br>
 PathToPCADMIXFiles/individual_id.pcadmix.1.2<br>
 Examles:<br>
 PathToPCADMIXFiles/GS000010321-ASM.pcadmix.1.1<br>
 PathToPCADMIXFiles/GS000010321-ASM.pcadmix.1.2<br>


### Contact
Ural Yunusbaev<br>
uralub@gmail.com<br>
