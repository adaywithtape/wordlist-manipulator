# Other options #
  * Menu option 10 Miscellaneous fun

  * Menu option f  File Information

  * Menu option h  Version information and listing of all functions

  * Menu option u  Check for updates


---


# Menu Option 10 #

Sub-menu for option 10. **Miscellaneous fun** consists of;
  1. Check possible wordlist sizes (with same min-max length only).
  1. Create a wordlist from a range of dates (datelist).
  1. Strip SSIDs from a kismet generated .nettxt file.
  1. Basic leetify options for wordlist.
  1. Leetify/Permute wordlist (Gitsnik's permute.pl script)
  1. Decode / Encode file with ROT18
  1. Decode / Encode file with ROT47
  1. Check all possible shifts on Caesar cipher shifted text


---


**10.1 check possible wordlist sizes**

This is a small script to check what the size would be of a wordlist created with for instance 'crunch'.
It only calculates sizes based on the same min/max length of words.

You are prompted to enter ;
> - the number of characters that would be used in creating the wordlist

> - the length of the words in wordlist (for instance 8, the minumum length for WPA)

> - the number of passphrases your system can handle per second. _(you can leave this item blank)_

The script will then calculate the estimated number of lines/words in the wordlist.

If you entered how many passphrases/sec your system can handle, then it will also show you an estimate on how much time it would take to go through such a wordlist.(not the creation time)

Finally it will show the estimated size of the wordlist in Bytes through to Petabytes.

![http://i94.photobucket.com/albums/l112/TAPE_RULEZ/crunch_size_wiki-1.png](http://i94.photobucket.com/albums/l112/TAPE_RULEZ/crunch_size_wiki-1.png)


---


**10.2 Create a wordlist based on dates _(datelist)_**

This script will create a date wordlist (numeric) based on a given range of dates.

You are first prompted for a start date in format yyyy-mm-dd

Then you are prompted for an end date in format yyyy-mm-dd

You then need to enter an output file name for the wordlist.

Then enter the desired output format of the date as per the guidance given.

Finally you can enter whether you want a spacing character in between days/months/years or not.

The script will list all dates in between the dates as specified and will use the output format as chosen as well as include the spacing character if one was entered.

![http://i94.photobucket.com/albums/l112/TAPE_RULEZ/dates_wiki.png](http://i94.photobucket.com/albums/l112/TAPE_RULEZ/dates_wiki.png)


---

**10.3 Strip SSIDs from a kismet generated .nettxt file**

This script is intended to strip SSIDs from a Kismet generated .nettxt file.
This can be used to for instance create wordlists with a great number of real-world SSIDs which can be used together with mdk3 to audit hidden SSIDs.

Same as usual, you are prompted for input .nettxt file, and also for an output file for the SSIDs.

![http://i94.photobucket.com/albums/l112/TAPE_RULEZ/ssid_strip_wiki-1.jpg](http://i94.photobucket.com/albums/l112/TAPE_RULEZ/ssid_strip_wiki-1.jpg)


---


**10.4 Basic leetify options for wordlist**

This is a basic form of 'leetifying' a wordlist by choosing which types of letter alteration you want to use.

You will be prompted for an input file and an output file.

Then you will be prompted to choose from a list of different letter alteration possibilities.

![http://i94.photobucket.com/albums/l112/TAPE_RULEZ/leet_wiki.png](http://i94.photobucket.com/albums/l112/TAPE_RULEZ/leet_wiki.png)


---


**10.5 Leetify/Permute wordlist (Gitsnik's permute.pl script)**

This script is written by Gitsnik, and I shamelessly included it ;)

It creates all possible permutations of the letters in each word and writes these to a new file, its a great bit of code.

The only drawback is that this can **massively** increase the wordlist size.

![http://i94.photobucket.com/albums/l112/TAPE_RULEZ/permute_wiki.png](http://i94.photobucket.com/albums/l112/TAPE_RULEZ/permute_wiki.png)


---


**10.6 ROT18 Encode/Decode a file**

This will take the text in a file and run ROT18 encoding on it;

Shifting letters up 13 characters and numeric values up 5 characters allowing the same encoding method to be used for 'encryption' and 'decryption'.

![http://i94.photobucket.com/albums/l112/TAPE_RULEZ/wlm-rot18_zpsbee5f6bf.png](http://i94.photobucket.com/albums/l112/TAPE_RULEZ/wlm-rot18_zpsbee5f6bf.png)


---


**10.7 ROT47 Encode/Decode a file**

This will take the text in a file and run ROT47 encoding on it.

More elaborate than ROT18 encoding, but still allows the same encoding to be used for both 'encryption' and 'decryption'.

![http://i94.photobucket.com/albums/l112/TAPE_RULEZ/wlm-rot47_zps98698cb4.png](http://i94.photobucket.com/albums/l112/TAPE_RULEZ/wlm-rot47_zps98698cb4.png)


---


**10.8 Check all possible shift values to decode a Caesar cipher shifted text**

Will take user input (not file) and prints all 26 possible Caesar cipher letter substitution shifts.

![http://i94.photobucket.com/albums/l112/TAPE_RULEZ/wlm-caesar_zps01915eaa.png](http://i94.photobucket.com/albums/l112/TAPE_RULEZ/wlm-caesar_zps01915eaa.png)


---


# Menu Option f File Information #

Simply enter a filename and the script will go through it and list ;
> - Filetype

> - Number of lines

> - Longest line

> - File size

> - First and last 3 lines of the file

![http://i94.photobucket.com/albums/l112/TAPE_RULEZ/file_info_wiki.png](http://i94.photobucket.com/albums/l112/TAPE_RULEZ/file_info_wiki.png)

---


# Menu Option h Version and listing of all functions #

This will show the version and build number of the wlm version in use.

On hitting Enter it will go on to show you the help information on using wlm and all the options wlm has.


![http://i94.photobucket.com/albums/l112/TAPE_RULEZ/version_wiki.png](http://i94.photobucket.com/albums/l112/TAPE_RULEZ/version_wiki.png)

_(entering anything else than just 'Enter' will take you back to main menu)_


---


# Menu Option u Check for updates #

_The update function was initially created for use on BackTrack and still needs some fine-tuning to get it to work as intended on other distros._

When running the update function it will check for internet connectivity and if found in order, will continue.

The latest version is downloaded from google code and compares version and build number with the version currently in use.

If found that the downloaded version is newer than the version in use, you will be prompted to accept update or not.

If accepted, then the temp file downloaded will be renamed to 'wlm' and should replace the old wlm file.

Information will be shown on the changes/updates from previous version to the new version.

The script will then stop and prompt to restart.

On restarting you should be running the latest and greatest.


![http://i94.photobucket.com/albums/l112/TAPE_RULEZ/update_wiki.png](http://i94.photobucket.com/albums/l112/TAPE_RULEZ/update_wiki.png)


---


Wiki links;

http://code.google.com/p/wordlist-manipulator/wiki/WLM_USAGE

http://code.google.com/p/wordlist-manipulator/wiki/WLM_OPTIONS