osr-random-generator
====================

A random generator for creating characters for old school fantasy rpgs.

Right now it just creates characters for Lamentations of the Flame Princess or Labyrinth Lord rules (though they could be easily used for other OSR type games, and there is some Swords & Wizardry support).

Online version at: http://derikb.github.io/osr-random-generator/

Install
-------

* Click the "Download ZIP" button at right to get a zip file of the app.
* Unzip the file ("osr-random-generator-master.zip") on your computer (most of the time, just double click and your computer should know what to do).
* Find the new folder that was made (should be called: "osr-random-generator-master").
* Open the "index.html" file in your browser (Chrome is preferred and the only one I've tested).
* Give it a try.
* If you save settings/characters they will be saved in your browser's local storage (so be careful when clearing data from your browser).
* Let me know if you have trouble or feature suggestions.

Usage
-----

* Use the Settings tab to set some parameters (rules, which data lists to use, how many traits to include).
* Use the NPCs tab to create new characters. You can click on most fields to edit them (some fields that are generated exclusively from other fields cannot be edited, i.e. Attack Bonus, AC). Click the first icon to save or the second to remove/delete.
* Assign characters to groups for sorting purposes on the "Saved Characters" list. From that list you can open the full character details (the character card will appear in the right column) or delete the character.
* Try printing. You should only get a print-out of the characters displayed in the right column, they should be set up as 5" wide cards (it's hard to limit it to 3" height, but I was going for a 3x5 card output, maybe I can improve this later on).

Credits
------

Coding by Derik A. Badman.

Made with: <a href="http://jquery.com">jQuery</a>, <a href="http://getbootstrap.com/">Bootstrap</a>, <a href="http://backbonejs.org/">Backbone</a> (with the <a href="https://github.com/jeromegn/Backbone.localStorage">Local Storage adapter</a>), and <a href="http://underscorejs.org/">Underscore</a>.

### DataSources

* <a href="http://www.lotfp.com/">Lamentations of the Flame Princess</a> rules by James Edward Raggi IV.
* <a href="http://www.goblinoidgames.com/labyrinthlord.html">Labyrinth Lord</a> rules by Daniel Proctor.
* Occupations list adapted from <a href="http://thegruenextdoor.blogspot.com/2013/12/characters-in-flesh.html">Christopher Adams</a>
* Spell list as compiled by <a href="https://plus.google.com/u/0/102353265648840654058/about">Adam Taylor</a> by way of html from <a href="http://save.vs.totalpartykill.ca/grab-bag/">Ramanan Sivaranjan</a> (which I converted into JSON).
* Appearance and Personality lists from <a href="http://www.lulu.com/shop/courtney-campbell/on-the-non-player-character/ebook/product-21094127.html">On the Non-Player Character</a> by <a href="http://hackslashmaster.blogspot.com/">Courtney Campbell</a>.
* Personality and Quirks lists from <a href="http://www.roleplayingtips.com/articles/npc-essentials.html">GM Mastery: NPC Essentials</a> by <a href="http://www.roleplayingtips.com/">Johnn Four</a>
* Holmesian Names are adapted from the <a href="http://zenopusarchives.blogspot.com/2013/07/random-names-one-sheet.html">Zenopus Archives' Holmesian Name Generator</a>.
* <a href="http://jrients.blogspot.com/2011/09/random-cornish-names.html">Cornish</a> and <a href="http://jrients.blogspot.com/2012/01/medieval-flemish-names.html">Flemish</a> first names taken from Jeff Rients.
* <a href="http://www.swordsandwizardry.com/">Swords &amp; Wizardry</a> rules by Matthew J. Finch</a>
* Goals list primarily taken from <a href="http://blog.retroroleplaying.com/2013/03/tarnhelms-terrible-tome-house-rules-for.html">Tarnheim's Terrible Tome</a> by Randall S Stukey

### Notes

* My original goal for this application was to create something that would be directly useful for me in prepping sessions for my game (we use LotFP rules), but that also might be useful during a session if something quick needs to be rolled up. I had collected so many books and pdfs and tables from various places that it was all a little overwhelming and hard to keep track of, so I thought I might be able to easily consolidate what I wanted to use in a simple way.
* I tried to make the application without any server-based component so that it could be downloaded and run in the browser without any difficult set-up procedure. One could even run it without a network connection if all the required js libraries were downloaded locally.
* I'm also trying to make the data elements of the app easily expandable so users can customize what tables they want to use. Unfortunately there's no simple way to take a table from a book, pdf, or blog post and make it structured enough that the application could make use of it. But if you are willing to put in some conversion time (much easier if you have a good text editor and some knowledge of regular expressions, which is how I converted all the data), it should be pretty easy to add your own tables.
* Warning: I've only tested this in Chrome (desktop and Android tablet) and Firefox, any other browser may not work right (especially Internet Explorer). I'll do more testing later (especially for mobile).
