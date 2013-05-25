Blickr
======

What you need
-------------

- Some Perl Modules
  - `Flickr::API2`
  - `Flickr::Upload`
  - `Config::Simple`
  - `Data::Dumper`
  - `Getopt::Std`
  - `LWP::Simple`
  - `File::Basename`
  - `POSIX`
  - `MIME::Base64`
  - `Archive::Tar`
- [Binwalk] in your $PATH
- Flickr-Account and [API-Key] (Token will be created on runtime)

How does it work?
-----------------
This script will append a choosen file to a 1x1 PNG and uploads it to Flickr.
All IDs of uploaded files will be stored localy.

Examples
--------
- `blickr /etc/passwd` will upload */etc/passwd* as a picture to Flickr
- `blickr -d 3` deletes Photo on position 3 in your localy stored DB.
- `blickr -g 5` downloads and extract your uploaded file with position 5 in DB.
- `blickr -l` lists your DB
- `blickr -c` will change your API-Key and Secret. As a result your token will not work anymore so it will be removed. You will not be able to remove file which are uploaded with your previously used API-Key.

ToDo
----
* GPG-Support
* Randomly choosen picture
* Multiple files
* (Asyncron Upload with statusbar)

[API-Key]: http://www.flickr.com/services/apps/create/apply/
[Binwalk]: http://code.google.com/p/binwalk/
