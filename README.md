# GDI (Genomic Data Integrator)
Python script to integrate  Beagle3 phased haplotypes, PCADMIX ancestry data, VEP, LOFTEE, CADD deleterious variants

There are 2 ways to start:

1) type

./gdi.py 22 individuals.list PathToBeagleFiles PathToPCADMIXFiles 

to integrate Beagle3 and PCADMIX files;

2) type

./gdi.py 22 individuals.list PathToBeagleFiles PathToPCADMIXFiles PathToVEPFiles PathToCADDFiles

to integrate Beagle3, PCADMIX, VEP and CADD files,

were

22 - chromosomes number

individuals.list - individuals list


Type
./gdi.py 1 oneindividual.list IN IN IN IN
to run using example files.

 File names format:
 individual_id.suffix.chromosome
 Examles:
 PathToBeagleFiles/GS000010321-ASM.bgl.1
 PathToVEPFiles/GS000010321-ASM.vep.1
 PathToCADDFiles/GS000010321-ASM.cadd.1

 File names format:
 individual_id.suffix.chromosome.haplotype
 PathToPCADMIXFiles/individual_id.pcadmix.1.1
 PathToPCADMIXFiles/individual_id.pcadmix.1.2
 Examles:
 PathToPCADMIXFiles/GS000010321-ASM.pcadmix.1.1
 PathToPCADMIXFiles/GS000010321-ASM.pcadmix.1.2
