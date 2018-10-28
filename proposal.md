# X-Team 115 Project Proposal: Searchable Journal

## Problem Description

Many people like to keep a journal electronically, to avoid the fuss of carrying a paper journal around everywhere.  Electronic Journals also have the advantage of being searchable, so a user can search the journal for key words to quickly find something they've written.  Our program will implement an electronic journal with keyword-search functionality to provide our users with these advantages.

## Questions to answer for Exercise #2
1. Name: Give your project proposal a name (and edit the top line of this file)

"Searchable Journal"

2. Output: Describe the output your program will produce.  Include an example format of the output produced.

Our program will have two types of output.  The first will simply be the text of the journal entry they've previously inputed, and the second will be a list of journal entries that contain the keyword the user searched for.  In the second type of output, the user will be able to click on the search results to navigate directly to the journal entry it represents.
 
Example output 1 format:

(Journal Entry Title)

(Journal Entry Date)
  
(Journal Entry Main Text Body)
 
Example output 2 format:

(search keyword inputted by the user)
 
(Journal Entry 1 containing the keyword)

(Journal Entry 2 containing the keyword)

(Journal Entry 3 containing the keyword)
...

3. Input: Describe the data that is needed to solve your problem. Include an example format of the input data.

To input a journal entry, the user will input a string of text to be used at the journal entry's title and a string of text that is the body of the journal entry.  

Example:

Title: "A great day"

Body: "Today I at 15 bowls of cereal."
 
When searching for a journal entry containing a specific keyword, the user will enter the keyword they are searching for

Example:

Search Keyword: "cereal"


4. User Interface: Describe a user interface for your program.  Use text menus or a simple graphic user interface.

Our program will use a simple GUI.  The main screen will be a scrollable listing (descending by date) of all the journal entries the user has inputted previously.  Clicking on any of these entries will pull up a screen devoted to the text-body of the journal entry.  The main screen will also have a button that says "search",  clicking this button will move the user to a search screen where they will be prompted to enter a search keyword.  Once they enter the keyword, a scrollable list of all journal entries that match the user's keyword (also ordered descending by date) will be outputed to the screen. Similarly to the main screen, clicking on any of these journal entries will navigate to a screen devoted to the text-body of that journal entry.

5. Types List: Break your solution idea down into units that you think can be implemented with a single class.
Name each interface or class and briefly describe its function or purpose.

Main.java
 This will be the main entry point into the program.  It will handle user input and display the corresponding output.

JournalEntry.java
 An instance of this class represents a single journal entry.  This will encapsulate the entry's date, title, and text-body.

Journal.java
 There will only be one instance of this class, which will contain a list (ordered by Date) of all of the journal entries.

HashTable.java
 This will be a hash table (to be used to optimize the search functionality) where the key will be a single word and the value will be a list of all the journal entries that contain that word.


## Edit and Submit this file and any figures referenced by this document.

