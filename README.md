osr-random-generator
====================

A random generator for old school fantasy rpgs.

Online version at: http://derikb.github.io/osr-random-generator/

It has a few related functions that are in varying states of development.

1) Random tables: View and roll on random tables. You can add your own tables from the very simple to the rather complex.

2) NPC generator: Creates NPCs (though I guess they could also be quickstart PCs) for Lamentations of the Flame Princess or Labyrinth Lord rules (though they could be easily used for other OSR type games, and there is some Swords & Wizardry support).

3) Dungeon Stocking: Using the Moldvay dungeon stocking rules, Labyrinth Lord monster stats, trap tables from Courtney Campbell, and... well no special yet... it will generate results for Dungeon rooms. Might not be super helpful for actual use, but I'm hoping to improve this later.

4) Wilderness Hex Generation: Put in a terrain type and it will generate hex dressing and encounters of various sorts. Primarily met as a pre-session prep in case your PCs head off into an unplanned wilderness, or as a way to add some extra flavor to travel.

User added tables & customization are an end-goal of this project, and I am hoping to make it as easy as possible, but, in the end, I have to balance a few goals and there is no way to avoid a certain level of complexity to the data.


Install on a Desktop or Laptop
------------------------------

* Click the "Download ZIP" button at right to get a zip file of the app.
* Unzip the file ("osr-random-generator-master.zip") on your computer (most of the time, just double click and your computer should know what to do).
* Find the new folder that was made (should be called: "osr-random-generator-master").
* Open the "index.html" file in your browser (Chrome is preferred and the only one I've really tested, Firefox should work as a second best option).
* Give it a try.
* If you save settings/characters they will be saved in your browser's local storage (so be careful when clearing data from your browser).
* Let me know if you have trouble or feature suggestions.

Install on a Phone or Tablet
----------------------------

* I'm working on getting the code ported to work on Android and iPhone to make it easier to use at the table.
* I have successfully tested a demo of the Android version.


Usage
-----

* Use the Settings tab to set some parameters and defaults. These will be saved in your browser, so will "stick" as long as you don't clear your browser data.
* Use the Random Tables tab to roll results on tables or to choose from the tables.
    * Click on tags to filter the list. Click on the x icon next to the current filter to show all tables again.
* The Import Tables tab let's you save your own tables.
    * The simplest format (put in the table data field) is to use:
        * One random entry per line.
        * To weight a random chance, prefix the entry with a number and two pound signs (i.e. "2##This entry will be twice as likely", "4##This entry is four times as likely").
    * It will also accept a JSON string of data.
        * I still need to document this (and make sure the format is all working right), but if you look in data/randomtables.json you can see some examples.
* Use the NPCs tab to create new characters. You can click on most fields to edit them (some fields that are generated exclusively from other fields cannot be edited, i.e. Attack Bonus, AC). Click the icons to save/remove/delete.
    * Assign characters to groups for sorting purposes on the "Saved Characters" list. From that list you can open the full character details (the character card will appear in the right column) or delete the character.
    * Try printing. You should only get a print-out of the characters displayed in the right column, they should be set up as 5" wide cards (it's hard to limit it to 3" height, but I was going for a 3x5 card output, maybe I can improve this later on).
* Most of the other tabs work similar to the NPCs tab. Many fields can be clicked on to edit them.

Credits
------

Coding by Derik A. Badman.

Made with: <a href="http://jquery.com">jQuery</a>, <a href="http://getbootstrap.com/">Bootstrap</a>, <a href="http://backbonejs.org/">Backbone</a> (with the <a href="https://github.com/jeromegn/Backbone.localStorage">Local Storage adapter</a>), and <a href="http://underscorejs.org/">Underscore</a>.

### DataSources

* For the most part, I am only using data that has an OGL license or is freely available online already. I have no plans to monetize this in any way, so please don't get mad.
* All the tables in the Random Tables tab have source/author information (click the info icon in the main table list).
* <a href="http://www.lotfp.com/">Lamentations of the Flame Princess</a> rules by James Edward Raggi IV.
* <a href="http://www.goblinoidgames.com/labyrinthlord.html">Labyrinth Lord</a> rules by Daniel Proctor.
* Occupations list adapted from <a href="http://thegruenextdoor.blogspot.com/2013/12/characters-in-flesh.html">Christopher Adams</a>
* Spell list as compiled by <a href="https://plus.google.com/u/0/102353265648840654058/about">Adam Taylor</a> by way of html from <a href="http://save.vs.totalpartykill.ca/grab-bag/">Ramanan Sivaranjan</a> (which I converted into JSON).
* Appearance and Personality lists from <a href="http://www.lulu.com/shop/courtney-campbell/on-the-non-player-character/ebook/product-21094127.html">On the Non-Player Character</a> by <a href="http://hackslashmaster.blogspot.com/">Courtney Campbell</a>.
* Personality and Quirks lists from <a href="http://www.roleplayingtips.com/articles/npc-essentials.html">GM Mastery: NPC Essentials</a> by <a href="http://www.roleplayingtips.com/">Johnn Four</a>
* Holmesian Names are adapted from the <a href="http://zenopusarchives.blogspot.com/2013/07/random-names-one-sheet.html">Zenopus Archives' Holmesian Name Generator</a>.
* <a href="http://jrients.blogspot.com/2011/09/random-cornish-names.html">Cornish</a> and <a href="http://jrients.blogspot.com/2012/01/medieval-flemish-names.html">Flemish</a> first names taken from Jeff Rients. Other names I compiled from various lists online.
* <a href="http://www.swordsandwizardry.com/">Swords &amp; Wizardry</a> rules by Matthew J. Finch</a>
* Goals list primarily taken from <a href="http://blog.retroroleplaying.com/2013/03/tarnhelms-terrible-tome-house-rules-for.html">Tarnheim's Terrible Tome</a> by Randall S Stukey
* Labyrinth Lord monster data adapted from <a href="http://www.wizardawn.com/rpg/tool_data.php">Wizardawn's Data files</a>.
* Dungeon generator "special" results from: <a href=\"http://rolesrules.blogspot.com/2014/02/download-bag-of-tricks-2-now-easier.html\">Bag of Tricks 2</a> by Roger S.G. Sorolla

### Notes

* My original goal for this application was to create something that would be directly useful for me in prepping sessions for my game (we use LotFP rules), but that also might be useful during a session if something quick needs to be rolled up. I had collected so many books and pdfs and tables from various places that it was all a little overwhelming and hard to keep track of, so I thought I might be able to easily consolidate what I wanted to use in a simple way.
* I tried to make the application without any server-based component so that it could be downloaded and run in the browser without any difficult set-up procedure. One could even run it without a network connection if all the required js libraries were downloaded locally.
* I'm also trying to make the data elements of the app easily expandable so users can customize what tables they want to use. Unfortunately there's no simple way to take a table from a book, pdf, or blog post and make it structured enough that the application could make use of it. But if you are willing to put in some conversion time (much easier if you have a good text editor and some knowledge of regular expressions, which is how I converted all the data), it should be pretty easy to add your own tables.
* Warning: I've only tested this in Chrome (desktop and Android tablet) and Firefox, any other browser may not work right (especially Internet Explorer). I'll do more testing later (especially for mobile).
