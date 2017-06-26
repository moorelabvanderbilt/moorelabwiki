<!-- TITLE: Genotyping -->

**Genotyping** is the procedure that we use to determine the DNA genotype of mice. 

For most transgenic and knockout mice that we use, there is not a readily observable phenotype that indicates the genotype of the mouse. Therefore, we must use genotyping to absolutely confirm the genotype of any non-true-breeding offspring.

# Collecting tissue
**Required items**
* PCR tubes, 8-tube strip, with individually attached lids (e.g. [product 1402-2900 from USA Scientific](http://www.usascientific.com/0.2ml-pcr-8-tube-strip-indivattached-caps.aspx))
* Scissors
* Ear tags (see [Ear Tags](/mouses/ear-tags) for more information)
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

Add 75 uL NaOH to each tail clipping. Make sure the clipping is submerged in the NaOH - vortexing the tubes can help with this. 

Place in the PCR machine at 95&deg;C for 30 min. 

Remove the tubes and vortex. There may be undigested hair in the mixture; this is normal.

Add 75 ul Tris-HCl to each tube and vortex again. 

This mixture contains your DNA and can be used in PCR protocols. It can also be stored at 4&deg;C for a long time.

## Clean prep
For some PCR protocols, the dirty prep does not amplify reliably. For these, you have to use a cleaner DNA prep kit, like the [QIAGEN DNeasy Blood and Tissue Kit](https://www.qiagen.com/us/shop/sample-technologies/dna/genomic-dna/dneasy-blood-and-tissue-kit/), which you can buy from the Core.

Simply follow the directions in the kit to get more pure DNA. However, the full protocol is much more labor intensive and takes longer than the dirty prep, so if the dirty prep works for your PCR protocol, use that instead.

The only protocol that we currently have that requires the clean prep is the [SAP protocol](/mouses/mouse-strains#sap).

# PCR Amplification
*This is a general overview of PCR that could be adapted for any gene. For PCR mixes and protocols to use with specific mouse strains, see [this page on mouse strains](/mouses/mouse-strains).*

Once you have DNA, it's time to amplify your segment of interest so it can be seen when you run it on a gel.

First, you need to mix your DNA into individual PCR mixes. Mix a master mix of everything except for the DNA. 

This recipe is for a single DNA sample, so multiply this by how many samples you have. In addition, sometimes you'll have more than two primers; this is okay, just reduce the amount of water so that the whole mix still comes out to 23 uL per sample.

Reagent | Amount (per rxn) | Stock Conc. | Final Conc.
--- | --- | --- | ---
Forward Primer | 1.5 uL | 10 uM | 0.6 uM
Reverse Primer | 1.5 uL | 10 uM | 0.6 uM
Promega Green Mix | 12.5 uL | 2X | 1X
Nuclease-free water | to 23 uL | - | -

The [Promega Green Mix](https://www.promega.com/products/pcr/endpoint-pcr/gotaq-flexi-dna-polymerase/) is available from the Core. It contains the *Taq* DNA polymerase, all four dNTPs, dyes, and salts which are necessary for the reaction to take place.

Aliquot 23 uL of this master mix into PCR tubes, then add 2.0 uL of each DNA sample to a separate tube, for a total of 25 uL per reaction.

Close the caps of the PCR tubes and place them into the PCR machine. Close and tighten the lid of the machine to keep the caps of the tubes on (the tubes get very hot during cycling, so if the caps aren't secured they can burst off and your reaction liquid inside can evaporate).

Set the PCR machine to use the protocol you need. Many protocols are saved in the machine already. If you need to add another protocol, see [Adding a new protocol to the cycler](/mouses/genotyping#adding-a-new-protocol-to-the-cycler) below.

When the PCR is done, the machine will hold the reactions at 4&deg;C. If you need to remove them but don't want to run them on a gel just yet, they can be stored at 4&deg;C in the fridge.

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

Our PCR machine is very old, so it's kind of a weird boring puzzle to interact with the display. If you're having trouble with this guide, check out the manual saved in the `/Protocols Etc./Equipment Manuals` folder on the server.

Starting on the home screen, using the arrow buttons to move the selection, select **FILES**. Press **Enter**.

![cycler 01](/uploads/genotyping/genotyping-00001.jpg "cycler 01")

Select **New**. Press **Enter**.

![cycler 02](/uploads/genotyping/genotyping-00002.jpg "cycler 02")

It will created a new protocol, called UNNAMED, and bring you to the editor screen.  
Select where it says **BLOCK**, and press **Sel** until it changes to **TUBE**.

![cycler 03](/uploads/genotyping/genotyping-00003.jpg "cycler 03")

Select the asterisks next to **LID=** and set it to 105&deg; using the numpad.

![cycler 04](/uploads/genotyping/genotyping-00004.jpg "cycler 04")

Using the arrow buttons, navigate the cursor to the left of **end**.

![cycler 05](/uploads/genotyping/genotyping-00005.jpg "cycler 05")

Press **Sel** until the row changes to **1 T=...** as shown.

![cycler 06](/uploads/genotyping/genotyping-00006.jpg "cycler 06")

Using the numpad, change the two sets of asterisks to the temperature and the time, respectively.

![cycler 07](/uploads/genotyping/genotyping-00007.jpg "cycler 07")

Again, navigate the cursor to the left of **end**. Repeat the previous steps for the other temperatures in the protocol. Note you do not have to specify the start of a loop until later.

When you reach the end of the loop, on **end**, press **Sel** until the row changes to **GOTO...** as shown.

![cycler 08](/uploads/genotyping/genotyping-00008.jpg "cycler 08")

Change the first set of asterisks to the step number of the start of the loop. Change the second set of asterisks to the number of times you want the loop to repeat.

When you reach the hold step, on **end**, press **Sel** until the row changes to **HOLD...** as shown. Set the temperature at which to hold.

![cycler 09](/uploads/genotyping/genotyping-00009.jpg "cycler 09")

Press **Exit**. The machine will prompt you to save the protocol. Choose **YES**. Press **Enter**.  
Using the arrow keys, select the letter in **UNNAMED** that you'd like to change. To cycle through the alphabet, press **Sel**. To enter a number, use the numpad. To delete a letter, press **Del**.

![cycler 10](/uploads/genotyping/genotyping-00010.jpg "cycler 10")

Press **Enter** to save the protocol. 

# Making a gel
While the PCR machine is running, it's good to go ahead and make your gel so that it is cooled and ready when the PCR is done.

Add 100 mL 1X TAE buffer to a 500 mL Erlenmeyer flask. Add 1.5 g agarose powder to the buffer. Swirl it around and put it in the microwave on high for 1 min 30 sec.

Put on a hot glove and take the flask out. Add 10 uL [SYBR Safe gel dye](https://www.thermofisher.com/us/en/home/life-science/dna-rna-purification-analysis/nucleic-acid-gel-electrophoresis/dna-stains/sybr-safe.html) (available at the Core). Swirl the flask until the dye is evenly distributed.

Place a gel tray in the caster as shown. Take care that the rubber gaskets do not roll out of place when sliding it in - this can cause a leak. 

Pour the contents of the flask into the gel tray. Wash the flask out with water and leave to dry.

Using the end of a gel comb, push any bubbles in the surface of the gel to the bottom end of the gel. 

Place the desired size combs in the slots in the gel tray. Leave to set (about 1 hour at room temperature).

# Running a gel
After the PCR is finished and the gel is set, it's time to run the PCR product in the gel so you can see the bands.

Remove the combs from the gel tray, taking care to keep the wells in the gel intact. Remove the gel tray with the gel from the caster and place it in the buffer chamber as shown. Make sure the gel is completely submerged in 1X TAE in the chamber.

Starting with the second well (leave the first well open for the DNA ladder), pipette about 10 uL of each PCR product into the wells of the gel (use 8 uL if you've used the 40-well comb). Keep them in the same order as they've been in so you can match them to the mice later.

I like to leave the well on the end open for a ladder too, if you have 28+ samples. Sometimes the gel advances unevenly so it's good to have a ladder on either side of the gel.

Pipette 5 uL 100bp DNA ladder (available at the Core) into the wells that you've left open. I like to have at least two ladders per row of wells.

Place the lid on the buffer chamber as shown, plugging the wires onto the contacts on the side of the chamber.

Set the power supply to 125 V and about 28 min, and press **run**. 

If the bands run off the edge of the gel, reduce the time a bit. You can also stop it early if you see that it's going to run off (the yellow dye marks the front of the bands).

# Imaging a gel
When the gel is finished running, you'll take it up to the Core to take a photo of the gel using their imager.

Using the gel tray, or after transferring the gel to a plastic box, carry the gel up to the Core on the 9th floor. Bring a flash drive with you. 

It's best to wear a glove on your right hand to touch the mouse and keyboard and gel trays. We use SYBR Safe dye, which is safe (hence the name), but a lot of people still use ethidium bromide, which is a potent carcinogen. Everything around that computer and imager up there is probably covered in ethidium bromide, so you do not want that to touch your skin.

The door just past the main Core store is where all the imagers are. Go to the second computer/imager on the left side of the room.

Take the blue tray out of the rack above your head. Take the gel out of your carrying container and place it on the blue tray. Try to press out any bubbles that form underneath the gel.

Open the imager and slide the tray in, gel-side first.

If it's not already open, open ImageLab. If the **New Protocol** window is not already showing, bring it up by pressing the button on the ribbon at the top-left.

Select **Nucleic acid gels > SYBR Safe**. Under **Optimize exposure for...**, select **Intense bands** (Generally, this works. Obviously, if your bands are faint, choose **Faint bands** and re-image). Uncheck **Highlight saturated pixels**.

Press **Run Protocol**.

It will show a picture of what your gel looks like. If it looks good, select **File > Export for Publication**. Select **600 dpi** and press export. Plug in your flash drive and export the image to the flash drive.

Take the gel out of the imager and put it back into your carrying container. We don't need it now that we have the photo, but I'm still not sure if we're allowed to throw them away in the Core (because of the EtBr problem mentioned above), so I bring them back to lab and then throw them out.

Clean off the blue tray with water and KimWipes and return it to the rack.

Get your flash drive out of the computer and come back to lab.

# Reading the gel
With the expected band sizes of your PCR protocol and the photo of the gel, you can figure out which mice have the genotype that you want. 

