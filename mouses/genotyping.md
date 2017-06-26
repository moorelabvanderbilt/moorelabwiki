<!-- TITLE: Genotyping -->

**Genotyping** is the procedure that we use to determine the DNA genotype of mice. 

For most transgenic and knockout mice that we use, there is not a readily observable phenotype that indicates the genotype of the mouse. Therefore, we must use genotyping to absolutely confirm the genotype of any non-true-breeding offspring.

# Collecting tissue
**Required items**
* PCR tubes, 8-tube strip, with individually attached lids ()
* Scissors
* Ear tags ()
* Ear tag appliers
* Sharpie to label tubes

**Collection**  

Label the tube strips with letters (A, B...) on one of the ends of the strip. This will be the tube 1 in that strip; the final tube is tube 8.

In the mouse room hood, place a cage with mice to genotype. Place an ear tag on each of the mice. 

Using the scissors, cut a small bit of the end of the tail off and place it into one of the tubes in the strip. You only need to get about 1-2 mm of tail.

Close the lid of the tube that you placed the tail in. Write down the ear tag number of the mouse and the tube number that you put the tail in so that you can match genotypes to mice when you are finished genotyping.

Repeat this process for all the mice you need genotyped. Bring your tubes with tail clippings back to lab.
# Extracting DNA from tissue
## Dirty prep
*Adapted from [Preparation of PCR-Quality Mouse Genomic DNA with Hot Sodium Hydroxide and Tris (HotSHOT). *BioTechniques* 29:52-54 (July 2000).](http://www.biotechniques.com/BiotechniquesJournal/2000/July/Preparation-of-PCR-Quality-Mouse-Genomic-DNA-with-Hot-Sodium-Hydroxide-and-Tris-HotSHOT/biotechniques-44169.html)*

**Required items**
* NaOH, 50 mM
* Tris-HCl, 40 mM
* PCR machine

Add 

## Clean prep
For some PCR protocols, the dirty prep does not amplify reliably. For these, you have to use a cleaner DNA prep kit, like the [QIAGEN DNeasy Blood and Tissue Kit](https://www.qiagen.com/us/shop/sample-technologies/dna/genomic-dna/dneasy-blood-and-tissue-kit/), which you can buy from the Core.

Simply follow the directions in the kit to get more pure DNA. However, the full protocol is much more labor intensive and takes longer than the dirty prep, so if the dirty prep works for your PCR protocol, use that instead.

The only protocol that we currently have that requires the clean prep is the SAP protocol.

# PCR Amplification
*This is a general overview of PCR that could be adapted for any gene. For PCR mixes and protocols to use with specific mouse strains, see [this page on mouse strains](/mouses/mouse-strains).*

Once you have DNA, it's time to amplify your segment of interest so it can be seen when you run it on a gel.

First, you need to mix your DNA into individual PCR mixes. Mix a master mix of everything except for the DNA. 

This recipe is for a single DNA sample, so multiply this by how many samples you have. In addition, sometimes you'll have more than two primers; this is okay, just reduce the amount of water so that the whole mix still comes out to 23 ul per sample.

Reagent | Amount (per rxn) | Stock Conc. | Final Conc.
--- | --- | --- | ---
Forward Primer | 1.5 ul | 10 uM | 0.6 uM
Reverse Primer | 1.5 ul | 10 uM | 0.6 uM
Promega Green Mix | 12.5 ul | 2X | 1X
Nuclease-free water | to 23 ul | - | -

The [Promega Green Mix](https://www.promega.com/products/pcr/endpoint-pcr/gotaq-flexi-dna-polymerase/) is available from the Core. It contains the *Taq* DNA polymerase, all four dNTPs, dyes, and salts which are necessary for the reaction to take place.

Aliquot 23 ul of this master mix into PCR tubes, then add 2.0 ul of each DNA sample to a separate tube, for a total of 25 ul per reaction.

Close the caps of the PCR tubes and place them into the PCR machine. Close and tighten the lid of the machine to keep the caps of the tubes on (the tubes get very hot during cycling, so if the caps aren't secured they can burst off and your reaction liquid inside can evaporate).

Set the PCR machine to use the protocol you need. Many protocols are saved in the machine already. If you need to add another protocol, see [Adding a new protocol to the cycler](/mouses/genotyping#adding-a-new-protocol-to-the-cycler) below.

## Creating a new protocol

All of the protocols that we use I stick to a simple formula:

Step | Temperature (&deg;C) | Time (m:ss)
--- | --- | ---
initialization | 94 | 3:00
- | - | start loop 35x
denaturation | 94 | 1:00
annealing | depends on primers | 1:00
elongation | 72 | 1:00
- | - | end loop
final elongation | 72 | 2:00
hold | 4 | &#x221e;

The only temperature that you have to determine is the annealing temperature. There are several online calculators for this - one that I use is [the one from Promega](http://www.promega.com/a/apps/biomath/?calc=tm), since then you can select Green Mix as your buffer mixture. However, this only calculates the *melting* temperature of one primer at a time. The *annealing* temperature (what you use in the PCR protocol) is generally about 5&deg;C below the lowest melting temperature.

In addition to using the calculator, if you have a PCR machine that can do a gradient of temperatures, you can set the annealing temperature step to a gradient of about &plusmn;5&deg;C from the annealing temperature suggested by the above calculation. If you run this gradient protocol with a single positive control sample for the gene of interest, you can see the temperature that produced the best band on the resulting gel.

In addition to this simple protocol, there are more complicated PCR protocols (often listed in the genotyping section of Jackson's website), like where the annealing temperature rises slightly each cycle. They have never worked very well for me, so I just use the simple ones.

## Adding a new protocol to the cycler

Our PCR machine is very old, so it's kind of a weird puzzle to get stuff entered.

Starting on the home screen, using the arrow buttons to move the selection, select **FILES**. Press **Enter**.

Select **New**. Press **Enter**.

It will created a new protocol, called UNNAMED, and bring you to the editor screen.  
Select where it says **BLOCK**, and press **Sel** until it changes to **TUBE**.

Select the asterisks next to **LID=** and set it to 105&deg; using the numpad.

Using the arrow buttons, navigate the cursor to the left of **end**.

Press **Sel** until the row changes to **1 T=\*\*\*\*&deg; \*\*\:\*\*\:\*\**


