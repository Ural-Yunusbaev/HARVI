# GDI (Genomic Data Integrator)
Python script to integrate  Beagle3 phased haplotypes, PCADMIX ancestry data, VEP, LOFTEE, CADD deleterious variants

There are 2 ways to start:<br>
1) type<br>
./gdi.py 22 individuals.list PathToBeagleFiles PathToPCADMIXFiles<br>
to integrate Beagle3 and PCADMIX files;<br>
2) type<br>
./gdi.py 22 individuals.list PathToBeagleFiles PathToPCADMIXFiles PathToVEPFiles PathToCADDFiles<br>
to integrate Beagle3, PCADMIX, VEP and CADD files,<br>
were<br>
22 - chromosomes number<br>
individuals.list - individuals list<br>

Type<br>
./gdi.py 1 oneindividual.list IN IN IN IN<br>
to run using example files.<br>

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
