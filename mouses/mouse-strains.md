<!-- TITLE: Mouse Strains -->

# B6
# NOD
# C3H
# NOD.uMT
# NOD.RAG-/-
# SLE123
# B6.IL15-/-
These mice are double knockouts for the IL15 (interleukin-15) gene, on a B6 background.

## Production
Mice of this genotype are true breeding.

## Genotyping
This protocol is also used to genotype the IL15 portion of the SAP-/- IL15-/- mice below.

### Primers
**IL15 F**: 5’ CAC TTC AGA GGC ATG TCG GT 3’ (20bp) - interleukin 15 isoform X1  
**IL15 R**: 5’ TAC AAG GGC TGT TCG TTG CT 3’ (20bp) - interleukin 15 isoform X1

### PCR Mix
Reagent | Amount (per rxn) | Stock Conc. | Final Conc.
--- | --- | --- | ---
IL15 F Primer | 1.5 ul | 10 uM | 0.6 uM
IL15 R Primer | 1.5 ul | 10 uM | 0.6 uM
Promega Green Mix | 12.5 ul | 2X | 1X
Nuclease-free water | 7.5 ul | - | -
DNA sample | 2.0 ul | - | -

### PCR protocol
Temperature (&deg;C) | Time (m:ss)
--- | ---
94 | 3:00
 - | start loop 35x
94 | 1:00
58 | 1:00
72 | 1:00
- | end loop
72 | 2:00
4 | &#x221e;

### Expected result
**Bands**:  
* wild-type: ~846 bp
* IL15-/-: no band
# B6.SAP-/-
These mice are double knockouts for the SAP (SLAM-associated protein) gene, on a B6 background.

## Production
We are not actively maintaining this strain.

