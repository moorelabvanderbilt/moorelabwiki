<!-- TITLE: Mouse Colony Spreadsheet -->

The main spreadsheet that I use to manage the mouse colony is called **Mouse Colony** and is hosted in Google Drive.

It is split into 3 tabs: Available, Mating, and Stats. These tabs are outlined below.
# Available
The Available tab shows the mice that we have in our colony that are not currently in breeding pairs. These mice are either available for use in experiments, or are currently enrolled in experiments. Each row represents one cage.

The columns are as follows:

* **(blank)**: this first column is just a empty column that I use during the census. I'll use this column to mark a cage as present, so I can delete all the ones that were unaccounted for.
* **Strain**: this contains the strain/genotype of the mouse.
* **Cage #**: this contains the cage card number.
* **DOB**: this contains the date of birth for the mice in the cage.
* **Age**: this is the age of the mice in weeks. This is auto-calculated based on the DOB.
* **Sex**: this is the sex of the mice.
* **#**: this is how many mice there are in this cage.
* **Comments**: this contains any comments about the status of these mice. We usually use this if a mouse is being saved for something, or has been injected with something.
* **(blank)**: this column is not used for anything - however, the macros that organize this sheet assume that it will be there, so it cannot be deleted.
* **Protocol**: this contains the protocol number that this cage is associated with. This is auto-filled based on the protocols numbers in the Stats tab.
* **Room**: this contains the room number that this cage is in.

Generally, this spreadsheet operates like a normal spreadsheet. However, it does have a macro associated with it that groups the mice by strain and sex, and sorts them by DOB. It also finds the protocol numbers based on the groupings given in the Stats tab.

This macro is triggered by going to the Mouse Functions menu item at the top of the page and pressing Sort Sheets.

# Matings
The Matings tab shows the mice that are currently in breeding pairs. Each row represents one cage.

The columns are as follows: 

**Expected offspring**:
**Cage #**: 	
**DOB**: 	
**DOW**:	
**# pups**:
**Comments**:
**Date Paired**:
**Last Wean**:
**F**:
M	Strain F	DOB F	Strain M	DOB M	Days since event	Too old?	Protocol	Room