`mod_downloader.sh` is a bash script that downloads module (.mod, .xm, .it, .s3m) files from modarchive.org. You can select the amount of files you want to download and use various search criteria as well as save locations for each download session. This is a quick way to get a huge mod library on your computer.

Based on the modarchive script by Fernando Sancho AKA 'toptnc' - https://github.com/toptnc/modarchive, modifications by Justin Wierbonski aka Demonic Sweaters - https://github.com/demonicsweaters/moddownloader, and edits by Milk - https://github.com/mxmilkb/moddownloader

Required packages:
* mikmod, opencp or audacious
* curl
* html2text
* sed
* grep
* awk

Warning: do not run multiple copies at the same time (yet)


```
Mod Downloader options:
  -h               Show this help message
  -n <number>      Number of tracks to download
  -s <section>     Download from selected section: Can be one of this
       uploads     This is a list of the recent member upload activity
       
       featured    These modules have been nominated by the crew for either
                     outstanding quality, technique or creativity
                     (or combination of).
		     
       favourites  These modules have been nominated by the members via their
                     favourites.
		     
       downloads   The top 1000 most downloaded modules, recorded since circa
                     2002.
		     
       topscore    This chart lists the most revered modules on the archive.
       new         Same than uploads but using search engine
       
       random      Ramdom module from entire archive
       
   -a <artist>     Search in artist database
   -m <module>     Search in module database (Title and Filename)
   -g <genre>      Download all of a specific genre: go to modarchive.org
                   genres page http://modarchive.org/index.php?request=view_genres.
                   Hover your mouse over the genre and look for the number in
                   the link address.)

Hint: Use + symbol instead blankspaces in search strings.
Hint 2: if you're running Mac OSX, you must first run this command before the
script will run:
  function _wget() { curl "${1}" -o $(basename "${1}") ; }; alias wget='_wget'
```