This strain can be purchased from [Jackson, stock number 025754](https://www.jax.org/strain/025754).

## Genotyping
This protocol can only be used with [clean DNA](/mouses/genotyping) prepared using a kit like the [QIAGEN DNeasy Blood & Tissue kit](https://www.qiagen.com/us/shop/sample-technologies/dna/genomic-dna/dneasy-blood-and-tissue-kit/#orderinginformation). It will not work with DNA prepared from NaOH-digested tissue.

This protocol is also used to genotype the SAP portion of the SAP-/- IL15-/- mice below.

### Primers
**SAP F**: 5’ CTC TCT GCA TCC TTC TCA CAT 3’ (21bp) - SH2 domain-containing protein 1A  
**SAP R**: 5’ GCC AGA GGA CTT TTC AAC TGG 3’ (21bp) - SAP gene  
**PFred**: 5’ CAT GCC GTT TCA TAT GAT CCG GG 3’ (23bp) - ? i don’t know what this is, but it does something  

### PCR Mix
Reagent | Amount (per rxn) | Stock Conc. | Final Conc.
--- | --- | --- | ---
SAP F Primer | 1.5 ul | 10 uM | 0.6 uM
SAP R Primer | 1.5 ul | 10 uM | 0.6 uM
PFred Primer | 1.5 ul | 10 uM | 0.6 uM
Promega Green Mix | 12.5 ul | 2X | 1X
Nuclease-free water | 6.0 ul | - | -
DNA sample | 2.0 ul | - | -

### PCR protocol
Temperature (&deg;C) | Time (m:ss)
--- | ---
94 | 3:00
 - | start loop 35x
94 | 1:00
61 | 1:00
72 | 1:00
- | end loop
72 | 2:00
4 | &#x221e;

### Expected result
**Bands**:  
* wild-type: ~210 bp
* SAP-/-: ~375 bp

# Qa1-/-
These mice are double knockouts for the Qa-1 gene, on a B6 background.
# B6.VH125+/+
These mice have V<sub>H</sub>125 inserted into both copies of the genome, on a B6 background.

This mouse produces B-cells that produce anti-insulin antibodies.

This mouse has an anti-insulin gene (V<sub>H</sub>125) inserted, replacing the endogenous IgJ<sub>H</sub>3 allele. Because it is site-directed to the native IgJ<sub>H</sub>3, these B-cells are able to class switch and produce both IgM<sup>a</sup> and IgD<sup>a</sup> (as opposed to only IgMa in non-site-directed V<sub>H</sub>125Tg mice).

## Production
This strain is maintained by breeding B6.VH125+/+ mice with each other. 

It can also be achieved by breeding B6.VH125+/- mice with each other, then genotyping the pups with both protocols shown below to select the +/+ genotype.

## Genotyping VH125
This protocol confirms the presence of one *or* two copies of the VH125 allele. It does not differentiate between mice that are heterozygous and homozygous for VH125. To confirm homozygosity, the mice must also be genotyped using the Jh3 protocol below.

### Primers
**VH125 F**: 5’ CAG ATC CAG TTG GTG CAG TC 3’ (20bp) - VH125 gene  
**VH125 R**: 5’ CCA GAC ATC GAA GTA CCC CT 3’ (20bp) - wild-type Jh gene  

### PCR Mix
Reagent | Amount (per rxn) | Stock Conc. | Final Conc.
--- | --- | --- | ---
VH125 F Primer | 1.5 ul | 10 uM | 0.6 uM
VH125 R Primer | 1.5 ul | 10 uM | 0.6 uM
Promega Green Mix | 12.5 ul | 2X | 1X
Nuclease-free water | 7.5 ul | - | -
DNA sample | 2.0 ul | - | -

### PCR protocol
Temperature (&deg;C) | Time (m:ss)
--- | ---
94 | 3:00
 - | start loop 35x
94 | 1:00
58 | 1:00
72 | 1:00
- | end loop
72 | 2:00
4 | &#x221e;

### Expected result
**Bands**:  
* wild-type: no band
* VH125+/-: ~290 bp
* VH125+/+: ~290 bp

## Genotyping wild-type insertion site (Jh3)
This protocol confirms the presence of one *or* two copies of the wild-type allele present at the location of the VH125sd insert. A mouse that is VH125+/+ will not have a band for this primer set. 

### Primers
**Jh F**: 5’ CCT GGT TTG CTT ACT GG 3’ (17bp) - wild-type Jh3 gene  
**Jh R**: 5’ GTA GTC CAT AGC ATA GTA ATC AC 3’ (23bp) - wild-type Jh4 gene  

### PCR Mix
Reagent | Amount (per rxn) | Stock Conc. | Final Conc.
--- | --- | --- | ---
Jh F Primer | 1.5 ul | 10 uM | 0.6 uM
Jh R Primer | 1.5 ul | 10 uM | 0.6 uM
Promega Green Mix | 12.5 ul | 2X | 1X
Nuclease-free water | 7.5 ul | - | -
DNA sample | 2.0 ul | - | -

### PCR protocol
Temperature (&deg;C) | Time (m:ss)
--- | ---
94 | 3:00
 - | start loop 35x
94 | 1:00
50 | 1:00
72 | 1:00
- | end loop
72 | 2:00
4 | &#x221e;

### Expected result
**Bands**:  
* wild-type: ~600 bp
* VH125+/-: ~600 bp
* VH125+/+: no band

# B6.Vk125+/+
These mice have V<sub>k</sub>125 inserted into both copies of the genome, on a B6 background.

## Production
This strain is maintained by breeding B6.Vk125+/+ mice with each other. 

It can also be achieved by breeding B6.Vk125+/- mice with each other, then genotyping the pups with both protocols shown below to select the +/+ genotype.

## Genotyping Vk125
This protocol confirms the presence of one *or* two copies of the Vk125 allele. It does not differentiate between mice that are heterozygous and homozygous for Vk125. To confirm homozygosity, the mice must also be genotyped using the Jk1 protocol below.

### Primers
**Vk125 F**: 5’ TAT GAT CGG AAT TCC TCG AGT CTA GAG CGG 3’ (30bp)  
**Vk125 R**: 5’ GCT CCA GCT TGG TCC CAG CA 3’ (21bp)  

### PCR Mix
Reagent | Amount (per rxn) | Stock Conc. | Final Conc.
--- | --- | --- | ---
Vk125 F Primer | 1.5 ul | 10 uM | 0.6 uM
Vk125 R Primer | 1.5 ul | 10 uM | 0.6 uM
Promega Green Mix | 12.5 ul | 2X | 1X
Nuclease-free water | 7.5 ul | - | -
DNA sample | 2.0 ul | - | -

### PCR protocol
Temperature (&deg;C) | Time (m:ss)
--- | ---
94 | 3:00
 - | start loop 35x
94 | 1:00
59 | 1:00
72 | 1:00
- | end loop
72 | 2:00
4 | &#x221e;

### Expected result
**Bands**:  
* wild-type: no band
* Vk125+/- or Vk125+/+: ~900 bp

Bands at ~600bp and below may be present in all genotypes and can be ignored.

## Genotyping wild-type insertion site (Jk1)
This protocol confirms the presence of one *or* two copies of the wild-type allele present at the location of the VH125sd insert. A mouse that is VH125+/+ will not have a band for this primer set. 

### Primers
**Jk F**: 5’ AAT CAG CAG TTC TCT GTC AGA GAA GCC 3’ (27bp) - wild-type Jk1 gene  
**Jk R**: 5’ GGT TAG ACT TAG TGA ACA AGA GTT GAG AA 3’ (29bp) - wild-type Jk2/3 gene  

### PCR Mix
Reagent | Amount (per rxn) | Stock Conc. | Final Conc.
--- | --- | --- | ---
Jk F Primer | 1.5 ul | 10 uM | 0.6 uM
Jk R Primer | 1.5 ul | 10 uM | 0.6 uM
Promega Green Mix | 12.5 ul | 2X | 1X
Nuclease-free water | 7.5 ul | - | -
DNA sample | 2.0 ul | - | -

### PCR protocol
Temperature (&deg;C) | Time (m:ss)
--- | ---
94 | 3:00
 - | start loop 35x
94 | 1:00
53 | 1:00
72 | 1:00
- | end loop
72 | 2:00
4 | &#x221e;

### Expected result
**Bands**:  
* wild-type or Vk125+/-: ~600 bp
* Vk125+/+: no band

Bands at ~400bp and below may be present in all genotypes and can be ignored.
# B6.VH+/+Vk+/+
# NOD.VH125+/+
Ideally, these mice would have V<sub>H</sub>125 inserted into both copies of the genome, on a NOD background.

However, to date, we've been unable to produce homozygous-positive mice, and therefore are stuck with heterozygotes (VH125+/-).

## Genotyping
The genotyping protocol is the same as the the B6.VH125+/+ protocol above.
# NOD.Vk125+/+
These mice have V<sub>k</sub>125 inserted into both copies of the genome, on a NOD background.
## Genotyping
The genotyping protocol is the same as the the B6.Vk125+/+ protocol above.
# NOD.VH+/+Vk+/+
# SAP-/- IL15-/-

