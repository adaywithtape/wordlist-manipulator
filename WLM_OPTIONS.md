# WLM (Wordlist Manipulator) #

![http://i94.photobucket.com/albums/l112/TAPE_RULEZ/wlm_v0-7.png](http://i94.photobucket.com/albums/l112/TAPE_RULEZ/wlm_v0-7.png)

wlm is a wordlist manipulation tool written to provide an easy menu-based possibility to cover the most used manipulation tasks.

wlm was written for use on BackTrack linux, however provided the required permissions are in place it should work on most Linux systems.

wlm is intended to simplify wordlist manipulation tasks by having the most common wordlist manipulation tasks done through a simple menu.


# ALL OPTIONS #


Each main option has a submenu and the full range of options are ;

**1. Case Options;**
  1. Change case of first letter of each word in the wordlist.
  1. Change case of last letter of each word in the wordlist.
  1. Change all lower case to upper case.
  1. Change all upper case to lower case.
  1. Invert case of each letter in each word.



**2. Combination options;**
  1. Combine words from 1 list to all words in another list.
  1. Combine all wordlists in a directory into 1 wordlist.



**3. Prefix characters to wordlist;**
  1. Prefix numeric values in sequence (ie. 0-999)
  1. Prefix fixed number of numeric values in sequence (ie. 000-999)
  1. Prefix a word or characters to wordlist.



**4. Append / Suffix characters to wordlist;**
  1. Suffix numeric values in sequence (ie. 0-999)
  1. Suffix fixed number of numeric values in sequence (ie. 000-999)
  1. Suffix a word or characters to wordlist.



**5. Include characters;**
  1. Include characters from a certain postion from start of word.
  1. Include characters from a certain postion from end of word.



**6. Substitute/Replace characters;**
  1. Substitute/Replace characters from start of word.
  1. Substitute/Replace characters from end of word.
  1. Substitute/Replace characters at specified positions in list.



**7. Optimize / tidy up wordlist;**
  1. Full optimization of wordlist.
  1. Optimize for WPA (min 8 chars max 63 chars).
  1. Sort words based on wordlength.(can help process speed with some programmes such as cRARk)



**8. Split options;**
  1. Split wordlists based on a user defined max linecount in each split file.
  1. Split wordlists based on a user defined max size of each split file.



**9. Removal / Deletion options;**
  1. Remove characters at a certain position from start of word.
  1. Remove characters at a certain position before end of word.
  1. Remove specific characters globally from words.
  1. Removing words containing specific characters from wordlist.
  1. Remove words with more than X number of identical adjacent characters from wordlist.
  1. Remove words existing in 1 list from another list (test version only for small lists).
  1. Remove words that do not have X number of numeric values.
  1. Remove words that have X number of repeated characters.
  1. Remove words of a certain length.



**10. Miscellaneous fun;**
  1. Check possible wordlist sizes (with same min-max length only).
  1. Create a wordlist from a range of dates (datelist).
  1. Strip SSIDs from a kismet generated .nettxt file.
  1. Basic leetify options for wordlist.
  1. Leetify/Permute wordlist (Gitsnik's permute.pl script).


**f. File information;**
> Gives information on aspects of selected file ;
> - Filetype
> - Wordcount of file
> - Longest line
> - File Size
> - first 3 and last 3 lines of file



**h. Version and help information.**



**u. Check for updates to the script.**


---


Wiki Links

http://code.google.com/p/wordlist-manipulator/wiki/WLM_USAGE

http://code.google.com/p/wordlist-manipulator/wiki/WLM_OPTIONS

http://code.google.com/p/wordlist-manipulator/wiki/WLM_EXTENDED_USAGE