Changing a note type without requiring a full new sync.

Copyright: Arthur Milchior arthur@milchior.fr
License: GNU GPL, version 3 or later; http://www.gnu.org/copyleft/gpl.html
Feel free to contribute to this code on https://github.com/Arthur-Milchior/anki-change-note-type
Anki add-on number: 719871418

"Change card's type" does not require a new upload of the database.
The only downside being that the identifier of the note change. 
I.e. you lose the content provided by the «info» button (i.e. the list of dates at which you clicked on again, hard, good, easy).
Note however that the number of leech, the easyness, the date of next review, etc... are all preserved.

#For developpers
The method change, of ModelManager, is changed. It now returns the list of the new note ids of the changed note

Update 2018-01-10: The creation date of note is preserved as much as possible (the date is incremented of a few miliseconds). The creation date of card is not preserved.