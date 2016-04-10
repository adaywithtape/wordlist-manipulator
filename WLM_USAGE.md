# Installing the script #
**BackTrack**

Download the script to directory of your choice, for instance /root/ ;
```
wget -q http://wordlist-manipulator.googlecode.com/svn/wlm -O /root/wlm
```

To allow the script to run make it executable:
```
chmod +x /root/wlm
```


---


**BackBox Linux**

Either follow the same as above for BackTrack, or grab the deb package that ZEROF from BackBox kindly put together;
```
wget http://wordlist-manipulator.googlecode.com/files/wlm-0.8_all.deb
sudo dpkg -i wlm-0.8_all.deb
```

Script can be started in BBox by navigating through the menu to > Auditing > Miscellaneous > wlm.

This method of sarting will (since the above _wlm-0.8\_all.deb_) prompt you for root password and all functions should work seamlessly.

![http://i94.photobucket.com/albums/l112/TAPE_RULEZ/BBOX_WIKI.png](http://i94.photobucket.com/albums/l112/TAPE_RULEZ/BBOX_WIKI.png)

Otherwise script can be started by simply typing 'wlm' in a terminal.


---



# Running the script #

**Running the script when not using a .deb package to install.**

WLM can be used in 2 ways ;
  * List all possible character permutations of a (single) word using Gitsnik's permute.pl script.
  * Alter a wordlist following the options as seen in the options menu.

Running wlm on a single word to list all possible permutations of that word (in this example the word 'one') ;
```
./wlm one
```
![http://i94.photobucket.com/albums/l112/TAPE_RULEZ/wlm_screenshot_06.jpg](http://i94.photobucket.com/albums/l112/TAPE_RULEZ/wlm_screenshot_06.jpg)


---


Running the script to get the options menu ;
```
./wlm
```
![http://i94.photobucket.com/albums/l112/TAPE_RULEZ/wlm_v0-7.png](http://i94.photobucket.com/albums/l112/TAPE_RULEZ/wlm_v0-7.png)



---


# Using the options menu #

All the options from **1** through to **9** work in the same way ;

After choosing the main option in options menu, you are presented with a sub-menu.

After choosing the desired option from the sub-menu, you are prompted to enter an input file and an output file.

_Note that there is **NO** auto-complete, so the full path/file needs to be input manually, you can alternatively drag and drop files to get the path/file_

Then, depending on the option chosen, some further input may be required after which the wordlist will be processed, the output file will be written and a summary of the first and last 3 lines of the newly created file will be shown.

_example of main options menu #1 Case Options_
![http://i94.photobucket.com/albums/l112/TAPE_RULEZ/Screenshot-wlm07.jpg](http://i94.photobucket.com/albums/l112/TAPE_RULEZ/Screenshot-wlm07.jpg)


---


There are verifications in place to check for the existance of the wordlist to be manipulated;

If you enter an incorrect input filename, you will be warned and prompted to enter correct /path/to/wordlist.



There are also some safeguards put in place in the script to ensure that you dont accidentally overwrite existing files;

If you enter an output filename which already exists, you will be warned that it will be overwritten and prompted to either overwrite or cancel the operation.

![http://i94.photobucket.com/albums/l112/TAPE_RULEZ/Screenshot-wlm08.jpg](http://i94.photobucket.com/albums/l112/TAPE_RULEZ/Screenshot-wlm08.jpg)


**_Note!_**

If you are using BBox and have started wlm from the menu, then wlm should be running in root and all should work seamlessly.
If you are using BBox and started wlm thorugh a terminal window, then it is possible that you will be prompted for root password when the script attempts to overwrite an existing file.



---


For information on usage of remaining items;

- tools in Menu Option 10

- File information

- Version and Help Information

- Update function

http://code.google.com/p/wordlist-manipulator/wiki/WLM_EXTENDED_USAGE


---

Wiki Links

http://code.google.com/p/wordlist-manipulator/wiki/WLM_USAGE

http://code.google.com/p/wordlist-manipulator/wiki/WLM_OPTIONS

http://code.google.com/p/wordlist-manipulator/wiki/WLM_EXTENDED_USAGE