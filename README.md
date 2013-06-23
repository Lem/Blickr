Blickr
======

What you need
-------------

- Some Gems
  - `gpgme`
  - `archive-tar-minitar`
  - `flickraw` 
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
- `blickr -e FILE` encrypt FILE && upload it
- `blickr FILE` upload FILE wihtout encryption

Note
----
This is my very first tool written in ruby. Please keep this in mind while using.

I will add video as soon as downloading your own original video is supported. [It seems that some cool flickr-devs currently working on it].

ToDo
----
* Randomly choosen picture
* Multiple files
* (Video up/download (1GB per file))
* (Asyncron Upload with statusbar)

[API-Key]: http://www.flickr.com/services/apps/create/apply/
[Binwalk]: http://code.google.com/p/binwalk/
[modified version]: https://github.com/Lem/flickraw
[It seems that some cool flickr-devs currently working on it]: http://www.flickr.com/help/forum/en-us/72157633536541721/72157634253091789/
