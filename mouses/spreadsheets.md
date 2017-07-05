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

* **Expected offspring**: the offspring you expect to get from this mating.
  *  For true-breeding mice, this is just the same strain as the parents.
  *  For non-true-breeding mice, this is the strain that you are aiming to get from the mating.
* **Cage #**: the number on the cage card.
* **DOB**: if this cage currently has pups, the day that they were born.
* **DOW**: if this cage currently has pups, the day they will be old enough to wean.
  * This cell will turn orange when the current date is equal to or later than the wean date.
* **# pups**: if this cage currently has pups, the number of pups in the cage.
* **Comments**: any misc. comments you'd like to note about this cage.
* **Date Paired**: the date that these mice were put together into as a mating cage.
* **Last Wean**: the date that mice were last weaned from this cage.
* **F**: the number of female breeders in this cage. Usually this is 1.
* **M**: the number of male breeders in this cage. Usually this is 1.	
* **Strain F**: the strain of the female breeder in this cage.	
* **DOB F**: the date of birth of the female breeder in this cage.	
* **Strain M**: the strain of the male breeder in this cage.
* **DOB M**: the date of birth of the male breeder in this cage.
* **Days since event**: this field is auto-calculated to be the number of days since the last wean from this cage (or if no weanings, from the date paired).
  * This field calculates using the **Last Wean** field and the **Date Paired** field.
  * This cell will turn red if it has been 60 days or more since the last wean.
* **Too old?**: this field is auto-calculated to be the number of days until any of the breeders in this cage are 9 months old.
  * This field calculates using the **DOB F** and the **DOB M** field.
  * This cell will turn red if either of the breeders in this cage is 9 months old or older.

# Stats
The Stats tab contains miscellaneous information about the whole colony. 

In the top left, there are counts of how many mice and cages we currently have. 

There is also a measure of how efficiently the mice are currently being stored in "Avg mice / cage". Ideally, this would be around 3.5 or above. The more low-density cages we have, the lower (worse) this number will be. Try to combine cages of similarly aged mice or sac unneeded single mice to increase the number.

In the lower left, there is a count of cages by protocols. This is useful because Dan will sometimes want a certain ratio of mouse spending on certain protocols, so this calculator helps you see which protocols should get more or less mice to reach the right ratio. This is also useful if you need to remove all mice of a certain protocol because you can see how many you have left.

In the top right, there is a list of protocol numbers. These are taken off of new cage cards when they are delivered and represent the first and last card numbers of that set of cards. The number to their right is how many cages are still in the colony from that cage card set. When there are none left, this field turns red. The Sort Sheets macro uses these numbers to fill in the protocol numbers of the cages listed in both the Available and Matings tabs.