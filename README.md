# Navaren's Name Maker
![Showcase Image](https://github.com/Daxiongmao87/navarens-name-maker/blob/639497e17658726ca70ef325105f352fd8e02f44/images/Showcase.gif?raw=true)

## Description
Navaren's Name Maker aims to be a robust and exhaustive tool for creating names for anything and everything.

## Installation
1. Go to the "Add-on Modules" tab in Foundry Setup
2. Click "Install Module" and search for **Navaren's Name Maker** OR alternatively copy this link ```https://www.com``` and paste it on the bottom where it says "Manifest URL:", then click the install button.
3. Load your world.
4. Navigate to the Settings tab, then click the "Manage Modules" button.
5. Search for **Navaren's Name Maker** module, and ensure the checkbox is checked, then click on the "Save Module Settings" button.

## Usage
1. On the top of some windows (such as actor windows) there is a "Make Name" button.  Clicking it will open the Maker List window.
2. This window will contain any "Makers" you've created, so naturally it will be empty if you have yet to create one.  To create a "Maker" click on the "New Maker" button on the bottom.
3. Currently there's only one algorithm to **Navaren's Name Maker** and it's based on an algorithm called a Markov Chain.  This is probably the most complex part so lets go through each portion individually:
  a. **Maker Name.** Just a name or label to give to this Maker
  b. **Dictionary.** This is a list of names or words you would like the maker to use as inspiration for new names.  An example of **human male names** would be something like this: 
  ```Michael,Christopher,Matthew,Michael,Christopher,Matthew,Joshua,Daniel,David,James,Robert,John,Joseph,Andrew,Ryan,etc.```
  c. **Delimier. (Default: ",")** This is the character the maker will use to determine where one dictinoary item ends and another begins.  Commas are often used as delimiters.
  d. **Context Depth. (Default: "2")** As the maker creates a new name, this is the number of characters back it will reference for context when deciding on the next character.  The larger the number, the more structured the name will become, at the cost of less variety.  It's suggested that you have a larger dictionary the higher you place this number.
  e. **Length Range.** This is the length the maker will *try* to reach when creating a new name.  The minimum length should always be above the **Relation Depth**.
4. Once all of the fields detailed above are filled, you can then save the new Maker by clicking the "Submit" button.
5.  Your Maker List should now populate with your new maker.  Clicking on its button will create 3 names located on the bottom half of this window.
6.  Once you've found a name that you're satisfied with, clicking on that name's button will copy it to your clipboard to paste wherever you'd like.

## Future Plans
* Other procedural methods to name generation that would fit other name styles
  * Like random affixes to generate clan names like "Red + Hammer"
* The ability to create full names using multiple different name generation methods.
  * Like having a first name and surname generated by a markov chain algorihm, a middle name generated by random affixes, etc for something like: Uthar "Demon's Bane" Kron.
* Adding the "Make Name" button to certain name fields (like actors, items, etc), and having a generated name auto-fill that field instead of going to your clipboard.
* Complete redo of the code since it's god-awful. (My first javascript project!)
* Localization

