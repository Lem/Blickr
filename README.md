Blickr
======

What you need
-------------

- Some Gems
  - `archive-tar-minitar`
  - `flickraw` ([modified version] provided in subdir since my pull-request is not accepted yet)
- *[Binwalk]* and *dd* in your $PATH
- Flickr-Account and [API-Key] (Token will be created on runtime)

How does it work?
-----------------
This script will append a choosen file to a 1x1 GIF and uploads it to Flickr.
All IDs of uploaded files will be stored localy.

Examples
--------
- `blickr /etc/passwd` will upload */etc/passwd* as a picture to Flickr
- `blickr -d 3` deletes Photo on position 3 in your localy stored DB.
- `blickr -g 5` downloads and extract your uploaded file with position 5 in DB.
- `blickr -l` lists your DB

ToDo
----
* GPG-Support
* Randomly choosen picture
* Multiple files
* (Asyncron Upload with statusbar)

[API-Key]: http://www.flickr.com/services/apps/create/apply/
[Binwalk]: http://code.google.com/p/binwalk/
[modified version]: https://github.com/Lem/flickraw
